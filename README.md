# Data-Science-Portfolio

## 📱 Análisis completo de aplicaciones de Android (Google Play Store)

### 🎯 Objetivo

Analizar más de **9,600 aplicaciones** de Google Play Store y miles de reseñas de usuarios para identificar los factores que influyen en el éxito de una aplicación, tales como calificación, categoría, tamaño, precio, número de instalaciones y percepción de los usuarios mediante análisis de sentimientos.

---

## 🔧 Tecnologías utilizadas

- 🐍 Python
- 📊 Pandas
- 🔢 NumPy
- 📈 Matplotlib
- 🎨 Seaborn
- 💬 Análisis de sentimientos (dataset con polaridad y subjetividad)
- 📓 Google Colab

---

## 📂 Conjunto de datos

Se trabajó con dos datasets:

- **apps.csv:** información de **9,659 aplicaciones** con características como categoría, rating, tamaño, instalaciones, precio, versión de Android, género y fecha de actualización.
- **user_reviews.csv:** más de **100 reseñas por aplicación**, incluyendo:
  - Sentimiento
  - Polaridad
  - Subjetividad

---

## 🔍 Proceso de análisis

### 🧹 1. Limpieza y preparación de datos

- Eliminación de registros duplicados.
- Conversión de columnas categóricas a numéricas.
- Limpieza de caracteres especiales (`+`, `,`, `$`) mediante funciones lambda.
- Conversión de variables **Installs** y **Price** a tipo numérico.
- Eliminación de valores nulos para el análisis estadístico.

---

### 📊 2. Análisis exploratorio (EDA)

Se analizaron diferentes aspectos del ecosistema de Google Play:

- Distribución de aplicaciones por categoría.
- Estadísticas descriptivas del dataset.
- Distribución de calificaciones (Rating).
- Promedio de rating por categoría.
- Relación entre tamaño de la aplicación y calificación.
- Relación entre precio y rating de aplicaciones de pago.
- Tendencias de precios entre categorías.
- Identificación de aplicaciones con precios superiores a **$200 USD**.

---

### 📈 3. Comparación entre aplicaciones gratuitas y de pago

Se compararon ambas estrategias de monetización mediante:

- Calificación promedio.
- Tamaño promedio.
- Distribución por categorías.
- Distribución de precios.
- Volumen total de instalaciones.
- Visualizaciones mediante gráficos de barras e histogramas.

---

### 💬 4. Análisis de sentimientos

Se integraron las reseñas de usuarios con la información de las aplicaciones para analizar:

- Distribución de sentimientos positivos, negativos y neutrales.
- Polaridad del sentimiento.
- Comparación del sentimiento entre aplicaciones gratuitas y de pago mediante diagramas BoxPlot.

---

## 📊 Resultados clave

- Se analizaron **9,659 aplicaciones** pertenecientes a **33 categorías**.
- La calificación promedio del ecosistema fue de **4.17/5**.
- Las categorías **Family** y **Game** concentran la mayor cantidad de aplicaciones disponibles.
- Las aplicaciones de pago presentan una calificación promedio ligeramente superior (**4.26**) respecto a las gratuitas (**4.17**).
- Las aplicaciones gratuitas concentran la mayor cantidad de instalaciones (más de **75 mil millones**).
- Se identificaron aplicaciones con precios de hasta **$400 USD**, principalmente en las categorías **Finance**, **Lifestyle** y **Family**.
- Se observó una relación moderada entre el tamaño de la aplicación, el precio y la calificación mediante visualizaciones exploratorias.
- El análisis de sentimientos permitió evaluar la percepción de los usuarios utilizando la polaridad de las reseñas.

---

## 📈 Visualizaciones realizadas

- Gráficas de barras por categoría.
- Histogramas de distribución.
- Scatter Plot.
- Joint Plot.
- Strip Plot.
- BoxPlot.
- Histogramas de precios.
- Barras comparativas de instalaciones.
- Distribución de polaridad de sentimientos.

---

## 📚 Principales habilidades demostradas

- Limpieza y transformación de datos.
- Análisis exploratorio de datos (EDA).
- Visualización de datos.
- Estadística descriptiva.
- Integración de múltiples datasets.
- Análisis de sentimientos.
- Comparación de estrategias de monetización.
- Comunicación de hallazgos mediante visualizaciones.
