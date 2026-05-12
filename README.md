# Análisis de Comportamiento y Bienestar en Redes Sociales 📱🧠

Este repositorio contiene el avance del proyecto de Analítica de Datos, enfocado en investigar la relación entre los hábitos de consumo digital y el bienestar emocional. Actualmente incluye la **Evidencia de Aprendizaje 2: Limpieza y Transformación de Datos**.

## 📋 Descripción del Proyecto

El proyecto aborda la problemática de la falta de mecanismos de detección temprana sobre el impacto negativo que los hábitos de navegación (tiempo de uso, horarios y velocidad de interacción) tienen sobre la salud mental y la higiene del sueño.

### 🔍 Pregunta de Investigación
> ¿En qué medida las variables de comportamiento digital influyen en la probabilidad de que un usuario reporte un puntaje de salud mental inferior a 5.0 y presente niveles moderados o severos de interrupción del sueño?

---

## 🛠️ Fase actual: Limpieza y Transformación (EA2)

En esta etapa se procesó el dataset original para asegurar la calidad de la información. Los pasos técnicos realizados fueron:

1. **Ajuste de Tipos de Datos:** Conversión de fechas a `datetime64` y variables de texto a `category` para optimizar memoria.
2. **Tratamiento de Outliers:** Aplicación de **Winsorización** en la duración de sesiones, topando los valores extremos en 111.54 minutos para evitar sesgos en los promedios.
3. **Estandarización:** Creación de la variable `mood_category` simplificando los estados de ánimo en categorías de sentimiento (**Positivo, Neutral y Negativo**).
4. **Cambio de Granularidad:** Agregación de datos por plataforma y sentimiento para obtener una visión estratégica del comportamiento grupal.

---

## 📊 Estructura del Dataset

El análisis utiliza el *Social Media User Behavior Dataset* de Kaggle (2,000 registros).

### Variables Críticas Analizadas:
| Variable | Descripción |
| :--- | :--- |
| `daily_usage_hours` | Horas diarias de uso de redes sociales. |
| `self_reported_mental_health_score` | Puntuación de salud mental (1-10). |
| `avg_session_duration_min` | Duración promedio de cada sesión (Datos Limpios). |
| `mood_category` | Categoría de sentimiento (Positivo, Neutral, Negativo). |

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3.x
- **Librerías:** `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
- **Gestión del Proyecto:** Trello (Metodología Kanban)

---

## 📁 Contenido del Repositorio

- `Arango_Isabela_EA2.pdf`: Informe detallado del proyecto.
- `social_media_user_behavior.csv`: Dataset original utilizado.
- `Arango_Isabela_EA2.ipynb`: Notebook de Jupyter con el código de exploración.
- `exploracion_datos.html`: HTML generado a partir de la exploración de datos con pandas.
- `Arango_Isabela_EA2_Limpio.csv`: Dataset final procesado listo para el análisis estadístico.
- `README.md`: Descripción general del proyecto (este archivo).

---

## 👤 Autora
**Isabela Arango Verona** Proyecto Integrado III - Analítica de Datos  
*Institución Universitaria Digital de Antioquia*
