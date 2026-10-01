# Clase 5 · Reto — El campo colombiano, variable por variable

## De qué se trata

En el demo aplicó el marco univariado de 5 pasos a una variable de consumo de agua, con el profesor
al lado. Mirar una variable sola, con su centro, su dispersión, su forma y sus outliers, es
**análisis univariado**: es la mitad del EDA que el Momento 1 pide, y la otra mitad —relacionar dos
variables— es la clase 6. Aquí hay 20.000 registros de producción agrícola de todo el país, y se
aplica el marco tres veces: la primera a mano, paso por paso, y las otras dos con una función ya
escrita. Al final, dos preguntas que se responden comparando entre grupos.

Su trabajo: resolver **siete tareas**, y escribir qué significa cada número que sale.

| Campo | Valor |
|-------|-------|
| Bloque | 3 (es el entregable de la clase) |
| Archivo de trabajo | `reto.ipynb` |
| Dataset | `../datos/evaluaciones_agropecuarias.csv` |
| Tamaño | 20.000 filas x 17 columnas |
| Fuente | Evaluaciones Agropecuarias Municipales (EVA), Ministerio de Agricultura, vía datos.gov.co |
| Tiempo en el salón | 60 minutos |
| Se termina | En casa (la tabla resumen, la validación y la reflexión) |
| Trabajo | Individual o en pareja |
| Entrega | El cuaderno completado, corriendo de arriba a abajo sin errores |

## Cómo está armado el cuaderno

Este reto se recorre solo, leyendo. Nadie dicta los pasos desde el tablero: el profesor circula por
el salón resolviendo dudas. Cada una de las siete tareas trae, en este orden:

| Parte | Qué contiene |
|-------|--------------|
| **La pregunta** | Lo que hay que responder, en español |
| **El concepto** | Qué técnica aplica y por qué esa y no otra |
| **Los comandos** | Las instrucciones exactas que va a usar, escritas de forma genérica |
| **Lo que decide usted** | Qué columna, qué operación, qué criterio. Ahí no hay respuesta escrita |
| **La celda de código** | Los pasos numerados en comentarios; las líneas las escribe usted |
| **La comprobación** | `comprobar('TN', ...)` dice si el resultado es el correcto, sin mostrarlo |

**Por qué esto sigue siendo un reto.** Le damos el camino, pero el camino lo recorre usted sobre un
dataset que no vio en el demo: elige la columna, elige la operación, **clasifica la forma de la
distribución**, **decide qué hacer con los outliers** y **arma solo la secuencia de la última
tarea**. Esas tres no las resuelve ninguna función. La técnica se guía; el criterio no, y el criterio es lo que se evalúa. Las celdas
`comprobar(...)` comparan una huella digital de su resultado con la esperada: nunca revelan la
respuesta, y escribir cualquier cosa hasta que pasen es engañarse en el propio entregable.

## El bucle de la clase 3, aquí

Usted ya tiene el bucle **especificar → planear → ejecutar → validar** y las cuatro skills del
catálogo. Este cuaderno le trae puestos dos tramos —la pregunta de cada tarea es la especificación, y
los pasos numerados son el plan— y le deja los dos que se evalúan:

| Tramo | Dónde pesa en este reto |
|-------|-------------------------|
| **Especificar** | La parte 6 llega en español y sin respuesta. Antes de teclear: qué tabla quiere, con qué columnas, ordenada por qué. Eso es un criterio de aceptación, y sin él la tarea solo se puede terminar, no validar |
| **Planear** | Ahí mismo: los comandos están listados, la secuencia no. El plan es esa secuencia, con lo que hay que mirar en cada paso |
| **Ejecutar** | Un paso, su salida impresa, y parar. Siete tareas de un tirón es lo que esa skill existe para impedir |
| **Validar** | Las cuatro preguntas del analista sobre la tabla resumen. **Siete comprobaciones en verde no son una validación**: dicen que el número coincide, no que la lectura sea correcta |

Pedirle a una IA el análisis completo es legítimo y así quedó dicho en la clase 3. Lo que no se puede
pedir prestado es la lectura, y la entrega pide frases **sin ningún número**. Fíjese en lo que un
modelo no puede saber de este archivo: que `c_d_dep` y `c_d_mun` son códigos y no cantidades. Un
agente le va a reportar ese r = 1,00 como el hallazgo estrella.

---

## El dataset

Las Evaluaciones Agropecuarias Municipales son el censo anual de producción agrícola de Colombia.

**Granularidad:** una fila = **un cultivo, en un municipio, en un año** (2017 o 2018). 32
departamentos, 13 grupos de cultivo.

Las tres variables del reto:

| Columna | Qué es | Unidad |
|---------|--------|--------|
| `producci_n_t` | Producción cosechada | toneladas |
| `rea_sembrada_ha` | Área sembrada | hectáreas |
| `rendimiento_t_ha` | Rendimiento: producción dividida por área | toneladas por hectárea |

Las que se usan para agrupar:

| Columna | Qué es |
|---------|--------|
| `departamento` | Uno de 32 departamentos |
| `municipio` | Municipio |
| `grupo_de_cultivo` | 13 grupos: FRUTALES, CEREALES, OLEAGINOSAS, TUBERCULOS Y PLATANOS, ... |
| `ciclo_de_cultivo` | TRANSITORIO, PERMANENTE o ANUAL |
| `cultivo` | Nombre del cultivo |
| `a_o` | Año: 2017 o 2018 |

**Tres cosas que hay que saber antes de escribir la primera línea:**

1. **Los nombres de columna están mal escritos, y son los reales.** `rea_sembrada_ha` perdió la "á"
   de "área" y `producci_n_t` perdió la "ó" de "producción" al exportarse desde datos.gov.co.
   Cópielos de `df.columns.tolist()`; no los teclee.
2. **Todo el texto está en MAYÚSCULAS y sin tildes.** Filtrar por `'Antioquia'` devuelve cero filas.
3. **Una de las tres variables tiene valores faltantes.** Cuál es, y por qué, es la tarea 1.

Este dataset **no** se limpia hoy: viene sin el problema de separadores de miles que tenía el de
Empocaldas.

---

## Las tareas

### Paso 0 · Cargar y reconocer

Las celdas ya están escritas. Ejecútelas y **deje la salida a la vista**: de ahí va a copiar los
nombres exactos de columnas, grupos y ciclos.

### Parte 1 · Paso 1 del marco: identificar

Objetivo: mirar la variable antes de calcular nada sobre ella. **No tiene tarea**: la celda de los
faltantes viene resuelta, porque la clase 4 fue entera sobre eso. Se ejecuta, se lee la salida y se
escribe una frase: por qué falta rendimiento y no las otras dos.

### Parte 2 · Pasos 2 y 3 sobre `producci_n_t`

Objetivo: centro y dispersión, calculados a mano una vez.

1. **El centro.** Media, mediana y moda de la producción, y la razón media/mediana.
2. **La dispersión.** Q1, Q3, desviación estándar y el IQR.

### Parte 3 · Pasos 4 y 5 sobre `producci_n_t`

Objetivo: las dos partes del marco donde ninguna función responde por usted.

Antes de las tareas hay una celda de acción sin comprobación: el histograma y el boxplot de la
variable, con título y los dos ejes etiquetados.

3. **La forma.** Clasificar la distribución: normal, sesgada a la derecha, sesgada a la izquierda o
   bimodal. Una sola palabra, y tiene que ser coherente con la razón de la tarea 1.
4. **Los outliers.** Los dos límites de la regla 1.5xIQR y el conteo de registros marcados. Después,
   con la tabla de los diez mayores a la vista, la decisión argumentada: ¿se conservan?

### Parte 4 · Las otras dos variables, con la función ya escrita

Objetivo: reconocer que es el mismo procedimiento, y compararlas.

5. **`rea_sembrada_ha` y `rendimiento_t_ha`**, de un golpe. El rendimiento es un **cociente**, y ahí
   está el punto de la parte: su razón media/mediana cae muchísimo respecto a las otras dos. Hay que
   explicar por qué, y mirar los seis rendimientos más altos antes de decidir si se conservan.

### Parte 5 · GroupBy

Objetivo: pasar de un número único a la comparación entre grupos. Las tres decisiones de los M&Ms.

6. **Producción media por grupo de cultivo.** Cuál encabeza, y por qué FLORES Y FOLLAJES queda a
   mitad de tabla pese a ser un renglón exportador clave.

### Parte 6 · Una pregunta que usted arma sola

Objetivo: el ensamblaje. El cuaderno lista todos los comandos que entran en juego, pero **no el
orden**. Es deliberado: en los momentos evaluativos nadie le va a dar la secuencia.

7. **Los grandes productores, ¿son los más eficientes?** Entre los 5 departamentos con mayor
   producción total, cuál tiene el rendimiento mediano más alto.

### Cierre (en casa)

- **La tabla resumen:** las tres variables una por una, con su centro, su forma, sus outliers y la
  medida recomendada. Más una frase por variable **sin ningún número**, de las que se pueden decir en
  voz alta en una reunión donde nadie ha visto el cuaderno.
- **La validación:** las cuatro preguntas del analista sobre esa tabla, una frase cada una. Es la
  celda que separa "el cuaderno corrió" de "la lectura es correcta".
- **Tres preguntas de reflexión**, una de ellas sobre el dataset del proyecto de su equipo.

### Opcional · Solo si terminó todo

No se comprueba ni entra en la retroalimentación: histograma en escala logarítmica, los tres boxplots
lado a lado, y producción total por departamento en barras horizontales.

---

## Cómo se entrega

1. Complete `reto.ipynb`.
2. Antes de entregar: **Kernel → Restart and Run All**. Si algo revienta, arréglelo. Un cuaderno que
   no corre de arriba a abajo le pone techo a Hacer.
3. Verifique que la tabla resumen, sus frases sin números y la validación de las cuatro preguntas
   están escritas.
4. Verifique que cada decisión sobre outliers está **argumentada**, no solo tomada.
5. Súbalo al aula virtual con el nombre `clase05_reto_APELLIDO.ipynb`.
6. Fecha límite: antes del inicio de la clase 6.

## Cómo se valora

**Este reto no produce nota ni cumplido / no cumplido.** Es práctica. La retroalimentación usa el
mismo instrumento de los momentos evaluativos —**Saber, Ser y Hacer, una banda por dimensión**:
Excelente, Bueno, Aceptable, Insuficiente, No aceptable— para que llegue familiarizado a las clases
evaluativas de los tres momentos. **Las tres dimensiones pesan lo mismo** y los elementos de cada fila **no tienen peso**:
no se suman ni se promedian, alimentan una sola banda por dimensión.

| Dimensión | Qué se mira en este reto |
|-----------|--------------------------|
| **Saber** | Las frases de interpretación: qué significa cada número. La razón media/mediana traducida a una frase sobre el campo colombiano, la comparación de las tres razones en la tarea 5, y la tabla resumen con sus frases sin números |
| **Ser** | La decisión sobre los outliers **argumentada** en lugar de aplicada por defecto, sobre todo el contraste entre la tarea 4 (caña azucarera: se conservan) y la 5 (rendimientos de tomate: se marcan y se consultan); y las tres preguntas de reflexión |
| **Hacer** | Las siete tareas con el resultado correcto (el punto de control final las cuenta), la tarea 7 armada por usted, los gráficos con título y ejes etiquetados, y el cuaderno corriendo completo con Restart & Run All |

**Topes por omisión** (techo a la banda, nunca resta, y no se acumulan):

- Respuestas correctas sin ninguna frase de interpretación: **Saber** no pasa de Insuficiente. El
  número no es el análisis; la frase que lo explica sí.
- El cuaderno no corre con Restart & Run All: **Hacer** no pasa de Aceptable.
- Gráficos sin título o sin etiquetas de eje: **Hacer** no pasa de Bueno.
- Una frase que afirme que una variable **causa** otra apoyándose en una diferencia entre grupos:
  **Saber** no pasa de Insuficiente. Que un grupo rinda más no explica por qué. Es la frontera más
  dura del Momento 1 y no se negocia.

## Si se atasca

| Síntoma | Qué revisar |
|---------|-------------|
| `FileNotFoundError` | La ruta es `../datos/evaluaciones_agropecuarias.csv`, relativa al cuaderno. Verifique con `import os; print(os.getcwd())` |
| `KeyError` con el nombre de una columna | Los nombres reales están mutilados. `df.columns.tolist()` y copie y pegue |
| El histograma de `producci_n_t` sale como una sola barra | Es el resultado correcto: el sesgo es tan fuerte que todo se apila contra el cero. Es un hallazgo, no un fallo |
| `.quantile(25)` da un número absurdo y no da error | Recibe una fracción entre 0 y 1: `0.25`, no `25` |
| `TypeError` al combinar dos condiciones | Faltan paréntesis. Cada condición entre paréntesis, sin excepción |
| La tarea 5 dice "sigue valiendo None" | Llamó la función pero no guardó lo que devuelve en una variable |

## Enlaces

- El `demo.ipynb` de esta misma clase tiene el marco de 5 pasos completo sobre otro dataset, con
  los recuadros que explican qué es una media, qué mide la desviación estándar, qué es un objeto
  agrupado y por qué la mediana resiste lo que la media no. Su sección 7 recorre el marco de 5 pasos
  completo de principio a fin: es el modelo de la tabla resumen de este reto. Úselo de referencia.
- Guía de entrega del Momento 1 y qué hace que un dataset sirva:
  `evaluaciones/momento1/guia_entrega.md`, sección 3. Fuente única: los criterios no se duplican aquí.
- Fuente del dataset: https://www.datos.gov.co/resource/2pnw-mmge
- Documentación de pandas sobre GroupBy:
  https://pandas.pydata.org/docs/user_guide/groupby.html
