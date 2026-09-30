# Contexto de esta carpeta

## Qué es esto

Trabajo del curso Analítica de Datos (709749, semestre 2026-2): un EDA completo sobre ventas de BigMart.
El entregable actual es **un solo cuaderno**, `EDA_bigmart_sales.ipynb` (70 celdas: 45 de código y 25 de markdown). Analiza `datos/archive/train.csv`, con 8.523 filas × 12 columnas: una fila representa un producto en una tienda.

El cuaderno cubre los cinco pasos del workflow de limpieza, análisis univariado y bivariado, agregaciones y cinco preguntas de investigación. Es un EDA: no entrena modelos ni genera predicciones. `test.csv` y `sample_submission.csv` se conservan como parte del conjunto BigMart, pero no son insumos de este entregable.

## Cómo se corre

Siempre desde la raíz de la carpeta, porque la ruta `datos/archive/train.csv` es relativa a ella.

```bash
.venv/bin/python -m jupyter nbconvert --to notebook --execute --inplace EDA_bigmart_sales.ipynb
```

La ejecución debe cerrar con `Afirmaciones comprobadas: 24 de 24` y `RESULTADO: las afirmaciones de la seccion 15 se sostienen en los datos.` Si alguno no aparece, el cuaderno está roto y no se entrega.

`EDA_bigmart_sales.nbconvert.ipynb` es el artefacto de una ejecución anterior; no es el cuaderno canónico. Al momento de esta actualización guarda las 45 salidas y las 24 comprobaciones correctas, mientras que el cuaderno canónico aún debe ejecutarse *in place* para guardar sus salidas.

Para trabajar el cuaderno a mano: `.venv/bin/jupyter lab`, o abrir el `.ipynb` en VS Code, que ya selecciona `.venv` por `.vscode/settings.json`.

## Convenciones

- Todo en español; los nombres de librerías, métodos, columnas y tipos de la fuente permanecen en inglés. Sin emojis en ningún archivo.
- El comentario de arriba de una celda explica **por qué**, no qué hace el código. Lo obvio no se escribe.
- Cada tramo abre y cierra con el mismo banner: `print('=' * 78)`, `print('TRAMO · n · qué hace')`, `print('=' * 78)`. El rótulo coincide con el título markdown de la sección.
- Una celda = una comprobación. Si una transformación cambia datos, se cuenta antes y después en esa misma celda.
- Las columnas de la fuente se conservan exactamente como llegan, incluidas las columnas identificadoras. Las variables auxiliares o derivadas usan nombres descriptivos en `snake_case` (`celdas_antes`, `r_fuerte`, `venta_promedio`). No renombrar ni convertir `Item_Identifier` y `Outlet_Identifier` a números: son códigos.
- `df` contiene los datos de trabajo y `df_original = df.copy()` conserva el crudo. `df_original` no se toca nunca y es el término de comparación del tramo 7. No crear una copia superficial con `df_original = df`.
- Los tramos van numerados en el markdown y las preguntas de investigación como `P1`..`P5`; las conclusiones las responden en ese orden.
- Números en la salida con separador de miles y precisión pertinente (`f'{x:,.2f}'`, `f'{n:,}'`). En el markdown, redactar números en español.
- Gráficos: `plt.style.use('seaborn-v0_8-whitegrid')`, tamaño explícito, título, ejes con unidades, `plt.tight_layout()` y `plt.show()`. Nada de `savefig`: no se exportan gráficos a disco.
- Los scatter se dibujan sobre `df.sample(6000, random_state=SEMILLA)` con `SEMILLA = 42`, y la salida declara el tamaño de la muestra.
- El heatmap de correlación usa `center=0, vmin=-1, vmax=1`; la matriz se calcula solo con las cuatro medidas numéricas de producto y venta. No tratar `Outlet_Establishment_Year` como una medida comparable.
- Toda cifra de las conclusiones sale de `CIFRAS` (penúltima celda) y se vuelve a comprobar con `comprobar(...)` en la celda final. Si cambia una cifra del análisis, se actualizan ambas partes.
- El cuaderno no descarga datos de internet: lee los CSV ya presentes. La URL de Kaggle es solo procedencia.
- Las salidas del cuaderno canónico deben estar guardadas y corresponder a una ejecución limpia antes de decir que el trabajo terminó. Si se toca código, se re-ejecutan todas las celdas con el comando anterior.

## Decisiones de datos que no se deben deshacer

- `Item_Weight` se imputa con la mediana de su `Item_Type`; no con una constante ni con la media global.
- `Outlet_Size` solo se reconstruye cuando el dominio lo permite. Las 1.855 filas de `Supermarket Type1` sin tamaño quedan marcadas explícitamente como `Sin dato`; no se les inventa un tamaño.
- Los 526 ceros de `Item_Visibility` son sospechosos pero no imposibles: se conservan y se documentan. No se sustituyen a ciegas.
- No se borra ninguna fila para limpiar este conjunto. La llave natural es `Item_Identifier` + `Outlet_Identifier`; no eliminar filas por esa llave sin demostrar un duplicado real y revisar qué representa una fila.
- `Item_Fat_Content` se normaliza de cinco escrituras a dos categorías (`Low Fat` y `Regular`), sin cambiar el significado de los datos.
- Las asociaciones no demuestran causalidad. Las cuatro características de tienda están ligadas a solo diez tiendas; no presentar una correlación a ese nivel como hallazgo generalizable.

## Qué NO hacer

- No hacer commit sin que te lo pidan.
- No convertir este EDA en un modelo predictivo ni generar un `submission` sin que el usuario amplíe explícitamente el alcance.
- No borrar, sobrescribir ni modificar `df_original`.
- No rellenar todos los nulos de `Outlet_Size` con la moda, una categoría arbitraria o el tamaño de otra tienda.
- No borrar los ceros de `Item_Visibility`, filas raras, outliers o identificadores solo para mejorar una gráfica o una métrica.
- No dejar en el markdown una cifra escrita a mano que no salga de `CIFRAS`.
- No bajar `pandas`, `numpy`, `scipy` o `scikit-learn` por debajo de los pisos de `requirements.txt`: alteraría resultados comprobados.
- No cambiar las cinco preguntas de investigación sin actualizar la sección de conclusiones y las comprobaciones finales.
