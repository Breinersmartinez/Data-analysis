# Contexto de esta carpeta

## Que es esto

Trabajo del curso Analítica de Datos (709749, semestre 2026-2): un EDA completo sobre regalías mineras en Colombia.
El entregable es **un solo cuaderno**, `EDA_regalias_ANM.ipynb` (83 celdas, 61 de código, 22 de markdown), que ya está ejecutado y con las salidas guardadas dentro.
El dato es un CSV de la ANM en `datos/` (77.369 filas × 15 columnas tal como se descarga); el cuaderno lo lee crudo, lo limpia en los cinco pasos del workflow y cierra con 19 afirmaciones comprobadas contra los datos.

## Como se corre

Siempre desde la raíz de la carpeta, porque la ruta del CSV es relativa a ella.

```bash
.venv/bin/python -m jupyter nbconvert --to notebook --execute EDA_regalias_ANM.ipynb
```

Tarda unos 85 s y debe terminar imprimiendo `RESULTADO: las 19 afirmaciones de la seccion 13 se sostienen en los datos.` Si eso no aparece, el cuaderno está roto: no lo entregues.

Para trabajar el cuaderno a mano: `.venv/bin/jupyter lab`, o abrir el `.ipynb` en VS Code, que ya selecciona `.venv` por `.vscode/settings.json`.

## Convenciones

- Todo en español; los nombres de librerías, métodos y tipos van en inglés (`groupby`, `dropna`, `DataFrame`, `outlier`). Sin emojis en ningún archivo.
- El comentario de arriba de una celda explica **por qué**, no qué hace el código. Lo obvio no se escribe.
- Cada tramo abre y cierra con el mismo banner: `print('=' * 78)`, `print('TRAMO · qué hace')`, `print('=' * 78)`. El rótulo del banner es el mismo que el del título markdown de la sección.
- Una celda = una comprobación. Se cuenta antes de aplicar y se vuelve a contar después, en la misma celda.
- Las columnas de la fuente se conservan tal cual, con mayúsculas y tildes (`Regalías pagadas`). Las derivadas van en snake_case minúscula y sin tilde: `regalias_cop`, `volumen`, `volumen_reportado`, `regalias_por_unidad`, `anio`, `periodo`.
- Los marcos: `df_original` es el crudo y no se toca nunca, `df_clean` es el que se limpia, y en la sección 8 `df` pasa a ser copia del limpio. `df` no se borra ni se reasigna con otro contenido.
- Los tramos van numerados en el markdown (`## 2. Paso 1 del workflow · ...`) y las preguntas de investigación como `P1`..`P5`; las conclusiones las responden en ese orden.
- Números en la salida con `f'{x:,.2f}'` (coma de miles, punto decimal). En el markdown, en español: `1,55 billones`, `78,31%`.
- Gráficos: `plt.style.use('seaborn-v0_8-whitegrid')`, `figsize` explícito, `plt.tight_layout()` y `plt.show()`. Nada de `savefig`: no se exporta nada a disco.
- Los scatter se dibujan sobre `df.sample(6000, random_state=42)` y el tamaño de la muestra se dice en la salida.
- El heatmap de correlación siempre con `center=0, vmin=-1, vmax=1`, y `.corr(numeric_only=True)`.
- Toda comparación de volumen se hace **dentro de una misma `Unidad Medida`**. El total nacional de regalías sí se puede sumar; el total nacional de volumen no se publica en ninguna parte.
- Toda cifra que aparece en las conclusiones se calcula en el diccionario `CIFRAS` (penúltima celda) y se vuelve a comprobar con `comprobar(...)` en la celda final. Si cambias un número del análisis, actualizas las dos.
- El cuaderno no descarga nada de internet: lee el CSV que ya está en `datos/`. Las dos URL de datos.gov.co están solo como procedencia, en la celda 1.
- El `requirements.txt` de la raíz es propio de esta carpeta, no el del curso: sus pisos de versión sustituyen lo que decía el `INSTALACION.md` del material borrado, que ya no existe.
- Las salidas del `.ipynb` están guardadas y hoy son idénticas a una corrida limpia. Si tocas código, re-ejecuta **todas** las celdas antes de decir que terminaste.

## Que NO hacer

- No hacer commit sin que te lo pidan.
- No sumar unidades de medida distintas (gramos con metros cúbicos) ni publicar un total de volumen nacional.
- No rellenar el volumen ausente con cero: `'- 0'` es el centinela de "no reportado" y va a `NaN` (3.399 filas). Rellenarlo rompe exactamente esas filas y la comprobación final lo dice.
- No borrar las 2.002 combinaciones de llave repetida (municipio + mineral + proyecto + año + periodo). Solo se eliminan los 4 duplicados exactos; el resto son liquidaciones distintas y borrarlas sería tirar plata.
- No dejar en el markdown un número escrito a mano que no salga de `CIFRAS`. La celda final existe para que una cifra escrita contradiga a los datos y se note.
- No bajar `pandas`, `numpy`, `scipy` o `scikit-learn` por debajo de los pisos de `requirements.txt`: cambian los resultados y la comprobación final empieza a fallar.
- No borrar ni sobrescribir `df_original`: es el término de comparación de la sección 8.
- No cambiar las cinco preguntas de investigación sin actualizar la sección de conclusiones; son los dos únicos lugares donde se nombran.
