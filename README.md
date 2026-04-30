# Análisis de Comportamiento y Bienestar en Redes Sociales 📱🧠

Este repositorio contiene la **Evidencia de Aprendizaje 1** para el proyecto de Analítica de Datos. El objetivo principal es investigar la relación entre los hábitos de consumo en redes sociales y el bienestar emocional de los usuarios mediante el análisis de un dataset sintético de 2,000 registros.

## 📋 Descripción del Proyecto

El proyecto aborda la problemática de la falta de mecanismos de detección temprana sobre el impacto negativo que los hábitos de navegación (tiempo de uso, horarios y velocidad de interacción) tienen sobre la salud mental y la higiene del sueño.

### 🔍 Pregunta de Investigación
> ¿En qué medida las variables de comportamiento digital influyen en la probabilidad de que un usuario reporte un puntaje de salud mental inferior a 5.0 y presente niveles moderados o severos de interrupción del sueño?

---

## 📊 Estructura del Dataset

El análisis se basa en el *Social Media User Behavior Dataset*, el cual cuenta con las siguientes especificaciones:
- **Registros:** 2,000 usuarios únicos.
- **Variables:** 34 (Demográficas, de uso, compromiso, salud mental y comercio).
- **Calidad de datos:** 100% de integridad (sin valores nulos ni duplicados).

### Variables Críticas Analizadas:
| Variable | Descripción |
| :--- | :--- |
| `daily_usage_hours` | Horas diarias de uso de redes sociales. |
| `self_reported_mental_health_score` | Puntuación de salud mental (1-10). |
| `sleep_disruption` | Nivel de afectación en el sueño. |
| `mood_while_scrolling` | Estado emocional predominante. |

---

## 🚀 Hallazgos Principales (Exploración de Datos)

Tras realizar la exploración con `ydata-profiling`, se identificaron los siguientes patrones:

1. **Patrones de Sesión:**
   - Existe una **fuerte correlación positiva (r = 0.785)** entre el uso diario total y la duración de las sesiones individuales.
   - Se identificó una **correlación inversa (r = -0.587)** entre la cantidad de sesiones y su duración, distinguiendo perfiles de "usuarios maratón" frente a "usuarios frecuentes".

2. **Impacto en Salud Mental:**
   - Sorprendentemente, la correlación lineal entre el tiempo de uso y el score de salud mental es casi nula (**0.019**). Esto sugiere que el bienestar depende más de variables cualitativas (cómo se usa la app) que de variables cuantitativas (cuánto tiempo).

3. **Métricas de Éxito:**
   - Se definió el **Puntaje de Alerta de Bienestar (PAB)** para monitorear usuarios con uso >5h y score de salud <5.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3.x
- **Librerías de Análisis:** `Pandas`, `NumPy`
- **Exploración Automática:** `ydata-profiling` (Pandas Profiling)
- **Gestión del Proyecto:** Trello (Metodología Kanban)

---

## 📁 Contenido del Repositorio

- `Arango_Isabela_EA1.pdf`: Informe detallado del proyecto.
- `social_media_user_behavior.csv`: Dataset original utilizado.
- `Analisis_Exploratorio.ipynb`: Notebook de Jupyter con el código de exploración.
- `README.md`: Descripción general del proyecto (este archivo).

---

## 👤 Autora
**Isabela Arango Verona** Proyecto Integrado III - Analítica de Datos  
*Institución Universitaria Digital de Antioquia*
