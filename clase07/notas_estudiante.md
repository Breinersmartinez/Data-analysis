# Acta Compilada de Retroalimentación — Momento 1: EDA Completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está en la ficha de cada equipo. El cumplido habilita el Momento 3.

---

<!-- INICIO ACTA EQUIPO: Breiner Martinez - Andres Felipe Lopez -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Breiner Martínez, Andrés Felipe López |
| Integrantes | Breiner Martínez, Andrés Felipe López |
| Dataset | [BigMart Sales Prediction (Kaggle / Analytics Vidhya)](https://www.kaggle.com/datasets/brijbhushan/bigmart-sales-data) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Explica correctamente el sesgo a la derecha en `Item_Outlet_Sales` y justifica el uso de la mediana frente a la media. Distingue IQR para dispersión.

**Qué le falta para la banda siguiente:**
> Mantener la fundamentación rigurosa en el Momento 2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular 2 hipótesis de modelo deductivo para M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Responde las 5 preguntas de investigación planteadas en la portada. Articula insights accionables para decisiones de inventario por `Outlet_Type`.

**Qué le falta para la banda siguiente:**
> Articular limitaciones de los datos agregados por tienda sin que se le pregunte.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Agregar sección explícita de sesgos del canal físico en M2. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Limpieza documentada en markdown de `Item_Weight` e `Item_Visibility` (ceros imputados). Histogramas, boxplots, heatmap Seaborn completo y groupby por tienda. 71 celdas ejecutadas sin errores.

**Qué le falta para la banda siguiente:**
> Mantener la calidad del código limpio y modular.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Diseñar pipeline de features para el dashboard en Streamlit. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Bueno |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Equipo sólido con excelente ejecución técnica en 71 celdas y tratamiento riguroso de ceros e imputación por canal.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Tratamiento y documentación en markdown de los valores 0 en `Item_Visibility` imputados por categoría.
2. Análisis bivariado completo con heatmap de correlación y visualizaciones desagregadas por `Outlet_Type`.
3. Excelente organización del notebook con 71 celdas que ejecutan sin errores con Restart & Run All.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** ¿Por qué en `Item_Visibility` imputaron los ceros como faltantes y qué impacto tuvo sobre la correlación con `Item_Outlet_Sales`?
2. **Pregunta:** Notaron que `Supermarket Type3` tiene ventas muy superiores a `Grocery Store`: ¿el `Item_MRP` medio de los productos vendidos en Type3 es más alto o es solo un tema de volumen de rotación?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Profundizar en la discusión de limitaciones de representatividad de las 10 tiendas.
- **Preguntas de investigación que hay que profundizar:** P4 sobre diferencias entre niveles de ciudad que sobreviven al partir el análisis por tipo de tienda.
- **Variables prometedoras para filtros del dashboard:** `Outlet_Type`, `Outlet_Location_Type`, `Item_Type`.
- **Variables prometedoras para KPIs:** Ventas totales por tienda (`Item_Outlet_Sales`), Promedio de MRP por categoría (`Item_MRP`), Ratio de visibilidad promedio.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Breiner Martinez - Andres Felipe Lopez -->

---

<!-- INICIO ACTA EQUIPO: Daniel Fierro - Miguel castiblanco -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Daniel Fierro y Miguel Castiblanco |
| Integrantes | Daniel Fierro, Miguel Castiblanco |
| Dataset | [Precios de Carros Usados en India (CarDekho / Kaggle)](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho) |
| Repositorio de GitHub | [miguel2345678/analisis-carros-usados-o-momento1-analitica-datos](https://github.com/miguel2345678/analisis-carros-usados-o-momento1-analitica-datos) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   | X |   |   |

**Evidencia que sostiene esta banda:**
> Identifican el sesgo severo en el precio de venta y aplican transformación logarítmica, pero no argumentan el cambio en la dispersión tras la transformación ni contextualizan las particularidades del mercado automotriz indio (tráfico, infraestructura y preferencias de combustible/transmisión). Además, eliminaron desjustificadamente variables clave como el número de dueños (`owner`) y el torque.

**Qué le falta para la banda siguiente:**
> Explicar el efecto de la escala logarítmica sobre el rango intercuartílico, contextualizar las condiciones del mercado en la India e interpretar el valor analítico de `owner`, `torque` y el sesgo por outliers extremos en precios.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Redactar párrafo interpretativo de métricas transformadas y justificación teórica del contexto de dominio en India y variables descartadas. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   | X |   |   |

**Evidencia que sostiene esta banda:**
> Presentación estructurada en los 3 objetivos, pero el reparto del tiempo se descompensó en la parte técnica. Responden preguntas con vacíos sobre la ejecución y sobre la segmentación del mercado indio (gamas de vehículos Diésel Automáticos como SUVs de lujo vs. sedanes).

**Qué le falta para la banda siguiente:**
> Mejorar el dominio de la ejecución en vivo, balancear el tiempo hacia los insights de negocio e investigar qué gamas de vehículos explican el comportamiento del mercado indio.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Practicar la sustentación con cronómetro interno de 7 min e investigar la segmentación del mercado indio. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> Repositorio oficial verificado (`https://github.com/miguel2345678/analisis-carros-usados-o-momento1-analitica-datos`) que incluye el dataset original (`car_details_v3_original.csv`), garantizando la reproducibilidad del proyecto. De 45 celdas de código, **44 corrieron perfectamente**; el único error registrado estuvo en la celda 46 al ejecutar `df.to_csv('car_details_v3_limpio.csv')` por un `PermissionError` (archivo abierto simultáneamente en Excel en la máquina local). Adicionalmente, descartaron variables por formato de texto (`torque`) en lugar de limpiarlas en dos columnas numéricas (`torque_nm` y `rpm_torque`), y borraron `owner`.

**Qué le falta para la banda siguiente:**
> Desbloquear los permisos de archivo local en la celda 46 para asegurar la ejecución completa con Restart & Run All y aplicar técnicas de limpieza de texto en lugar de descartar columnas.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Corregir las rutas/permisos de guardado de archivos (`PermissionError`), implementar la extracción de `torque_nm` y `rpm_torque` y recuperar `owner`. | 2026-10-08 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Aceptable |
| Ser | Aceptable |
| Hacer | Insuficiente |

**Dónde está el equipo, en una frase:**

> El proyecto garantiza la reproducibilidad con su repositorio oficial en GitHub y 44 de 45 celdas ejecutadas correctamente, pero requiere desbloquear la celda 46 (`PermissionError` por archivo abierto en Excel) y rescatar variables analíticas descartadas (`owner` y `torque`).

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[X] El equipo queda citado a horario de atención dentro de la semana siguiente.** Fecha: 2026-10-08 14:00

---

## Lo que hicieron bien

1. Repositorio oficial verificado (`https://github.com/miguel2345678/analisis-carros-usados-o-momento1-analitica-datos`) con el dataset original (`car_details_v3_original.csv`), lo que garantiza la reproducibilidad completa.
2. Excelente tasa de ejecución técnica en 44 de las 45 celdas de código de su notebook.
3. Identificación rigurosa de 1.211 filas duplicadas exactas (14,9% del dataset).
4. Aplicación de transformación logarítmica para mitigar el sesgo del precio de venta.
5. Planteamiento de 3 preguntas de investigación claras sobre precio, kilometraje y rendimiento.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Falla celda 46 por PermissionError al exportar CSV (44 de 45 celdas ejecutan perfectamente, CSV original en repo) | Hacer | Hacer no pasa de Insuficiente |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Se verificó que en su repositorio oficial 44 de 45 celdas corren perfectamente y el CSV original está disponible. Sin embargo, la celda 46 arrojó `PermissionError` al intentar exportar `car_details_v3_limpio.csv`. ¿A qué se debió este fallo en el permiso de escritura y cómo se resuelve?
2. **Pregunta:** Eliminaron la columna del número de dueños anteriores (`owner`) y descartaron `torque` por estar en formato texto (ej. '190Nm@ 2000rpm'). ¿Por qué consideraron que `owner` no influye en el precio de reventa? ¿No valía la pena realizar una limpieza de texto separándolo en `torque_nm` y `rpm_torque` en vez de descartarlo?
3. **Pregunta:** ¿El análisis de correlación y precio medio no está fuertemente sesgado por outliers extremos en los precios? Al hallar que los vehículos Diésel Automáticos son los más costosos, ¿investigaron qué tipos/gamas de vehículos (ej. SUVs de lujo vs. sedanes) componen esa categoría en la India y por qué se comportan así?
4. **Pregunta:** El dataset proviene del mercado automotriz de la India. ¿Cómo influyen las condiciones de tráfico, infraestructura y preferencia de combustible/transmisión de ese país en los patrones de precio de reventa encontrados?
5. **Pregunta:** Identificaron 1.211 filas duplicadas exactas (14,9%). ¿Por qué se producen en CarDekho y cuál fue el criterio estadístico para tratarlos?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Ajustar la celda 46 (evitando tener el archivo `.csv` abierto en Excel) para que el notebook corra 100% limpio con Restart & Run All; rescatar `owner` y realizar extracción de texto sobre `torque` para separar `torque_nm` y `rpm_torque`.
- **Preguntas de investigación que hay que profundizar:** Pregunta 2 sobre relación entre rendimiento de combustible (`kmpl`) y precio de venta, incorporando la segmentación por gamas en Diésel Automático y el contexto de tráfico/infraestructura de la India.
- **Variables prometedoras para filtros del dashboard:** `Marca_Carro`, `Tipo_Combustible`, `Tipo_Transmisión`, `Año_Modelo`, `owner`, `torque_nm`.
- **Variables prometedoras para KPIs:** Precio Mediano de Venta, Kilometraje Promedio, Ratio Precio/Kilometraje, Torque Promedio (Nm).

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Daniel Fierro - Miguel castiblanco -->

---

<!-- INICIO ACTA EQUIPO: Javier Orozco Martinez -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Javier Orozco Martínez |
| Integrantes | Javier Orozco Martínez |
| Dataset | [Videojuegos VGChartz 2024 (Kaggle)](https://www.kaggle.com/datasets/gregorut/videogamesales) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   | X |   |   |

**Evidencia que sostiene esta banda:**
> Cálculo de estadísticos descriptivos y lectura de correlación regional.

**Qué le falta para la banda siguiente:**
> Incorporar diagramas de caja para evaluar cuartiles y comparar la variabilidad de ventas entre consolas.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Calcular IQR y construir boxplots por región en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Preguntas de investigación claras en la portada del notebook y buena estructura de historia.

**Qué le falta para la banda siguiente:**
> Reconocer de forma explícita las limitaciones de cobertura de datos en el portal VGChartz para lanzamientos recientes.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Incluir celda de sesgos de datos de VGChartz. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   | X |   |   |

**Evidencia que sostiene esta banda:**
> Tope por omisión: incluyó histogramas y barras pero omitió boxplots para visualizar la dispersión y outliers de ventas globales.

**Qué le falta para la banda siguiente:**
> Incluir gráficos de boxplot para todas las variables cuantitativas clave.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Generar `sns.boxplot` para ventas globales y regionales. | 2026-10-15 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Aceptable |
| Ser | Bueno |
| Hacer | Aceptable |

**Dónde está el equipo, en una frase:**

> Análisis conceptual y narrativa sólida con preguntas claras en la portada del notebook, pero limitado técnicamente por el tope por omisión de boxplots.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Uso sobresaliente del concepto de la regla 80/20 (Pareto) para explicar la concentración de ventas.
2. Comparación regional clara entre mercados (Norteamérica, Europa y Japón).
3. Preguntas de investigación claras en la portada del notebook y buena estructura de historia.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Solo histogramas, sin boxplots ni estadísticos completos de dispersión | Hacer | Hacer no pasa de Aceptable |


---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Incluiste histogramas para las ventas globales, pero omitiste los boxplots. Dado que la distribución de ventas está fuertemente sesgada por títulos taquilleros (ej. Wii Sports o GTA V), ¿cómo identificaste los outliers extremos y el rango intercuartílico (IQR) sin un gráfico de caja y bigotes?
2. **Pregunta:** Al analizar las ventas por región en tus agrupaciones (`groupby`), ¿qué diferencias encontraste entre las preferencias de plataformas y géneros en Japón frente a Norteamérica y Europa?
3. **Pregunta:** En tu matriz de correlación, ¿las ventas en Norteamérica correlacionan más fuerte con Europa o con Japón? ¿Qué te dice esa diferencia sobre la similitud de los mercados?

---

## Recomendaciones clave para llevar al Momento 2

- **Incorporar Boxplots:** Graficar boxplots de ventas por género y plataforma para identificar visualmente los outliers taquilleros y calcular el IQR.
- **Segmentación de Outliers:** Aislar los blockbuster (Top 10 en ventas) del resto del catálogo para analizar si la tendencia en juegos de presupuesto medio difiere.
- **Preguntas de investigación que hay que profundizar:** P1 sobre la variación de preferencias por género entre NA, EU y JP.
- **Variables prometedoras para filtros del dashboard:** `Plataforma`, `Género`, `Año_Lanzamiento`.
- **Variables prometedoras para KPIs:** Ventas Globales Totales, Ventas Regionales Promedio, Porcentaje de Concentración de Top 10 Juegos.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Javier Orozco Martinez -->

---

<!-- INICIO ACTA EQUIPO: Jhossymar Garces Angulo -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Jhossymar Garcés Angulo |
| Integrantes | Jhossymar Garcés Angulo |
| Dataset | Infecciones Asociadas a la Atención en Salud en UCI (OSB / datos.gov.co) — **Sin URL de procedencia declarada** |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> Confusión estadística entre una suma matemática (tautología de género: confundió la suma de hombres + mujeres con una correlación de riesgo de r=0.98) y un análisis de riesgo real. Omisión de tasas estandarizadas por 1.000 días de exposición/estancia. Muestra solo conteos básicos y agregados por UCI, sin calcular ni interpretar medidas de tendencia central, dispersión ni forma en distribuciones numéricas.

**Qué le falta para la banda siguiente:**
> Diferenciar sumas aritméticas de análisis de riesgo estadístico, calcular e interpretar media, mediana, desviación estándar e IQR para la estancia y estandarizar tasas por 1.000 días de exposición.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Construir tabla descriptiva completa con tasas estandarizadas por 1.000 días e interpretación analítica en markdown. | 2026-10-08 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> Fallo en la sustentación en vivo: la exposición careció de estructura, tuvo serias dificultades para sostener la narrativa de su trabajo, no pudo responder con solvencia las preguntas de su propio análisis y la presentación en vivo no transmitió dominio técnico ni seguridad sobre las decisiones del notebook. Conclusiones basadas en obviedades de conteos brutos (confundió la suma de hombres + mujeres con una correlación de riesgo de género de r=0.98 y omitió tasas por 1.000 días de estancia).

**Qué le falta para la banda siguiente:**
> Estructurar la exposición verbal con solvencia y dominio técnico, fundamentar las conclusiones en evidencia cuantitativa real y sustentar con seguridad la narrativa del notebook.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Redactar conclusiones analíticas basadas en evidencia cuantitativa y preparar la estructura de sustentación para la cita de atención. | 2026-10-08 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> EL NOTEBOOK CONTIENE SOLO 5 CELDAS EN TOTAL (2 MD y 3 CÓDIGO). Dataset de 576 filas (incumple la consigna de 5.000 a 10.000 filas). Sin URL de procedencia declarada. Carece de análisis univariado (sin histogramas, sin boxplots). Solo 1 groupby básico y 1 heatmap directo.

**Qué le falta para la banda siguiente:**
> Cumplir la consigna de volumen de dataset (5.000 a 10.000 filas), declarar la URL de procedencia y desarrollar un notebook con flujo completo de limpieza, univariado (hist + boxplots), bivariado y markdown expositivo.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Cargar/ampliar el dataset al volumen requerido (5.000-10.000 filas), declarar URL de origen y desarrollar el notebook completo siguiendo la plantilla del curso. | 2026-10-08 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Insuficiente |
| Ser | Insuficiente |
| Hacer | Insuficiente |

**Dónde está el equipo, en una frase:**

> Entrega e interacción en vivo gravemente deficientes: notebook de 5 celdas con dataset de 576 filas sin URL, confusión entre sumas brutas y correlación de riesgo, y fallo en la sustentación verbal, requiriendo reestructuración total inmediata para no inhabilitar M3.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, pero al borde de la inhabilitación para el Momento 3.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[X] El equipo queda citado a horario de atención dentro de la semana siguiente.** Fecha: 2026-10-07 15:00 (Citación obligatoria en horario de atención por 3 dimensiones en Insuficiente y fallo en la sustentación en vivo).

---

## Lo que hicieron bien

1. Selección de un dataset relevante en salud pública sobre infecciones intrahospitalarias en UCI (OSB Bogotá).
2. Planteamiento inicial de preguntas asociadas a factores de riesgo en unidades de cuidados intensivos.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Sin análisis univariado real (sin histogramas, sin boxplots) | Hacer | Hacer en Insuficiente |
| Dataset de 576 filas (incumple consigna de 5.000 a 10.000 filas) y sin URL declarada | Hacer | Hacer en Insuficiente |
| Confusión estadística entre suma de conteos brutos y análisis de correlación/riesgo | Saber | Saber en Insuficiente |
| Fallo en la sustentación en vivo (falta de estructura e insolvencia en Q&A) | Ser | Ser en Insuficiente |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Tu entregable consta únicamente de 5 celdas (3 de código) y un dataset de 576 filas sin URL declarada. ¿Dónde está la caracterización univariada con histogramas y boxplots de las tasas de infección o días de estancia?
2. **Pregunta:** Afirmas que existe una correlación de r=0.98 en el riesgo por género, pero solo sumaste conteos brutos de hombres y mujeres. ¿Cómo diferencias una suma aritmética de una verdadera correlación de riesgo estandarizada por 1.000 días de estancia?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Reestructurar el notebook incorporando un dataset de volumen adecuado (5.000 a 10.000 filas), declarando la URL de procedencia y agregando histogramas, boxplots y bivariado explicativo.
- **Preguntas de investigación que hay que profundizar:** Reformular la evaluación de riesgo por género y tipo de UCI utilizando tasas estandarizadas por 1.000 días de estancia.
- **Variables prometedoras para filtros del dashboard:** `Tipo_UCI`, `Procedimiento_Invasivo`, `Grupo_Etario`.
- **Variables prometedoras para KPIs:** Tasa de Infección por 1.000 Días de Estancia, Promedio de Días de Estancia en UCI, Total de Eventos Adversos Reportados.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Jhossymar Garces Angulo -->

---

<!-- INICIO ACTA EQUIPO: Juan Munoz Caiced -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja |
| Integrantes | Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja |
| Dataset | [10.000 Empresas más Grandes del País (Supersociedades, datos.gov.co 2021-2025)](https://www.datos.gov.co/Econom-a-y-Finanzas/10-000-Empresas-m-s-Grandes-del-Pa-s/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |


> **NOTA DE CONSOLIDACIÓN DE ENTREGA:** Se certifica que esta entrega realizada en el directorio individual `Juan Munoz Caiced` es IDÉNTICA a la entregada en la carpeta grupal `Sebastián Muñoz - Angélica Aguirre - Alexandra Merchan`. Se evalúa como un único trabajo en equipo de 3 integrantes (Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja).


---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Demuestra de forma sobresaliente la necesidad de usar medianas y transformaciones logarítmicas por la presencia de megaempresas (Ecopetrol/Terpel). Explica asimetría e IQR con maestría.

**Qué le falta para la banda siguiente:**
> Mantener este nivel conceptual de cara al modelado multivariado en M2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular indicadores de rentabilidad relativa (ROA/ROE) en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Genera 4 insights económicos de alto impacto sobre la concentración de ganancias por macrosector y región. Reconoce explícitamente las limitaciones de datos autorreportados a Supersociedades.

**Qué le falta para la banda siguiente:**
> Mantener el ritmo de trabajo colaborativo y la coherencia narrativa.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Crear prototipo de visualización ejecutiva en Streamlit. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Notebook de 64 celdas impecable. Justificación explícita en markdown de la conservación de atípicos (empresas reales), histogramas, boxplots logarítmicos, heatmap completo y `groupby` multinivel.

**Qué le falta para la banda siguiente:**
> Mantener la estructura limpia de código.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Optimizar consultas de agregación para el dashboard. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Trabajo de nivel profesional con tratamiento riguroso de escalas logarítmicas y justificación madura de atípicos.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Justificación teórica y empírica impecable de la conservación de valores atípicos superiores en empresas reales.
2. Uso correcto de escalas logarítmicas para corregir la extrema asimetría en ingresos y activos.
3. Notebook de 64 celdas sumamente estructurado con respuestas rigurosas a las 4 preguntas de investigación.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Al analizar los ingresos operacionales aplicaron una escala logarítmica para los boxplots. ¿Cuál fue la brecha exacta entre media y mediana en el sector Minero-Energético frente al Comercio?
2. **Pregunta:** En la celda 2.5 justificaron conservar los valores atípicos superiores en vez de eliminarlos. ¿Por qué eliminar un outlier como Ecopetrol alteraría la respuesta sobre concentración de mercado?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Mantener el pipeline limpio para la construcción de vistas interactivas.
- **Preguntas de investigación que hay que profundizar:** P3 sobre relaciones entre ingresos, activos y niveles de endeudamiento.
- **Variables prometedoras para filtros del dashboard:** `Macrosector`, `Región`, `Departamento`, `Año`.
- **Variables prometedoras para KPIs:** Ingresos Operacionales Totales, Mediana de Ganancia/Pérdida, Margen de Endeudamiento Promedio.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Juan Munoz Caiced -->

---

<!-- INICIO ACTA EQUIPO: Kevin  Lopez - Daniel Zamora - Julián Arévalo -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Kevin López, Daniel Zamora, Julián Arévalo |
| Integrantes | Kevin López, Daniel Zamora, Julián Arévalo |
| Dataset | [Colombianos Detenidos en el Exterior (Cancillería / datos.gov.co 2018-2025)](https://www.datos.gov.co/Relaciones-Exteriores/Colombianos-Detenidos-en-el-Exterior/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Explican adecuadamente las distribuciones de conteos por consulado y la asimetría de delitos. Relacionan correctamente el volumen de detenidos en Madrid (12,3%) con la dinámica migratoria y ejecutan comparaciones cruzadas entre tipos de delito y ubicación.

**Qué le falta para la banda siguiente:**
> Anticipar espontáneamente en markdown la justificación del uso de porcentajes relativos frente a absolutos y profundizar en la caracterización cruzada de delitos específicos (narcotráfico vs. delitos migratorios o contra la propiedad).

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Incorporar análisis de tasas por cada 100.000 colombianos en el exterior y desgloses de crosstab por consulado. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Responden con claridad las 3 preguntas (consulados líderes, evolución temporal y diferencias de género/situación jurídica). Participan los 3 integrantes y analizan las causas de la concentración de detenidos en Madrid.

**Qué le falta para la banda siguiente:**
> Evaluar a fondo el sesgo por el tamaño de la comunidad migrante residente en España, convenios judiciales o políticas migratorias europeas, además de discutir las limitaciones de subregistro institucional en Cancillería.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Redactar sección de sesgos migratorios, convenios judiciales y limitaciones de Cancillería. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Notebook de 66 celdas muy robusto. Normalización de cadenas de texto complejas (`NO REPORTA – CONFIDENCIALIDAD ESTATAL`), histogramas, boxplots, tablas cruzadas (`crosstab` / `groupby`) de delito vs. ubicación y heatmap bivariado por género y consulado.

**Qué le falta para la banda siguiente:**
> Mantener el orden del pipeline de preprocesamiento de texto y modularizar las funciones de tabulación cruzada.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Documentar funciones helpers de limpieza y tablas cruzadas para M2. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Bueno |
| Ser | Bueno |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Excelente trabajo técnico de preprocesamiento de texto y análisis bivariado cruzado sobre datos de la Cancillería, con buena articulación del contexto migratorio en Madrid.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Normalización avanzada de cadenas de texto complejas con guiones en categorías de confidencialidad.
2. Análisis bivariado completo con tablas cruzadas (`crosstab` / `groupby`) y heatmap de distribución por delito, género y consulado.
3. Evaluación inicial de la concentración de detenidos en Madrid y excelente participación de los 3 integrantes con notebook de 66 celdas perfectamente ejecutable.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** En el preprocesamiento de datos se encontraron con variaciones en `NO REPORTA – CONFIDENCIALIDAD ESTATAL`. ¿Qué técnica de limpieza de strings aplicaron en Python para evitar fragmentación en el groupby?
2. **Pregunta (Concentración Geográfica y Causas):** El consulado de Madrid presenta la mayor concentración de detenidos (12,3%). ¿Por qué creen que en Madrid hay más detenidos que en otros consulados? ¿Evaluaron el sesgo por el tamaño de la comunidad migrante colombiana residente en España, los convenios judiciales de repatriación/cooperación o las políticas migratorias europeas?
3. **Pregunta (Cruce Bivariado Delito vs. Ubicación):** ¿Hicieron la comparación cruzada (`crosstab` / `groupby`) entre tipos de delito y ubicación/consulado? ¿Qué arrojó ese cruce respecto a qué delitos específicos (ej. narcotráfico vs. delitos migratorios o contra la propiedad) empujan las cifras en Madrid frente a los consulados de Estados Unidos o Latinoamérica?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Agregar contextualización con estimaciones poblacionales de residentes en el exterior (tasas por cada 100.000 habitantes) para evaluar adecuadamente la concentración en Madrid.
- **Preguntas de investigación que hay que profundizar:** P3 sobre diferencias por género y ubicación en la tabla cruzada de tipos de delito (narcotráfico vs. migratorios o propiedad).
- **Variables prometedoras para filtros del dashboard:** `Consulado`, `País`, `Delito_Grupo`, `Género`, `Situación_Jurídica`, `Año`.
- **Variables prometedoras para KPIs:** Total de Detenidos, Tasa por 100k residentes, Porcentaje de Condenados vs Procesados, Top Delito Específico por Consulado (Madrid vs. EE. UU. vs. LatAm).

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Kevin  Lopez - Daniel Zamora - Julián Arévalo -->

---

<!-- INICIO ACTA EQUIPO: Maria Norena Rodriguez - Zharick Rivera -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | María José Noreña Rodríguez y Zharick Rivera |
| Integrantes | María José Noreña Rodríguez, Zharick Rivera |
| Dataset | [Pima Indians Diabetes (Kaggle / UCI Machine Learning Repository)](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Trata ceros fisiológicos como missing values, imputa por mediana, analiza asimetría e IQR con rigor estadístico.

**Qué le falta para la banda siguiente:**
> Mantener el rigor en la selección de métricas robustas en el Momento 2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular hipótesis de modelos deductivos para M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Informe analítico estructurado en `reports/informe_analitico.md`, arquitectura limpia y profesional con justificación clara de negocio.

**Qué le falta para la banda siguiente:**
> Mantener la calidad expositiva y profundizar en recomendaciones de negocio.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Diseñar prototipo de visualización ejecutiva en Streamlit. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Código modular en `src/analisis.py` (17 KB), análisis univariado, bivariado, multivariado con correlación, heatmap, boxplots y outliers por IQR.

**Qué le falta para la banda siguiente:**
> Mantener la calidad del código modular y reproducible.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Conectar los scripts modulares de `src/analisis.py` con el dashboard interactivo. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Excelente trabajo técnico y analítico con arquitectura modular profesional en Python (`src/analisis.py`), tratamiento riguroso de ceros fisiológicos e IQR, y completa caracterización bivariada y multivariada.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Modularización profesional del código en `src/analisis.py` con funciones reutilizables (`prepare_data`, `save_univariate`, `save_bivariate`, `save_multivariate`, `iqr_outliers`, `write_report`).
2. Identificación y tratamiento riguroso de ceros físicamente imposibles en variables médicas mediante imputación por mediana y análisis de IQR.
3. Excelente informe de investigación analítica en `reports/informe_analitico.md` e integración completa de análisis bivariado, matriz de correlación, heatmap y boxplots.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Impacto de Imputación Masiva en la Correlación (Análisis de Sensibilidad):** *"Imputaron casi la mitad de los datos de insulina (374 registros de 768) con la mediana. ¿Cómo afectó esa concentración artificial en el centro a la correlación que observaron entre la insulina y la diabetes? ¿Si hubieran eliminado esas filas en vez de imputarlas, creen que la insulina habría mostrado una asociación más fuerte?"*
2. **Interpretación de Pearson vs. Spearman (Estadística Conceptual):** *"En su informe compararon Pearson y Spearman. En la variable edad, el coeficiente de Spearman ($\rho=0.309$) fue considerablemente mayor que el de Pearson ($r=0.238$). ¿Qué les dice esa diferencia sobre la forma de la relación entre la edad y el riesgo de diabetes? ¿Es lineal o monótona no lineal?"*
3. **Desbalance de Clase y Matriz de Confusión de Salud Pública (Toma de Decisiones):** *"Reportaron una prevalencia del 35% de casos positivos. Si una entidad de salud usara su análisis para priorizar programas de prevención, ¿qué es más costoso o riesgoso: un Falso Positivo (evaluar a alguien sano) o un Falso Negativo (dejar sin diagnosticar a alguien enfermo)? ¿Cómo impacta esto la métrica de decisión?"*
4. **Generalización y Sesgo de Cohorte (Pensamiento Crítico):** *"El dataset estudia una cohorte específica de mujeres de la comunidad Pima de Arizona. ¿Por qué razones genéticas o de estilo de vida sus hallazgos no se pueden extrapolar directamente a una población en Colombia sin ajustes previos?"*

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Integrar las funciones modulares de `src/analisis.py` en la carga y procesamiento dinámico del dashboard en Streamlit.
- **Preguntas de investigación que hay que profundizar:** Evaluar el impacto relativo del IMC frente a la edad en la probabilidad de diagnóstico positivo de diabetes.
- **Variables prometedoras para filtros del dashboard:** `Edad_Grupo`, `Diagnóstico`, `Nivel_Glucosa`.
- **Variables prometedoras para KPIs:** Promedio de Glucosa, Mediana de IMC, Proporción de Casos Positivos (Outcome=1), Conteo de Insumos/Pacientes Imputados.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Maria Norena Rodriguez - Zharick Rivera -->

---

<!-- INICIO ACTA EQUIPO: Monica Alejandra Morales - Samuel Moreno -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Mónica Alejandra Morales, Samuel Moreno |
| Integrantes | Mónica Alejandra Morales, Samuel Moreno |
| Dataset | [10.000 Empresas más Grandes de Colombia (Supersociedades, datos.gov.co 2026/2021)](https://www.datos.gov.co/Econom-a-y-Finanzas/10-000-Empresas-m-s-Grandes-del-Pa-s/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Calculan e interpretan correctamente medias y medianas por macrosector y región, notando el sesgo impuesto por la concentración en Bogotá/Cundinamarca.

**Qué le falta para la banda siguiente:**
> Profundizar en la justificación formal del IQR frente a la desviación estándar al comparar sectores heterogéneos.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Justificar cuantitativamente el uso de IQR en la memoria de M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Responden a las 3 preguntas de investigación (macrosectores por ingresos, regiones por ingresos y volumen de empresas). Presentan informe PDF de soporte. Sin embargo, aunque el análisis y la limpieza son sólidos, falta mayor profundidad en el hilo conductor que explique las causas reales de la concentración geográfica y sectorial.

**Qué le falta para la banda siguiente:**
> Profundizar en el hilo conductor que explique las causas reales de la concentración geográfica (efecto sede corporativa en Bogotá) y sectorial (volumen de Comercio).

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Agregar sección de recomendaciones explicativas y análisis de causa raíz. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Notebook de 45 celdas ordenado y ejecutable. Buena limpieza de datos y excelente estructuración inicial del dataset. Histogramas, boxplots de ingresos/ganancias, matriz de correlación Seaborn y `groupby` por región y sector.

**Qué le falta para la banda siguiente:**
> Incluir celdas de análisis bivariado adicionales para cruzar pasivos vs patrimonio.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Incorporar scatter plots de endeudamiento vs rentabilidad. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Bueno |
| Ser | Bueno |
| Hacer | Bueno |

**Dónde está el equipo, en una frase:**

> Trabajo sólido y estructurado respaldado con un informe PDF de buena presentación ejecutiva, con buena limpieza de datos y excelente estructuración inicial del dataset, aunque requiere profundizar en el hilo conductor.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Buena limpieza de datos y excelente estructuración inicial del dataset.
2. Excelente informe gráfico complementario en PDF (`MOMENTO 1 MONICA - SAMUEL.pdf`).
3. Análisis univariado y bivariado completo con visualizaciones claras de ingresos y ganancias.
4. Notebook de 45 celdas limpio que ejecuta de principio a fin.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** *"Si realizáramos la segmentación por tamaño de empresa (no solo ver las 10.000 como un bloque, sino pequeñas vs. medianas vs. gigantes), ¿qué patrones diferentes surgirían en la rentabilidad y activos?"*
2. **Pregunta:** *"¿Identificaron empresas atípicas gigantes (como Ecopetrol o Terpel) que estén halando hacia arriba las cifras de sus macrosectores? ¿Qué pasa si las remueven del cálculo?"*
3. **Pregunta:** *"Bogotá aparece como la región más grande en ingresos. ¿Es porque la actividad comercial ocurre físicamente allí, o porque las multinacionales tienen registrada su sede principal/fiscal en Bogotá (efecto sede corporativa) aunque operen en todo el país?"*
4. **Pregunta:** *"¿Qué factores específicos explican que el macrosector Comercio represente un volumen de ingresos tan desproporcionadamente alto frente a otros sectores?"*

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Profundizar en el hilo conductor que explique las causas reales de la concentración geográfica (efecto sede corporativa vs. actividad real) y sectorial (desproporción de Comercio), e incluir el análisis bivariado pasivo/patrimonio.
- **Preguntas de investigación que hay que profundizar:** P1 sobre concentración de ingresos por macrosector, segmentación por tamaño de empresa y aislamiento de atípicos gigantes (Ecopetrol/Terpel).
- **Variables prometedoras para filtros del dashboard:** `Macrosector`, `Región`, `Departamento`.
- **Variables prometedoras para KPIs:** Ingresos Totales por Región, Mediana de Ganancias por Sector, Número de Empresas Activas.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Monica Alejandra Morales - Samuel Moreno -->

---

<!-- INICIO ACTA EQUIPO: Sebastián Muñoz - Angélica Aguirre - Alexandra Merchan -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja |
| Integrantes | Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja |
| Dataset | [10.000 Empresas más Grandes del País (Supersociedades, datos.gov.co 2021-2025)](https://www.datos.gov.co/Econom-a-y-Finanzas/10-000-Empresas-m-s-Grandes-del-Pa-s/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |


> **NOTA DE CONSOLIDACIÓN DE ENTREGA:** Se certifica que esta entrega realizada en la carpeta grupal `Sebastián Muñoz - Angélica Aguirre - Alexandra Merchan` es IDÉNTICA a la entregada en el directorio individual `Juan Munoz Caiced`. Se evalúa como un único trabajo en equipo de 3 integrantes (Juan Sebastián Muñoz Caicedo, Angélica Aguirre Paz, Alexandra Merchán Pantoja).


---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Demuestra de forma sobresaliente la necesidad de usar medianas y transformaciones logarítmicas por la presencia de megaempresas (Ecopetrol/Terpel). Explica asimetría e IQR con maestría.

**Qué le falta para la banda siguiente:**
> Mantener este nivel conceptual de cara al modelado multivariado en M2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular indicadores de rentabilidad relativa (ROA/ROE) en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Genera 4 insights económicos de alto impacto sobre la concentración de ganancias por macrosector y región. Reconoce explícitamente las limitaciones de datos autorreportados a Supersociedades.

**Qué le falta para la banda siguiente:**
> Mantener el ritmo de trabajo colaborativo y la coherencia narrativa.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Crear prototipo de visualización ejecutiva en Streamlit. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Notebook de 64 celdas impecable. Justificación explícita en markdown de la conservación de atípicos (empresas reales), histogramas, boxplots logarítmicos, heatmap completo y `groupby` multinivel.

**Qué le falta para la banda siguiente:**
> Mantener la estructura limpia de código.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Optimizar consultas de agregación para el dashboard. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Trabajo de nivel profesional con tratamiento riguroso de escalas logarítmicas y justificación madura de atípicos.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Justificación teórica y empírica impecable de la conservación de valores atípicos superiores en empresas reales.
2. Uso correcto de escalas logarítmicas para corregir la extrema asimetría en ingresos y activos.
3. Notebook de 64 celdas sumamente estructurado con respuestas rigurosas a las 4 preguntas de investigación.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Al analizar los ingresos operacionales aplicaron una escala logarítmica para los boxplots. ¿Cuál fue la brecha exacta entre media y mediana en el sector Minero-Energético frente al Comercio?
2. **Pregunta:** En la celda 2.5 justificaron conservar los valores atípicos superiores en vez de eliminarlos. ¿Por qué eliminar un outlier como Ecopetrol alteraría la respuesta sobre concentración de mercado?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Mantener el pipeline limpio para la construcción de vistas interactivas.
- **Preguntas de investigación que hay que profundizar:** P3 sobre relaciones entre ingresos, activos y niveles de endeudamiento.
- **Variables prometedoras para filtros del dashboard:** `Macrosector`, `Región`, `Departamento`, `Año`.
- **Variables prometedoras para KPIs:** Ingresos Operacionales Totales, Mediana de Ganancia/Pérdida, Margen de Endeudamiento Promedio.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Sebastián Muñoz - Angélica Aguirre - Alexandra Merchan -->

---

<!-- INICIO ACTA EQUIPO: Vanesa Otero - Samuel Escobar -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Vanesa Otero y Samuel Escobar |
| Integrantes | Vanesa Otero, Samuel Escobar |
| Dataset | [Asignación de Dosis de Vacunas COVID-19 en Colombia (MinSalud / datos.gov.co)](https://www.datos.gov.co/Salud-y-Protecci-n-Social/Asignaci-n-de-dosis-de-vacuna-contra-COVID-19/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Justificaron de forma impecable que el dataset solo cuenta con una variable cuantitativa continua principal (cantidad de dosis por resolución), por lo que construir una matriz de correlación o heatmap de 1x1 no tenía sentido matemático ni analítico. El profesor validó y destacó positivamente esta defensa ("Me encantó esa respuesta. Bien justificado").

**Qué le falta para la banda siguiente:**
> Profundizar en la interacción entre la variable cuantitativa continua y las variables categóricas clave (laboratorio, departamento).

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Analizar la variabilidad entre grupos por laboratorio y departamento para M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   | X |   |   |

**Evidencia que sostiene esta banda:**
> Presentación clara y estructurada centrada en responder preguntas de la operación logística de MinSalud, pero a las conclusiones les falta un hilo conductor y un cierre más contundente sobre el impacto real de la distribución de vacunas (equidad territorial, logística de ultracongelación).

**Qué le falta para la banda siguiente:**
> Articular una conclusión de política pública e impacto real de negocio más fuerte con recomendaciones estratégicas al Ministerio de Salud.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Fortalecer la narrativa analítica y redactar recomendaciones estratégicas de política pública. | 2026-10-15 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   | X |   |

**Evidencia que sostiene esta banda:**
> Notebook de 30 celdas con excelente análisis univariado, boxplots por laboratorio/departamento, agrupaciones (groupby) y limpieza sólida. Se elimina el tope por omisión al validarse que no aplicaba matriz de correlación sobre 1 variable continua.

**Qué le falta para la banda siguiente:**
> Incorporar análisis bivariado avanzado agrupando variables categóricas con la continua y estructurar vistas analíticas para el dashboard.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Enriquecer la caracterización bivariada cuantitativa-categórica para M2. | 2026-10-15 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Bueno |
| Ser | Aceptable |
| Hacer | Bueno |

**Dónde está el equipo, en una frase:**

> Excelente defensa técnica de por qué no aplicaba la correlación sobre 1 variable continua, con trabajo sólido en univariado y limpieza, pero requiriendo mayor punch e hilo conductor en sus conclusiones de política pública.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Excelente defensa técnica validada positivamente por el profesor sobre por qué no aplicaba construir una matriz de correlación 1x1 al tener una sola variable cuantitativa continua.
2. Limpieza sólida de datos y construcción de análisis univariado completo con boxplots por laboratorio y departamento.
3. Estructuración clara de la operación logística y reparto equilibrado del tiempo entre integrantes.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto (Tope por omisión de heatmap eliminado tras validación técnica) |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Justificaron muy bien por qué no tenía sentido un heatmap con una sola variable numérica. ¿Qué variable categórica (ej. laboratorio o departamento) explicó la mayor parte de la variación en la asignación de dosis?
2. **Pregunta:** Al analizar la distribución por regiones, ¿qué conclusión alcanzaron sobre las barreras logísticas de ultracongelación (Pfizer vs. Sinovac) en departamentos periféricos?
3. **Pregunta:** Si tuvieran que entregarle este análisis al Ministerio de Salud para una futura emergencia Sanitaria, ¿cuál es la recomendación central con la que cerrarían su conclusión?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Construir un hilo conductor claro en las conclusiones y articular recomendaciones impactantes para el Ministerio de Salud.
- **Preguntas de investigación que hay que profundizar:** Brecha entre dosis asignadas por resolución y dosis efectivamente aplicadas, y barreras logísticas de ultracongelación en zonas periféricas.
- **Variables prometedoras para filtros del dashboard:** `Departamento`, `Laboratorio_Vacuna`, `Año`.
- **Variables prometedoras para KPIs:** Total Dosis Asignadas, Número de Resoluciones, Cobertura por Laboratorio.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Vanesa Otero - Samuel Escobar -->

---

<!-- INICIO ACTA EQUIPO: Yovanny Lozano Reyes -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Yovanny Lozano Reyes |
| Integrantes | Yovanny Lozano Reyes |
| Dataset | [Retail Sales Simulated Data (Kaggle - `retail-sales-data-simulated`)](https://www.kaggle.com/datasets/retail-sales-data-simulated) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> Ejecutó descriptivos básicos sobre datos simulados sin cuestionar la distribución artificial de los descuentos y ventas.

**Qué le falta para la banda siguiente:**
> Demostrar comprensión analítica sobre datos reales, justificando el comportamiento de variables no simuladas e interpretando la asimetría y el IQR.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Migrar a un dataset real (ej. Online Retail II de UCI o comercio en datos.gov.co) y argumentar la distribución de datos e IQR. | 2026-10-08 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> Se registró que durante la sustentación en vivo el estudiante se limitó a leer la presentación diapositiva por diapositiva, sin transmitir apropiación del proyecto ni dominio de los conceptos estadísticos y analíticos del curso. Omitió las 3 preguntas de investigación en la portada del notebook. Notebook escueto de 10 celdas, aunque entregó reporte complementario en Word (`Proyecto_Final_Reporte.docx`).

**Qué le falta para la banda siguiente:**
> Formular al menos 3 preguntas de investigación claras en la portada del notebook en estructura Markdown y alinearlas con la toma de decisiones comerciales.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Definir las 3 preguntas de negocio en la portada del notebook en estructura Markdown. | 2026-10-08 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   | X |   |   |   |

**Evidencia que sostiene esta banda:**
> BANDERA ROJA: DATASET SINTÉTICO, SIMULADO O GENERADO PRESENTADO COMO REAL (`retail-sales-data-simulated`). Celdas de código condensadas (5 celdas de código de 10 celdas totales).

**Qué le falta para la banda siguiente:**
> Sustituir el dataset por un conjunto de datos real de transacciones comerciales y desarrollar un notebook completo con estructura analítica en Markdown.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Reemplazar el dataset simulado por uno real de transacciones comerciales (ej. Online Retail II de UCI o datos.gov.co). | 2026-10-08 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Insuficiente |
| Ser | Insuficiente |
| Hacer | Insuficiente |

**Dónde está el equipo, en una frase:**

> Entrega afectada por banderas rojas de dataset sintético/simulado y ausencia de preguntas de investigación en el notebook.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[X] El equipo queda citado a horario de atención dentro de la semana siguiente.** (Citación obligatoria para reorientar proyecto sobre datos reales). Fecha: 2026-10-07 16:00

---

## Lo que hicieron bien

1. Entrega complementaria de reporte en Word (`Proyecto_Final_Reporte.docx`).
2. Inclusión de archivo `.xlsx` de datos en la carpeta del repositorio.
3. Ejecución limpia de las celdas de código presentadas.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Dataset sintético, simulado o generado presentado como real (`retail-sales-data-simulated`) | Hacer | Hacer en Insuficiente o inferior |
| Menos de 3 preguntas de investigación en el notebook | Ser | Ser en Insuficiente |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Declaraste en la URL que tu dataset proviene de Kaggle `retail-sales-data-simulated`. Dado que los datos fueron simulados con distribuciones matemáticas aleatorias, ¿qué limitaciones impone esto al intentar extraer patrones de comportamiento de clientes reales?
2. **Pregunta:** Al revisar la columna de descuentos, aparecen decimales flotantes como `0.289875`. En una tienda retail real, los descuentos se manejan en porcentajes comerciales fijos (ej. 10%, 20%). ¿Cómo afecta esa variabilidad artificial tus agrupaciones de ventas?
3. **Pregunta:** Tu notebook omitió las 3 preguntas de investigación en la portada. Si tuvieras que presentarle este informe al Gerente Comercial, ¿cuáles son las 3 preguntas de negocio central que responderías con tus agrupaciones?

---

## Recomendaciones clave para llevar al Momento 2

- **Migración Obligatoria a Dataset Real:** Reemplazar el archivo simulado por un dataset de transacciones comerciales reales (ej. *Online Retail II* de UCI o comercio en `datos.gov.co`) para remover la bandera roja en el Momento 2.
- **Estructura en Markdown:** Incluir las 3 preguntas de investigación en la portada del notebook e interpretar la asimetría y el IQR de las ventas.
- **Variables prometedoras para filtros del dashboard:** `Categoría_Producto`, `Región`, `Canal_Venta`, `Cliente_ID`.
- **Variables prometedoras para KPIs:** Ventas Totales Reales, Margen de Ganancia Promedio, Transacciones por Cliente, Descuento Comercial Promedio.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: Yovanny Lozano Reyes -->

---

<!-- INICIO ACTA EQUIPO: andersson - angela aguilera -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Andersson, Ángela Aguilera |
| Integrantes | Andersson, Ángela Aguilera |
| Dataset | [Tarjetas de Crédito y Débito en Colombia (Superfinanciera / datos.gov.co)](https://www.datos.gov.co/Econom-a-y-Finanzas/Tarjetas-de-cr-dito-y-d-bito/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Justificación brillante sobre el comportamiento de tarjetas bloqueadas vs. vigentes. Comprenden la auditoría de origen: el dataset viene limpio porque es un reporte financiero regulado por la Superintendencia Financiera de Colombia (SFC), normado y auditado previamente por circulares financieras obligatorias antes de remitirse a datos.gov.co.

**Qué le falta para la banda siguiente:**
> Mantener la solvencia estadística en el diseño de modelos predictivos o analíticos para M2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular ratios de morosidad/bloqueo por entidad en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Responden minuciosamente las 6 preguntas de investigación formuladas. Dominan el sentido de negocio financiero (cuotas de manejo, interchange fee cobrado a comercios e intereses diferidos) y evalúan cómo el volumen y número de tarjetas activas determina si es rentable para un competidor ingresar al mercado de medios de pago.

**Qué le falta para la banda siguiente:**
> Proyectar el impacto de sus hallazgos en la toma de decisiones de riesgo de crédito y estrategia de mercado.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Diseñar propuesta de tablero interactivo en Streamlit con simulador financiero. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Notebook extraordinario de 81 celdas. Análisis temporal, univariado (hist + boxplots), bivariado con matriz de correlación y heatmap, más agregaciones detalladas por entidad financiera. Delimitan rigurosamente los canales, separando transacciones con tarjeta frente a transferencias electrónicas interbancarias (ACH, PSE).

**Qué le falta para la banda siguiente:**
> Mantener la pulcritud y reproducibilidad del código.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Empaquetar el pipeline de datos en un módulo `.py` reutilizable separando canales. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Trabajo verdaderamente impecable de 81 celdas con profundización en series temporales, comparaciones por entidad bancaria, claridad en la regulación SFC y dominio del modelo financiero de medios de pago.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Estructura de notebook ejemplar de 81 celdas con ejecución limpia sin errores.
2. Análisis detallado de 6 preguntas de investigación que abarcan tipología de cliente (natural vs jurídica) y estado de tarjeta.
3. Visualizaciones bivariadas y temporales de alta calidad técnica sobre la banca colombiana.
4. **Auditoría de Origen:** Comprensión clara de la regulación de la Superintendencia Financiera de Colombia (SFC) que garantiza la calidad de captura de datos antes de datos.gov.co.
5. **Alcance de Canales:** Delimitación técnica entre las operaciones con tarjeta y transferencias electrónicas (ACH, PSE).
6. **Modelo Financiero:** Identificación precisa de las fuentes de monetización bancaria (cuotas de manejo, *interchange fee* e intereses diferidos) y barreras por masa crítica de tarjetas activas.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta (Auditoría de Origen SFC):** El dataset venía prácticamente limpio de origen. ¿Qué concluye el equipo sobre esto y cuál fue la razón? (Al ser un reporte regulado de la Superintendencia Financiera de Colombia - SFC, la captura bancaria está normada y auditada previamente por circulares financieras antes de llegar a datos.gov.co).
2. **Pregunta (Definición de Canales):** Discutir el alcance de los tipos de transacciones: ¿El dataset incluye transferencias? ¿Tienen sentido las transferencias dentro de un análisis exclusivo de tarjetas de débito/crédito o corresponden a canales bancarios distintos (ACH, PSE)?
3. **Pregunta (Modelo Financiero y Mercado):** Si una entidad financiera evaluara ingresar al mercado de medios de pago, ¿cómo el volumen y número de tarjetas activas en el mercado determina si es rentable invertir o entrar a competir? ¿Cuál es el modelo de negocio real detrás de las tarjetas (cuotas de manejo, comisiones de intercambio/interchange fee a comercios, intereses por diferidos)?
4. **Pregunta:** Al comparar tarjetas débito vigentes entre personas naturales y jurídicas, ¿qué estadístico de dispersión les permitió evidenciar la concentración de plásticos corporativos?
5. **Pregunta:** En su matriz de correlación identificaron una relación fuerte entre tarjetas bloqueadas y canceladas. ¿Responde este patrón a cierres de año o saneamiento de cartera?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir / Ajustar antes del Momento 2:** Explicar explícitamente en el pipeline la procedencia regulada SFC y aislar las transferencias electrónicas (ACH/PSE) del análisis de tarjetas débito/crédito.
- **Preguntas de investigación que hay que profundizar:** Evaluar cómo el parque de tarjetas activas condiciona la rentabilidad y punto de equilibrio operacional.
- **Variables prometedoras para filtros del dashboard:** `Entidad_Financiera`, `Tipo_Tarjeta`, `Tipo_Persona`, `Periodo`.
- **Variables prometedoras para KPIs:** Total Tarjetas Vigentes/Activas, Ratio de Cancelación, Volumen de Tarjetas Bloqueadas, Estimación de Ingresos por *Interchange Fee* y Cuotas de Manejo.

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: andersson - angela aguilera -->

---

<!-- INICIO ACTA EQUIPO: jean Cardenas - carlos grueso -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Carlos Grueso, Jean Cárdenas, Carlos Cifuentes |
| Integrantes | Carlos Grueso, Jean Cárdenas, Carlos Cifuentes |
| Dataset | [Producción de Frutales en el Valle del Cauca (MinAgricultura / datos.gov.co 2000-2022)](https://www.datos.gov.co/Agricultura-y-Desarrollo-Rural/Producci-n-de-frutales-Valle-del-Cauca/) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Demuestran que la producción total pasó de 410.278 a 965.498 toneladas. Explican la necesidad de usar medianas debido a la concentración masiva en polos agrarios (cítricos/chontaduro).

**Qué le falta para la banda siguiente:**
> Mantener el rigor en la selección de métricas robustas frente a distribuciones agrarias sesgadas.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Incorporar tasas de rendimiento (ton/ha) en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Responden con precisión las 5 preguntas de investigación. Insights agrícolas de alto valor para la Secretaría de Agricultura; reconocen limitaciones por datos antiguos. Traen PDF de soporte.

**Qué le falta para la banda siguiente:**
> Proyectar el análisis hacia la focalización de subsidios agrícolas.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Diseñar maqueta de dashboard de producción en Streamlit. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Notebook de 91 celdas con documentación excepcional en markdown celda por celda. Depuración justificada (eliminación de 39 duplicados exactos y conversión de texto con puntos de miles/comas decimales a flotante). Uso impecable de la transformación logarítmica (`log10`) para visualizar la distribución asimétrica y comparar municipios/cultivos. Histogramas, boxplots, matriz de correlación con heatmap y comparaciones por ciclo (permanente vs transitorio).

**Qué le falta para la banda siguiente:**
> Mantener la calidad y reproducibilidad del notebook.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Estructurar filtros geográficos para la app de M2. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Trabajo sobresaliente / muy buen trabajo. EDA agrícola brillante de 91 celdas con documentación exhaustiva celda por celda, limpieza justificada (39 duplicados exactos y conversión de miles/decimales a flotante), uso impecable de `log10`, excelente análisis univariado y bivariado, y soporte en diapositivas.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Documentación expositiva en markdown celda por celda que explica cada decisión de transformación.
2. Análisis bivariado completo discriminando ciclos agrícolas (anual vs semestral) y subregiones del Valle.
3. Presentación complementaria de 10 diapositivas en PDF (`Presentacion_EDA_Frutales_Resumen_10_diapositivas.pdf`).
4. **Limpieza y depuración justificada:** Claridad absoluta en la razón de por qué borraron datos (eliminación de 39 duplicados exactos) y por qué realizaron la limpieza (conversión de texto con puntos de miles/comas decimales a flotante).
5. **Uso excelente de la función logarítmica:** Uso impecable de la escala/transformación logarítmica (`log10`) para visualizar la distribución asimétrica y hacer las gráficas comparables entre municipios y cultivos.
6. **Calidad del análisis:** Excelente análisis univariado y riguroso análisis bivariado (Trabajo sobresaliente / muy buen trabajo).

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Al analizar la concentración municipal observaron que 3 municipios concentran más del 50% de la producción de frutales. ¿Cómo afectó esto a la media y por qué la mediana refleja mejor al municipio típico?
2. **Pregunta:** En su desglose bivariado compararon cultivos de ciclo permanente frente a transitorios. ¿Qué diferencia sustancial observaron en la correlación entre área cosechada y tonelaje?

---

## Recomendaciones clave para llevar al Momento 2

- **Corregir antes del Momento 2:** Estandarizar las unidades de rendimiento (toneladas por hectárea cosechada).
- **Preguntas de investigación que hay que profundizar:** P5 sobre cultivos ganadores y perdedores de producción entre 2000 y 2022.
- **Variables prometedoras para filtros del dashboard:** `Cultivo`, `Subregión`, `Municipio`, `Ciclo_Cultivo`.
- **Variables prometedoras para KPIs:** Producción Total (Toneladas), Área Cosechada Total (Hectáreas), Rendimiento Promedio (Ton/Ha).

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: jean Cardenas - carlos grueso -->

---

<!-- INICIO ACTA EQUIPO: johan fernando sanches -->

# Acta de retroalimentación — Momento 1: EDA completo

Curso 709749 · Analítica de Datos · **Momento formativo: produce retroalimentación, no nota**  
Rúbrica completa: `evaluaciones/momento1/rubrica.md`

| Campo | Valor |
|-------|-------|
| Equipo | Johan Fernando Sánchez |
| Integrantes | Johan Fernando Sánchez |
| Dataset | [California Housing Census Data (Kaggle / StatLib)](https://www.kaggle.com/datasets/camnugent/california-housing-prices) |
| Fecha de sustentación | Octubre 2026 |
| Evaluador | Profesor de Analítica de Datos |

---

## Por qué este documento no trae un número

**Porque no hay ninguno.** El Momento 1 no produce nota: ni ese día, ni después, ni "por dentro". No se está reteniendo un número hasta la sesión de cierre ni queda guardado en la hoja del profesor. Si la pregunta es "¿cuánto me habría dado?", la respuesta honesta es que no existe tal número.

Lo que sí hay es esto: **la banda de cada una de las tres dimensiones, qué le falta para la de arriba, y una acción concreta por dimensión.** Un número le diría dónde quedó; una banda le dice qué hacer.

**La única nota del semestre es la del Momento 3**, y ahí la cuenta es `(Saber + Ser + Hacer) / 3`. Nada más. Con las bandas de abajo usted ya sabe exactamente contra qué va a jugar en el Momento 3.

Este acta produce además un **cumplido / no cumplido**, que está más abajo. El cumplido habilita el Momento 3.

---

## Dimensión SABER

*Distingue técnicas para la ubicuidad de la información.* Conocimiento conceptual: elegir la medida estadística correcta antes de calcularla y leerla bien después.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> Imputación condicional de `total_bedrooms` por `ocean_proximity`, justificación estadística de sesgo e IQR, dominio de correlaciones de Pearson y paradoja de Simpson.

**Qué le falta para la banda siguiente:**
> Mantener la profundización teórica en el modelado predictivo del Momento 2.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Formular modelo deductivo multivariado en M2. | 2026-10-15 |

---

## Dimensión SER

*Asocia técnicas y procedimientos de Minería de Datos.* Juicio valorativo, insights, responsabilidad y trabajo en equipo: qué se afirma, con qué respaldo, a quién le sirve y qué se reconoce como límite.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> 5 preguntas de investigación claras, estructura narrativa fluida, excelente contextualización del censo y economía urbana de California. Responde rigurosamente y propone decisores.

**Qué le falta para la banda siguiente:**
> Diseñar la estructura de toma de decisiones para planeación urbana.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Crear propuesta de simulador de precios en Streamlit. | 2026-10-22 |

---

## Dimensión HACER

*Aplica técnicas de minería de datos para solucionar problemas.* Desempeño técnico sobre datos reales y sucios: preparación de datos, análisis univariado, análisis bivariado y multivariado, calidad del código y reproducibilidad.

**Banda obtenida:**

| No aceptable | Insuficiente | Aceptable | Bueno | Excelente |
|:------------:|:------------:|:---------:|:-----:|:---------:|
|   |   |   |   | X |

**Evidencia que sostiene esta banda:**
> NOTEBOOK EXTRAORDINARIO DE 93 CELDAS. Univariado con KDE y boxplots, mapa scatter geográfico de latitud/longitud vs. precio, matriz de correlación completa y heatmap, ingeniería de variables (`cuartos_por_hogar`, `poblacion_por_hogar`) y tratamiento del tope en $500k.

**Qué le falta para la banda siguiente:**
> Mantener la calidad impecable del código.

**Su acción para el Momento 2:**

| Acción | Fecha |
|--------|-------|
| Exportar el pipeline transformador de variables a un script reutilizable. | 2026-10-22 |

---

## Lectura de conjunto

| Dimensión | Banda |
|-----------|-------|
| Saber | Excelente |
| Ser | Excelente |
| Hacer | Excelente |

**Dónde está el equipo, en una frase:**

> Notebook extraordinario de 93 celdas con imputación condicional geográfica por proximidad al océano, mapa scatter de precios, 5 preguntas de investigación y verificación de la Paradoja de Simpson.

> **Esta banda no es tu nota, pero es exactamente la banda que sí va a ser tu nota si llegas igual al Momento 3.**

---

## Cumplido / No cumplido

**[X] Cumplido   [ ] No cumplido**

> **Cumplido** = el equipo entregó y sustentó, y ninguna dimensión quedó en banda **No aceptable**.  
> **El cumplido habilita el Momento 3.** Un no cumplido inhabilita al equipo para sustentar el Momento 3.

---

## Alerta temprana

**[ ] El equipo NO requiere citación a alerta temprana.**

---

## Lo que hicieron bien

1. Imputación condicional de `total_bedrooms` por `ocean_proximity` e ingeniería de atributos pasando de datos censales agregados a promedios por hogar (`cuartos_por_hogar`, `poblacion_por_hogar`).
2. 5 preguntas de investigación claras con estructura narrativa fluida y contextualización rigurosa del censo de vivienda.
3. Análisis univariado completo con KDE y boxplots, mapa scatter geográfico (latitud/longitud vs. precio) y matriz de correlación completa ($r=0.688$ para `median_income`).
4. Verificación empírica avanzada de la Paradoja de Simpson y tratamiento riguroso de la censura de datos en el tope de $500.001 USD.

---

## Banderas rojas y topes por omisión aplicados

| Regla aplicada | Dimensión afectada | Efecto sobre la banda |
|----------------|--------------------|-----------------------|
| Ninguna aplicada | N/A | Sin efecto |

---

## Q&A / Puntos a responder en sustentación

1. **Pregunta:** Imputaste los nulos de `total_bedrooms` agrupando por la proximidad al océano (`ocean_proximity`) en vez de usar la mediana global. ¿Por qué ese criterio geográfico produce un mejor llenado de datos y cómo cambió la distribución final frente a una imputación simple?
2. **Pregunta:** Al analizar la distribución del valor de la vivienda (`median_house_value`), aparece una acumulación artificial muy alta exactamente en $500.001 USD. ¿A qué se debe ese 'techo o truncamiento de datos' en el censo y cómo impacta la correlación con el ingreso mediano?
3. **Pregunta:** Graficaste la latitud y longitud con el precio de la propiedad. ¿Por qué la distancia a la costa y la cercanía a las áreas metropolitanas (San Francisco/Los Ángeles) muestran una relación no lineal tan fuerte con el precio, superando al número de habitaciones o antigüedad?
4. **Pregunta:** Tu matriz de correlación identificó que `median_income` es la variable con mayor correlación con el precio ($r=0.688$). ¿Por qué el ingreso medio de los residentes es un indicador más confiable de valorización que la densidad poblacional?

---

## Recomendaciones clave para llevar al Momento 2

- **Tratamiento del Tope Censurado ($500k):** Señalar explícitamente las viviendas con el tope censurado de $500.001 USD en el dashboard para evitar sesgos en el análisis de valorización.
- **Feature Engineering:** Construir ratios como `cuartos_por_hogar` (`total_rooms / households`) y `poblacion_por_hogar`, los cuales tienen mayor poder explicativo que las variables agregadas por bloque censal.
- **Corregir antes del Momento 2:** Mantener las características transformadas (`cuartos_por_hogar`, `poblacion_por_hogar`) para los modelos de regresión.
- **Variables prometedoras para filtros del dashboard:** `ocean_proximity`, `Quintil_Ingreso`, `Edad_Vivienda_Grupo`.
- **Variables prometedoras para KPIs:** Valor Mediano de la Vivienda, Ingreso Mediano por Distrito, Densidad Poblacional por Hogar (`poblacion_por_hogar`), Ratio Cuartos por Hogar (`cuartos_por_hogar`).

---

## Apelación

Tiene **5 días hábiles** desde que recibió este documento para pedir reevaluación por escrito exponiendo la dimensión específica que apela y discutiendo la evidencia utilizada.


<!-- FIN ACTA EQUIPO: johan fernando sanches -->

---
