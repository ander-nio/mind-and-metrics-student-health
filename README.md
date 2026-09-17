# Impacto de los Hábitos Diarios en el Rendimiento Académico y Estrés Estudiantil

# Introducción y Pregunta de Investigación
El rendimiento académico de los estudiantes suele ser el resultado de un equilibrio complejo entre el tiempo dedicado al estudio, el descanso y el bienestar mental. Este proyecto explora la siguiente interrogante:

> **¿Es posible predecir el rendimiento académico (`Grades`) de un estudiante a partir de sus hábitos de estilo de vida y determinar qué factores impactan de forma más significativa?**

Se analizó una muestra de 2,000 registros estudiantiles que evalúan variables como horas de estudio, sueño, actividad física, interacción social, actividades extracurriculares y nivel de estrés.

---

# Análisis Exploratorio y Storytelling
A partir del análisis exploratorio de datos, se identificaron tres hallazgos clave:

1. **Distribución del Sueño y Calificaciones:** La mayoría de los estudiantes mantiene promedios intermedios-altos, con distribuciones de sueño concentradas alrededor de las 6 a 8 horas diarias.
2. **Impacto del Estrés:** Los estudiantes agrupados en niveles de estrés alto presentan una dispersión mayor en sus notas, reflejando cómo la tensión constante afecta la consistencia académica.
3. **Estudio vs. Promedio:** Existe una tendencia positiva clara entre las horas de estudio diarias y la nota obtenida, aunque con retornos decrecientes cuando no se combina con un descanso adecuado.

# Modelo Predictivo e Interpretación
Se entrenó un modelo de **Regresión Lineal Múltiple** utilizando el 80% de los datos para entrenamiento y el 20% para evaluación a ciegas.

# Métricas de Evaluación
* **Coeficiente de Determinación ($R^2$):** `0.5497`
  * *Interpretación:* El modelo logra explicar el **55% de la variabilidad** en las calificaciones académicas basándose únicamente en los hábitos diarios recopilados.
* **Error Cuadrático Medio ($RMSE$):** `0.5128`
  * *Interpretación:* En promedio, las predicciones del modelo se alejan solo **$\pm 0.51$ puntos** de la nota real del estudiante.

# Peso de los Hábitos (Coeficientes)
El modelo permite cuantificar el impacto estimado de cada hora adicional dedicada a las distintas actividades sobre la nota final.

## Aplicación Profesional
Este enfoque demuestra cómo la analítica de datos aplicada a la educación y psicología puede transformar la gestión del bienestar universitario:

* **Sistemas de Alerta Temprana:** Implementar este modelo en plataformas estudiantiles para detectar automáticamente a alumnos con combinaciones de hábitos en riesgo de bajo rendimiento o *burnout*.
* **Intervención Preventiva:** Permitir a los equipos de acompañamiento académico y psicológico ofrecer tutorías o asesorías de manejo del tiempo antes de que el estudiante repruebe o colapse emocionalmente.

---

## Estructura del Repositorio
```text
├── data/                  # Dataset original (.csv)
├── notebooks/             # Cuaderno de Google Colab (.ipynb)
├── src/                   # Scripts modulares de Python (.py)
└── README.md              # Informe principal del proyecto
