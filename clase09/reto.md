# Clase 9 · Reto — Data storytelling: 4 slides y pitch de 3 minutos

## De qué se trata

En la primera parte de la clase vimos cómo un análisis con datos rigurosos fracasa si la audiencia
no entiende qué hacer con él. Modelamos la estructura de cuatro diapositivas con el caso del
presupuesto nacional y comprobamos cómo cambia la historia cuando se pasa del anecdotario del analista
a la decisión que necesita la organización.

En este reto aplicas el marco completo: preparas durante **1 hora cronometrada** en el taller tu **mini-deck de exactamente 4 slides**
sobre tema libre y lo sustentas en un **pitch de 3 minutos** frente a la sala plenaria (con aviso a los 2 minutos y corte duro a los 3 minutos), recibiendo retroalimentación estructurada (*I like, I wish, What if*).

| Campo | Valor |
|-------|-------|
| Consigna | **Tema libre:** el proyecto de semestre de tu equipo o cualquier fenómeno con datos cuantitativos (movilidad, gaming, música, deportes, finanzas, salud) |
| Tiempo en sala | **1 hora (60 min)** de preparación y ensayo interno (Bloque 2) + **pitches de 3 min** en sala plenaria (Bloque 3) |
| Entregable | Mini-deck de **exactamente 4 slides** (*Contexto → Hallazgo → Implicación → Acción*) sin código en pantalla |
| Formato | **Libre:** Canva, Google Slides, PowerPoint, HTML o PDF exportado |
| Sustentación | Pitch de **3 minutos con corte duro** a los 180 segundos (tarjeta amarilla a los 2 min / 120s, tarjeta roja a los 3 min) + coevaluación y feedback |
| Evaluación | Formativa, basada en las tres dimensiones institucionales (**Saber, Ser y Hacer**) |

Este ejercicio es el ensayo general directo de la sustentación del **Momento 2 (clase 11)**.

---

## 1. La consigna: tema libre con evidencia cuantitativa

El objetivo del reto no es evaluar la sintaxis de Python, sino entrenar la musculatura narrativa y la
capacidad de síntesis del analista de datos.

Puedes elegir entre dos opciones:

1. **El dataset de tu equipo (proyecto de semestre):** si ya tienes avanzado el EDA del Momento 1,
   este es el espacio para destilar tus hallazgos preliminares y probar tu narrativa antes
   de la sustentación formal.
2. **Cualquier fenómeno con datos que te apasione:** movilidad urbana, consumo en plataformas de
   streaming musical (Spotify), hábitos de compra y abandono en gaming (Steam), rendimiento deportivo
   (fútbol), accidentalidad vial o transporte público urbano.

> [!IMPORTANT]
> **La única condición sobre el tema:** debe fundamentarse en cifras cuantitativas con contraste
> claro. No presentes intuiciones abstractas: presenta la cifra que inclina la balanza de una decisión.

---

## 2. El entregable: exactamente 4 slides sin código en pantalla

La estructura del mini-deck es estricta e innegociable. Cuatro diapositivas. Ni tres ni cinco.

| # | Slide | La pregunta que responde | Señal de alarma si está mal |
|---|-------|--------------------------|-----------------------------|
| 1 | **Contexto** | ¿De qué estamos hablando, cuál era la promesa y por qué importa hoy? | Si parece la agenda de la reunión o la historia de la empresa desde 1995, está mal. |
| 2 | **Hallazgo** | ¿Qué encontramos que rompe la intuición? (Con cifra y contraste) | Si amontonas tres hallazgos o pones una tabla de 20 filas, está mal. |
| 3 | **Implicación** | ¿Y eso qué significa para el negocio? ¿A quién le duele? | Si repite el hallazgo con otras palabras, está mal. |
| 4 | **Acción** | ¿Qué decisión concreta se debe tomar, quién la ejecuta y para cuándo? | Si concluye con "se recomienda seguir investigando o concientizar", está mal. |

### Reglas del diseño de diapositivas

- **Cero código en pantalla:** La sala no vino a ver cómo importaste `pandas` ni cuántas líneas
  te tomó limpiar el CSV. La audiencia valora las conclusiones, el contraste de magnitudes y la
  decisión operativa.
- **El título es el mensaje (La prueba de tapar la pantalla):** Los títulos no son etiquetas de
  archivo (`"Análisis de ventas"`, `"Gráfico 2"`, `"Resultados"`). Son oraciones completas con verbo
  activo y cifra: *"El 12% de los usuarios consume la mitad del agua potable"* o *"Los motociclistas
  concentran el 62% de las muertes en solo 5 corredores"*. Si alguien lee solo los 4 títulos de
  corrido, ya entendió la historia completa.
- **Gráficos con alto data-ink:** Cada gráfico o número destacado existe para respaldar una sola
  afirmación. Elimina fondos oscuros pesados, leyendas redundantes y cuadrículas innecesarias.
- **La slide de acción nombra doliente, acción y plazo:** Debe responder con precisión **quién**
  firma la orden, **qué** hace el lunes a primera hora y **cuándo** se revisa el impacto.

### Formato libre

Usa la herramienta que tu equipo domine con mayor agilidad:
- **Canva**
- **Google Slides**
- **PowerPoint** o **Keynote**
- **HTML** o **PDF exportado**

> [!TIP]
> **Regla de taller:** El tiempo que inviertes escogiendo tipografías o animaciones 3D es tiempo
> que le quitas a afilar tus títulos y tu recomendación. Lo que se juzga es la fuerza del argumento,
> no la plantilla.

---

## 3. El bucle de trabajo: especificar antes de diseñar

Antes de abrir cualquier editor de diapositivas, resuelve en borrador (en papel o editor de notas)
las tres preguntas del **Paso 0.5**:

```
┌────────────────────────────────────────────────────────────────────────┐
│                   PASO 0.5: ESPECIFICAR EN PAPEL                       │
├────────────────────────────────────────────────────────────────────────┤
│ 1. ¿A quién le hablo? (Audiencia única: directivo, gerente o técnico)  │
│ 2. ¿Qué decisión concreta quiero que tomen el lunes?                   │
│ 3. ¿Cuál es el único número que vuelve inevitable esa decisión?        │
└────────────────────────────────────────────────────────────────────────┘
```

Si no hay acuerdo en el equipo sobre la audiencia y la decisión, cualquier diapositiva que dibujen
saldrá desenfocada.

### La prueba del intercambio

Una vez escritos los borradores de tus 4 títulos, haz la prueba ácida: **intercambia de lugar la
Slide 2 (Hallazgo) y la Slide 3 (Implicación)**. Si la presentación se puede leer en ese orden
alterado y sigue funcionando igual, no tienes una historia: tienes una lista de mercado. La
implicación debe ser una consecuencia inevitable del hallazgo, no un sinónimo.

---

## 4. El pitch plenario de 3 minutos

Todos los equipos presentan su trabajo en sesión plenaria frente a la sala completa.

### Las cuatro reglas de oro

1. **Corte duro a los 3 minutos (180 segundos):**
   - Dispones de 3 minutos netos de exposición (180 segundos).
   - Al minuto **2:00 (120 segundos):** Se levanta la **tarjeta amarilla** (aviso de 1 minuto restante). Debes estar cerrando la implicación y entrando de inmediato a la Slide 4 de acción.
   - Al minuto **3:00 (180 segundos):** Se levanta la **tarjeta roja** y se corta la exposición en seco. Lo que no cupo en 3 minutos, no existió.
2. **Prohibido leer las diapositivas:**
   - La diapositiva es para que el público verifique las cifras; tú miras a los ojos a la persona
     que toma la decisión. Si le das la espalda a la sala para leer la pantalla, pierdes la atención.
3. **Ritmo sostenido y distribución del tiempo:**
   - No gastes minuto y medio en el contexto. El reparto recomendado es:
     - *Slide 1 · Contexto:* ~35 - 40 segundos.
     - *Slide 2 · Hallazgo:* ~50 - 55 segundos.
     - *Slide 3 · Implicación:* ~50 - 55 segundos.
     - *Slide 4 · Acción:* ~35 - 40 segundos.
4. **Remate en la acción:**
   - Tu última frase debe ser la decisión propuesta (*"Por eso, el lunes la Secretaría debe..."*).
     Prohibido cerrar con dudas, disculpas por los datos o un simple *"eso era todo, ¿preguntas?"*.

---

## 5. Protocolo de retroalimentación: I like, I wish, What if

Inmediatamente después de cada pitch de 3 minutos, se abre el espacio de feedback estructurado y coevaluación (~1.5 - 2 minutos):
- **45 segundos:** Un compañero par asignado entrega su evaluación oral según el marco (*I like / I wish / What if*).
- **45 segundos:** El profesor aporta un apunte quirúrgico sobre la causalidad narrativa, el foco visual (data-ink) o la precisión de la acción.
- El resto del salón registra sus comentarios en el formulario de coevaluación.

El feedback oral y escrito se entrega estrictamente en este formato de tres frases:

- **I like... (Lo que funcionó):** Concreto y respaldado en hechos observables.
  *Ejemplo:* *"Me gustó el contraste entre la promesa de 100 millones de canciones y la cifra de que el 78% tiene menos de 50 reproducciones."*
- **I wish... (Lo que faltó):** Enfocado en el trabajo y la narrativa, nunca en la persona.
  *Ejemplo:* *"Me hizo falta que la slide 3 explicara qué le pasa a los músicos locales en lugar de repetir el número de reproducciones."*
- **What if... (Una propuesta constructiva):** Una alternativa accionable para mejorar.
  *Ejemplo:* *"¿Qué pasaría si en la slide 4 asignan la responsabilidad al Director de Producto en vez de decir de forma abstracta 'se recomienda a la plataforma'?"*

> [!WARNING]
> **El que presenta no se defiende: solo escucha y anota.** Discutir o justificar consume el tiempo
> del siguiente equipo y no cambia lo que la sala entendió. Si la audiencia no lo captó en 3 minutos,
> el ajuste debe hacerse en el artefacto, no en el debate.

---

## 6. Cómo se ve un buen trabajo (Rúbrica formativa: Saber, Ser y Hacer)

La retroalimentación se estructura en las tres dimensiones institucionales de la universidad:
**Saber, Ser y Hacer**.

| Dimensión | Qué se mira en el pitch | Se cumple cuando |
|-----------|-------------------------|------------------|
| **Saber** | *Evidencia y contraste* | Las cifras sostienen con rigor el mensaje, tienen contraste numérico claro y no hay código ni tecnicismos innecesarios en pantalla. |
| **Ser** | *Presencia y escucha* | Sostiene el pitch sin leer las slides, remata con la acción concreta y recibe el feedback anotando sin ponerse a la defensiva. |
| **Hacer** | *Estructura y tiempo* | Cumple la secuencia de 4 slides (*Contexto → Hallazgo → Implicación → Acción*) y clava el pitch dentro de los 3 minutos (180 s) sin corte de micrófono. |

---

## 7. Qué hacer en casa

El reto de clase instala el hábito de la síntesis bajo presión. En casa se consolida el trabajo:

- [ ] **Incorporar el feedback:** Ajustar los títulos y gráficos atendiendo al menos dos de los comentarios (*I wish* / *What if*) recibidos en sala.
- [ ] **Ensayar con cronómetro:** Practicar la exposición oral en voz alta midiendo exactamente los 3 minutos (con aviso a los 2 minutos). El ensayo mental oculta tropiezos y exceso de tiempo.
- [ ] **Alinear con el Momento 2:** Si usaste el dataset de tu equipo, este mini-deck es el núcleo conceptual de tu sustentación para la Clase 11.

---

## Este reto no tiene nota numérica

Como todos los retos semanales del curso, esta actividad es **formativa**. No produce nota
cuantitativa. Su propósito es permitirte experimentar el rigor del corte duro y pulir tu capacidad
comunicativa en un entorno seguro antes de la sustentación formal del **Momento 2 (clase 11)**,
donde el turno será de 10 minutos (7 de exposición con corte duro, 2 de preguntas y 1 de transición).
