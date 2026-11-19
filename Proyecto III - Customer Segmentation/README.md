# 🛒 Customer Segmentation & Product Sales Analysis

## 🎯 Objetivo

Desarrollar un proyecto de análisis y segmentación de productos mediante técnicas de Machine Learning no supervisado, utilizando el algoritmo **K-Means**, con el propósito de identificar patrones de comportamiento comercial a partir de variables relacionadas con las ventas y los precios.

El proyecto busca identificar grupos de productos con características similares, analizar su desempeño comercial y descubrir diferencias entre categorías y regiones.

El flujo de trabajo abarca desde la integración, limpieza y transformación de datos, hasta la estandarización de variables, reducción de dimensionalidad mediante PCA, aplicación de algoritmos de clustering y evaluación de los resultados obtenidos.

---

## 🛠️ Tecnologías

- 🐍 Python
- 📊 Pandas
- 🔢 NumPy
- 📈 Matplotlib
- 🎨 Seaborn
- 🤖 Scikit-learn
- 📉 PCA (Principal Component Analysis)
- 📓 Jupyter Notebook

---

# 📌 Proyecto 1: Product Segmentation Using K-Means

## 📂 Dataset

Se utilizaron cinco conjuntos de datos relacionados con información de productos, segmentos, categorías, calendario y ventas:

- **DIM_PRODUCT:** Información de productos, fabricantes, marcas, formatos y características.
- **DIM_SEGMENT:** Clasificación de productos por segmentos.
- **DIM_CATEGORY:** Catálogo de categorías comerciales.
- **DIM_CALENDAR:** Información temporal organizada por semanas, años y meses.
- **FACT_SALES:** Información de ventas unitarias, valor de ventas, promedios semanales y regiones.

Se integraron las diferentes fuentes de información para construir una base de datos consolidada que permitiera analizar el comportamiento de los productos.

### 📊 Variables analizadas

- Fabricante
- Marca
- Producto
- Categoría
- Formato
- Segmento
- Región
- Ventas unitarias totales
- Valor total de ventas
- Promedio de ventas unitarias semanales
- Ventas diarias
- Precio promedio

---

## 🔍 Análisis Exploratorio (EDA)

Durante esta etapa se realizaron:

- Inspección inicial de los conjuntos de datos.
- Identificación de valores nulos.
- Detección de registros duplicados.
- Análisis de las características de los productos.
- Revisión de las variables relacionadas con las ventas.
- Integración de las tablas mediante operaciones de Merge.
- Análisis del comportamiento comercial por marca, categoría y región.

---

## ⚙️ Preprocesamiento

Se realizaron diferentes procesos para preparar la información antes de aplicar los algoritmos de Machine Learning:

- Renombramiento y estandarización de columnas.
- Tratamiento de valores nulos.
- Eliminación de registros duplicados.
- Limpieza y normalización de textos.
- Integración de las bases de datos.
- Conversión y unificación de fechas.
- Creación de la variable **Ventas Diarias**.
- Agrupación de registros por clave de producto.
- Creación de la variable **Precio Promedio**.
- Selección de variables numéricas para el modelado.
- Estandarización de características mediante **StandardScaler**.

---

## 🤖 Modelo utilizado

### K-Means Clustering

Se implementó el algoritmo **K-Means** para identificar grupos de productos con comportamientos similares de acuerdo con sus características comerciales.

Se utilizaron las siguientes variables:

- Total Unitario de Ventas.
- Valor Total de Ventas.
- Ventas Diarias.
- Promedio Total Unitario de Ventas Semanales.
- Precio Promedio.

Se realizaron:

- Entrenamiento del modelo K-Means.
- Evaluación de diferentes cantidades de clusters.
- Identificación de centroides.
- Asignación de productos a diferentes grupos.
- Visualización de los segmentos identificados.

### 📉 Selección del número de clusters

Para determinar el número adecuado de agrupaciones se utilizaron dos métodos:

**1. Método del Codo (Elbow Method)**

Se analizó la variación del WCSS (Within-Cluster Sum of Squares) para identificar el número de clusters adecuado.

**2. Coeficiente de Silueta (Silhouette Score)**

Se evaluó la calidad de las agrupaciones mediante diferentes valores de K.

Resultados obtenidos:

- **K = 2:** Silhouette Score ≈ 0.7967
- **K = 3:** Silhouette Score ≈ 0.4678
- **K = 4:** Silhouette Score ≈ 0.5307

Se exploraron modelos con diferentes cantidades de clusters para comparar sus resultados y visualizar los patrones identificados.

---

## 📊 Reducción de Dimensionalidad (PCA)

Se implementó **Principal Component Analysis (PCA)** para reducir las cinco variables originales a dos componentes principales.

Se realizaron:

- Estandarización de las variables.
- Aplicación de PCA.
- Reducción de dimensionalidad de cinco a dos componentes.
- Transformación de los datos originales.
- Aplicación de K-Means sobre los componentes principales.
- Visualización de los clusters en un plano bidimensional.

El objetivo fue facilitar la interpretación visual de las agrupaciones y observar la distribución de los productos.

---

# 📌 Proyecto 2: Segmentation by Product Category

## 📂 Agrupación por categorías

Se desarrolló un segundo análisis de segmentación enfocado en las categorías de productos.

Se identificaron y clasificaron las siguientes categorías:

- CLORO
- PRELAVADOR
- SAFE BLEACH
- SANITIZANTE

Se agruparon las ventas por categoría y se calcularon las siguientes variables:

- Total Unitario de Ventas.
- Valor Total de Ventas.
- Precio Promedio.

---

## 🤖 Modelo K-Means por categoría

Se aplicó nuevamente el algoritmo **K-Means**, utilizando dos variables principales:

- Volumen de ventas.
- Precio promedio.

Se realizaron:

- Estandarización de las variables mediante StandardScaler.
- Entrenamiento de K-Means con tres clusters.
- Asignación de categorías a sus respectivos grupos.
- Identificación de patrones de comportamiento comercial.
- Visualización de la segmentación por categoría.

---

# 🌎 Proyecto 3: Regional Sales Segmentation

## 📂 Análisis por región

Se realizó una segmentación geográfica para identificar diferencias en el comportamiento de las ventas entre las distintas regiones comerciales.

Se analizaron las siguientes regiones:

- TOTAL AUTOS AREA 1
- TOTAL AUTOS AREA 2
- TOTAL AUTOS AREA 3
- TOTAL AUTOS AREA 4
- TOTAL AUTOS AREA 5
- TOTAL AUTOS AREA 6
- TOTAL AUTOS SCANNING MEXICO

Se calcularon indicadores comerciales como:

- Total Unitario de Ventas.
- Valor Total de Ventas.
- Precio Promedio.

---

## 🤖 Modelo K-Means por región

Se implementó K-Means con tres clusters para identificar grupos de regiones con características comerciales similares.

Se realizaron:

- Agrupación de ventas por región.
- Estandarización de variables.
- Aplicación del algoritmo K-Means.
- Asignación de clusters a cada región.
- Comparación de volúmenes de ventas.
- Análisis de diferencias en los precios promedio.

---

# 🏷️ Análisis de Marcas

Se realizó un análisis adicional para identificar la participación de las marcas dentro de las diferentes categorías comerciales.

Se incluyeron:

- Identificación del número de marcas originales.
- Comparación de marcas con y sin registros de ventas.
- Identificación de marcas presentes en la base consolidada.
- Construcción de tablas dinámicas mediante **Pivot Tables**.
- Análisis del valor total de ventas por marca y categoría.
- Visualización del desempeño comercial mediante mapas de calor (Heatmaps).

---

# 📊 Resultados principales

✔️ Integración de cinco conjuntos de datos relacionados con productos, categorías, segmentos, calendario y ventas.

✔️ Limpieza, transformación y estandarización de la información.

✔️ Construcción de una base consolidada para el análisis comercial.

✔️ Identificación de patrones de comportamiento mediante el algoritmo **K-Means**.

✔️ Evaluación de diferentes cantidades de clusters mediante Elbow Method y Silhouette Score.

✔️ Reducción de dimensionalidad utilizando **PCA**.

✔️ Segmentación de productos según sus características de ventas y precios.

✔️ Identificación de grupos de categorías comerciales.

✔️ Segmentación de regiones con base en sus indicadores de ventas.

✔️ Análisis del desempeño de marcas por categoría.

✔️ Identificación de marcas sin registros de ventas en la base consolidada.

---

# 📈 Visualizaciones

El proyecto incluye diferentes visualizaciones para facilitar la interpretación de los resultados:

- Gráfico del método del codo (Elbow Method).
- Evaluación del coeficiente de silueta.
- Scatter Plots de segmentación de productos.
- Visualización de clusters y centroides.
- Gráficos de dispersión utilizando PCA.
- Segmentación por categoría.
- Gráficos de barras de variables promedio por cluster.
- Boxplots de distribución de ventas por cluster.
- Scatter Plots de segmentación regional.
- Heatmaps del desempeño de marcas por categoría.

---

# 🧠 Habilidades demostradas

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Data Integration
- Data Transformation
- Data Wrangling
- Data Aggregation
- Feature Engineering
- Feature Scaling
- Unsupervised Learning
- K-Means Clustering
- Principal Component Analysis (PCA)
- Dimensionality Reduction
- Cluster Evaluation
- Silhouette Analysis
- Elbow Method
- Product Segmentation
- Regional Analysis
- Sales Analysis
- Data Visualization
- Business Intelligence
- Python for Data Science
- Scikit-learn

---

# 📚 Algoritmos y técnicas utilizadas

- K-Means Clustering
- Principal Component Analysis (PCA)
- StandardScaler
- Elbow Method
- Silhouette Score
