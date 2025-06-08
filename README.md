# Proyecto Medical Insurance Cost Prediction

Este proyecto utiliza algoritmos de machine learning para predecir el costo de seguros médicos a partir de información demográfica y de estilo de vida. Se comparan modelos regresivos, se optimizan hiperparámetros y se analizan métricas clave para identificar el modelo más preciso y robusto.

---

## 📊 Dataset

- **Nombre:** [Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Tamaño:** 1338 registros
- **Características:**
  - `age`: Edad del asegurado
  - `sex`: Género
  - `bmi`: Índice de Masa Corporal
  - `children`: Número de hijos dependientes
  - `smoker`: Si fuma o no
  - `region`: Región geográfica (US)
  - `charges`: Costo del seguro médico (target)

---

## 🛠️ Tecnologías utilizadas

- Python 3
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebooks

---

## 🔄 Preprocesamiento

- Estandarización de variables numéricas (`StandardScaler`)
- Codificación One-Hot de variables categóricas
- Uso de `Pipeline` y `ColumnTransformer` para integrarlo todo

---

## 🤖 Modelos entrenados

- Linear Regression (baseline)
- Random Forest Regressor
- Gradient Boosting Regressor

> Se usó `GridSearchCV` para tuning de hiperparámetros y validación cruzada (5-fold).

---

## 📈 Resultados

| Model              | RMSE   | R²      | MAE   | MedAE | MAPE (%) |
|-------------------|--------|---------|-------|--------|-----------|
| Linear Regression | 5796.28 | 0.7836 | 4181.19 | 2695.14 | 46.89 |
| Random Forest     | 4591.93 | 0.8642 | 2522.79 | 1197.37 | 29.73 |
| Gradient Boosting | **4303.06** | **0.8807** | **2457.27** | 1636.15 | 32.21 |

> 🔥 **Gradient Boosting** fue el modelo con mejor desempeño general.

---

## 📊 Visualizaciones

- Distribución de características
- Matriz de correlación
- Importancia de variables
- Curvas de aprendizaje
- Análisis de residuos

> _(el notebook principal para más detalles)_

