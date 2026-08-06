# ❤️ Heart Attack Prediction & Handwritten Digit Recognition

## 🎯 Objetivo

Desarrollar un flujo completo de Machine Learning utilizando algoritmos de aprendizaje supervisado para resolver dos problemas de clasificación:

- Predicción de riesgo de ataque al corazón mediante variables clínicas.
- Reconocimiento de dígitos escritos a mano utilizando el dataset MNIST.

El proyecto abarca desde el análisis exploratorio de datos (EDA), preprocesamiento y entrenamiento de modelos, hasta la evaluación del desempeño y comparación entre diferentes algoritmos de clasificación.

---

## 🛠️ Tecnologías

- 🐍 Python
- 📊 Pandas
- 🔢 NumPy
- 📈 Matplotlib
- 🎨 Seaborn
- 🤖 Scikit-learn
- 📄 YData Profiling
- 🖼️ Pillow (PIL)
- 📓 Jupyter Notebook

---

# 📌 Proyecto 1: Predicción de Ataque al Corazón

## 📂 Dataset

Se utilizó el dataset **Heart Attack**, el cual contiene variables clínicas relacionadas con la salud cardiovascular de los pacientes.

Algunas variables analizadas:

- Edad
- Sexo
- Tipo de dolor de pecho
- Presión arterial
- Colesterol
- Azúcar en sangre
- Electrocardiograma
- Frecuencia cardiaca máxima
- Angina inducida por ejercicio
- Variable objetivo (Heart Attack)

---

## 🔍 Análisis Exploratorio (EDA)

Durante esta etapa se realizaron:

- Estadísticas descriptivas.
- Matriz de correlación con la variable objetivo.
- Histogramas de todas las variables.
- Diagramas de dispersión.
- Perfil automático del dataset mediante **YData Profiling**.

---

## ⚙️ Preprocesamiento

- Selección de variables predictoras.
- División de datos en entrenamiento (70%) y prueba (30%).
- Escalamiento mediante **MinMaxScaler**.
- Preparación de variables independientes y objetivo.

---

## 🤖 Modelo utilizado

### K-Nearest Neighbors (KNN)

Se entrenó un clasificador utilizando Scikit-Learn para predecir la probabilidad de ataque al corazón.

Se realizaron:

- Entrenamiento del modelo.
- Predicción sobre nuevos registros simulados.
- Clasificación binaria.

---

# ✍️ Proyecto 2: Reconocimiento de Dígitos (MNIST)

## 📂 Dataset

Se utilizó el conjunto de datos **MNIST**, compuesto por imágenes de 28×28 píxeles correspondientes a los dígitos del 0 al 9.

---

## 🔍 Procesamiento de imágenes

El proyecto incluye:

- Visualización de imágenes.
- Conversión de imágenes propias.
- Redimensionamiento a 28×28 píxeles.
- Eliminación de ruido.
- Conversión de imágenes al formato requerido por Scikit-Learn.
- Predicción sobre imágenes creadas por el usuario.

---

## 🤖 Modelos implementados

### ✅ K-Nearest Neighbors

Se entrenó un clasificador utilizando diferentes valores de **k**.

Se evaluó:

- Accuracy
- Overfitting
- Underfitting
- Selección del mejor número de vecinos.

**Mejor valor encontrado:**

- **k = 3**
- **Accuracy ≈ 96.64%** :contentReference[oaicite:0]{index=0}

---

### ✅ Regresión Logística

Se implementó un segundo modelo de clasificación utilizando:

- StandardScaler
- LogisticRegression (solver="saga")

Se evaluó mediante:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report

**Accuracy obtenido:**

- **92.06%** :contentReference[oaicite:1]{index=1}

---

# 📊 Resultados principales

✔️ Análisis exploratorio completo del dataset clínico.

✔️ Identificación de las variables con mayor correlación respecto al riesgo de ataque cardíaco.

✔️ Implementación del algoritmo **K-Nearest Neighbors** para clasificación binaria.

✔️ Predicción de nuevos pacientes utilizando datos simulados.

✔️ Clasificación automática de imágenes manuscritas.

✔️ Comparación entre **KNN** y **Regresión Logística**.

✔️ Optimización del parámetro **k** mediante análisis de precisión.

✔️ Evaluación del desempeño utilizando métricas de Machine Learning.

---

# 📈 Visualizaciones

- Histogramas
- Scatter Plots
- Matriz de correlación
- Reporte automático de EDA
- Curvas de precisión Training vs Testing
- Visualización de imágenes MNIST
- Predicción de imágenes personalizadas

---

# 🧠 Habilidades demostradas

- Exploratory Data Analysis (EDA)
- Data Visualization
- Feature Selection
- Data Preprocessing
- Feature Scaling
- Supervised Learning
- Binary Classification
- Multiclass Classification
- Model Evaluation
- Hyperparameter Tuning
- Computer Vision (MNIST)
- Predictive Modeling
- Scikit-learn

---

# 📚 Algoritmos utilizados

- K-Nearest Neighbors (KNN)
- Logistic Regression

---

## 🚀 Autor

**Tu Nombre**

Data Analytics | Machine Learning | Python
