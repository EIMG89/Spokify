# 🎵 Spokify: Data Preparation & Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/status-completed-success)

## 📌 Contexto del Negocio
**Spokify**, un líder emergente en streaming musical, enfrenta una crisis silenciosa: un aumento alarmante en su tasa de cancelación (*Churn Rate*) durante el último trimestre. 

Este proyecto aborda la fase crítica de **Preparación de Datos y Análisis Exploratorio (EDA)** para descifrar patrones de fuga. El objetivo principal es estructurar y limpiar los datos para habilitar modelos predictivos robustos que permitan estrategias de fidelización proactivas.

## 📊 Hallazgos Clave (Insights)
1. **Desbalanceo Crítico:** La gran mayoría de los usuarios no cancelan (Clase 0), lo que requerirá técnicas como **SMOTE** o ajustes de pesos (class_weights) en la fase de Machine Learning para evitar sesgos algorítmicos.
2. **El "Falso Negativo" de los Podcasts:** El porcentaje exacto de consumo de podcasts tiene una correlación cercana a cero con el *churn*. Sin embargo, el simple acto de escucharlos es determinante.
3. **Feature Engineering:** A partir del hallazgo anterior, se diseñó una variable binaria (`Escucha_Podcasts`) que proporciona una señal algorítmica mucho más limpia para futuros modelos.

## 🛠️ Stack Tecnológico
* **Procesamiento y Transformación:** Python, NumPy, Pandas (uso avanzado de `pd.merge()`, `df.groupby()`, `np.where()`).
* **Visualización:** Seaborn (`sns.histplot`, `sns.boxplot`, `sns.heatmap`), Matplotlib.
* **Presentación Ejecutiva:** Disponible en el directorio `/presentations` para comunicación con *stakeholders* no técnicos.

## 🚀 Cómo ejecutar este proyecto

1. Clona el repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/spokify-churn-eda.git](https://github.com/tu-usuario/spokify-churn-eda.git)
   cd spokify-churn-eda
