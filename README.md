# Optimización de Operaciones y Forecasting en Plantas de Energía Solar

----

## 1. Impacto de Negocio & Contexto
Las plantas de energía solar fotovoltaica operan en un entorno altamente variable dependiente de factores climáticos (radiación, nubosidad, temperatura). 
* **El Problema:** El operador del sistema eléctrico exige estimaciones precisas de la energía que se inyectará a la red al día siguiente. Las desviaciones (generar de más o de menos) se traducen en **penalizaciones financieras** significativas y fallas de eficiencia operativa.
* **El Objetivo:** Desarrollar un pipeline de análisis de datos para identificar anomalías en los inversores de la planta, entender los factores físicos de eficiencia y construir un modelo analítico base (*Baseline*) para predecir la generación de potencia AC.

##  2. Stack Tecnológico
* **Lenguaje:** Python 3.10
* **Entorno de Desarrollo:** VS Code / Jupyter Notebooks
* **Librerías Clave:** * Manipulación de datos: `Pandas`, `NumPy`
  * Visualización: `Matplotlib`, `Seaborn`, `Plotly`
  * Modelamiento: `Scikit-Learn`
* **Metodología de Desarrollo:** Modular (Estructura de código reproducible con `/notebooks` y `/src`).

## 3. Metodologia y ciclo del proyecto
Paso 1: Ingesta y Limpieza de Datos (`1_data_cleaning.ipynb`)
* Se estandarizaron los registros temporales de la Planta 2 transformando la variable `DATE_TIME` al formato nativo de series de tiempo (`datetime64`).
* Se verificó la integridad de los datos eliminando registros duplicados y aplicando técnicas de interpolación para mitigar la pérdida de lecturas de los sensores climáticos.
* Se consolidaron las métricas de inversores y telemetría ambiental mediante un proceso de *Merge* estructurado, generando un dataset unificado listo para la fase exploratoria.
---
datos de keggle  "anikannal/solar-power-generation-data"