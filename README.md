# proyecto-fuga-clientes
Proyecto Final Ciencia de Datos II
# Predicción de Fuga de Clientes (Customer Churn) - Telecomunicaciones


## 📌 Descripción del Proyecto
El objetivo principal es desarrollar un modelo de Machine Learning Supervisado para predecir si un cliente cancelará sus servicios en el próximo periodo (fuga de clientes o *churn*). Al identificar estos perfiles, el negocio puede diseñar estrategias y promociones focalizadas para retenerlos.

## 📂 Archivos en este Repositorio
*   `entrega_final_churn.ipynb`: Cuaderno reproducible con todo el pipeline de datos (EDA, Limpieza, Pruebas de hipótesis, VIF, Modelado con XGBoost y explicabilidad con SHAP).
*   `requirements.txt`: Lista de librerías de Python requeridas para ejecutar el proyecto de forma reproducible.

## ⚙️ Requisitos de Instalación
Para replicar el entorno de desarrollo y ejecutar el notebook de forma local, instala las dependencias mediante:

```bash
pip install -r requirements.txt

Pipeline Metodológico Desarrollado
Entendimiento de Negocio: Formulación del problema y selección de métricas adecuadas (F1-Score y ROC-AUC).
EDA: Imputación de nulos y análisis de distribución.
Estadística: Detección de outliers (IQR) y pruebas de hipótesis (Mann-Whitney U para numéricas y Chi-cuadrado para categóricas con tamaño de efecto).
Preprocesamiento: Control de multicolinealidad con VIF (Factor de Inflación de la Varianza), One-Hot Encoding y estandarización.
Modelos: Entrenamiento de modelos y optimización de hiperparámetros con GridSearchCV.
Explicabilidad: Uso de SHAP para interpretar qué variables (como el tipo de contrato mensual) influyen más en la fuga de clientes.
