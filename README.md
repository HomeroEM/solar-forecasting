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

---

## 3. Estructura del Repositorio
```text
proyecto-solar-forecasting/
│
├── data/
│   ├── raw/                # Datos originales sin modificaciones (Sensores e Inversores)
│   └── processed/          # Datos limpios con fechas indexadas y variables imputadas
│
├── notebooks/
│   ├── 1_data_cleaning.ipynb      # Extracción, tratamiento de nulos y tipado
│   ├── 2_exploratory_analysis.ipynb # Análisis de curvas de generación y correlaciones
│   └── 3_forecasting.ipynb        # Modelamiento predictivo y cálculo de errores (MAE)
│
├── src/
│   ├── __init__.py
│   └── utils.py            # Funciones auxiliares reutilizables
│
├── .gitignore              # Control de archivos excluidos de Git
├── README.md               # Documentación principal del proyecto
└── requirements.txt        # Dependencias del entorno
```

---
datos de keggle  "anikannal/solar-power-generation-data"