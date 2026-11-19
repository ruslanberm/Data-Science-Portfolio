# 📊 Sales Performance Dashboard & Business Intelligence | Power BI

## 🎯 Objetivo

Desarrollar un dashboard interactivo utilizando **Microsoft Power BI** para analizar el comportamiento de las ventas desde diferentes perspectivas comerciales, facilitando la identificación de tendencias, patrones estacionales y oportunidades de negocio.

El proyecto busca transformar información comercial en indicadores clave de desempeño (KPIs) y visualizaciones interactivas que permitan evaluar el rendimiento de las ventas por año, mes, producto, categoría, marca y región.

El análisis abarca la evolución de las ventas, comparación entre períodos, seguimiento de indicadores acumulados y exploración de los principales factores que influyen en el desempeño comercial.

---

## 🛠️ Tecnologías

- 📊 Microsoft Power BI
- 📈 Power BI Desktop
- 🧮 DAX (Data Analysis Expressions)
- 🔄 Power Query
- 📉 Data Visualization
- 📊 Business Intelligence
- 🗄️ Data Modeling

---

# 📌 Parte 1: Sales Performance Analysis

## 📂 Modelo de datos

Se trabajó con información comercial organizada mediante tablas dimensionales y una tabla de hechos.

Se identificaron las siguientes tablas:

- **DIM_CATEGORY:** Información relacionada con las categorías comerciales.
- **DIM_PRODUCT:** Características de los productos, fabricantes, marcas, segmentos y categorías.
- **DIM_CALENDAR:** Información temporal organizada por años, meses y semanas.
- **FACT_SALES:** Información relacionada con las ventas, cantidades, valores y regiones.

La integración de estas tablas permite analizar el comportamiento comercial desde diferentes dimensiones.

---

## 📊 Indicadores clave (KPIs)

Se incorporaron indicadores para monitorear el desempeño comercial:

- **Total Sales:** Valor total de las ventas.
- **Sales Quantity:** Cantidad total de unidades vendidas.
- **Sales Value YTD:** Valor acumulado de ventas durante el año (Year-to-Date).
- **Sales Value VS LastYear:** Comparación del valor de ventas respecto al año anterior.
- **YTD VAR %:** Variación porcentual de las ventas acumuladas.
- **Sales YoY %:** Variación porcentual de las ventas respecto al año anterior.

Estos indicadores permiten evaluar el rendimiento comercial y comparar los resultados entre diferentes períodos.

---

# 📈 Parte 2: Sales Evolution & Regional Analysis

## 📊 Evolución de las ventas

Se desarrolló un análisis temporal para identificar el comportamiento de las ventas a través de los diferentes períodos.

Se analizaron:

- Evolución de ventas por año.
- Comportamiento mensual.
- Variaciones entre períodos.
- Desempeño por categoría.
- Distribución de ventas por región.

Se incorporó un gráfico de líneas para visualizar la evolución de las ventas y facilitar la comparación entre diferentes años.

### 🔍 Análisis regional

Se implementó una visualización geográfica mediante mapas para explorar el desempeño comercial de las diferentes regiones.

Se incorporó un filtro interactivo que permite seleccionar regiones y analizar su contribución al total de ventas.

---

# 🏷️ Parte 3: Product & Brand Performance Analysis

## 📂 Análisis por categoría y marca

Se desarrolló un análisis para identificar las categorías y marcas con mayor participación en las ventas.

Se utilizaron las siguientes dimensiones:

- Categoría.
- Marca.
- Producto.
- Año.
- Mes.

Se identificaron dos categorías con una participación importante en las ventas:

- CLORO (FABRIC)
- SAFE BLEACH (FABRIC)

---

## 📊 Análisis de tendencias comerciales

Se incorporaron visualizaciones para estudiar:

- Distribución de ventas por categoría.
- Desempeño de marcas.
- Comportamiento mensual.
- Patrones estacionales.
- Comparación de ventas entre períodos.

Se utilizaron gráficos de tipo **Treemap** y **Ribbon Chart** para facilitar la identificación de las categorías y marcas con mayor participación comercial.

### 🔍 Principales insights

- Las categorías CLORO y SAFE BLEACH concentran una parte importante de las ventas.
- Se identifican picos estacionales principalmente durante mayo, junio y noviembre.
- CLORO presenta una participación importante en los períodos de mayor actividad comercial.
- SAFE BLEACH mantiene un comportamiento relativamente más estable durante el período analizado.

---

# 📉 Parte 4: Year-to-Date & Year-over-Year Analysis

## 📊 Comparación de indicadores comerciales

Se desarrolló un análisis comparativo para evaluar el comportamiento de las ventas acumuladas respecto al año anterior.

Se utilizaron indicadores como:

- Sales Value YTD.
- Sales Value VS LastYear.
- YTD VAR %.
- Sales YoY %.

Se incorporaron filtros y marcadores interactivos para facilitar la comparación entre diferentes años.

### 🔍 Principales insights

- Se identificó una variación aproximada de **-42.4% en las ventas YTD** respecto al año anterior, considerando los datos disponibles.
- El año 2023 no representa un período completo dentro del análisis.
- El desempeño de 2023 muestra una disminución frente al año anterior en los datos disponibles.

---

# 🌳 Parte 5: Sales Decomposition & Business Insights

## 🔍 Decomposition Tree

Se implementó una visualización de tipo **Decomposition Tree** para explorar los factores que contribuyen al valor total de las ventas.

Se utilizaron diferentes dimensiones para descomponer el indicador comercial:

- Región.
- Año.
- Marca.
- Segmento.
- Categoría.
- Fabricante.

Esta herramienta permite profundizar en el análisis y detectar qué combinaciones de variables tienen mayor impacto en el desempeño comercial.

---

# 🎛️ Interactividad del Dashboard

Se incorporaron diferentes elementos interactivos para facilitar la exploración de la información:

- Filtros por región.
- Segmentadores por año.
- Marcadores (Bookmarks) para alternar entre períodos.
- Navegación entre páginas.
- Visualizaciones interactivas.
- Exploración de indicadores comerciales.
- Análisis dinámico mediante selección de categorías y marcas.

El dashboard está organizado en cuatro páginas:

- **GUÍA:** Orientación para navegar por el reporte.
- **GRÁFICOS 1:** Evolución de ventas y análisis regional.
- **GRÁFICOS 2:** Análisis de categorías, marcas y comparación de períodos.
- **GRÁFICOS 3:** Descomposición de ventas mediante Decomposition Tree.

---

# 📊 Resultados principales

✔️ Desarrollo de un dashboard interactivo utilizando Power BI.

✔️ Organización de información comercial mediante tablas dimensionales y de hechos.

✔️ Implementación de indicadores clave de desempeño (KPIs).

✔️ Análisis de ventas por año, mes, categoría, marca y región.

✔️ Identificación de patrones estacionales en el comportamiento de las ventas.

✔️ Comparación de indicadores Year-to-Date (YTD).

✔️ Análisis de variaciones Year-over-Year (YoY).

✔️ Identificación de categorías con mayor participación comercial.

✔️ Implementación de visualizaciones geográficas.

✔️ Desarrollo de un análisis de descomposición mediante Decomposition Tree.

✔️ Incorporación de filtros, segmentadores y marcadores interactivos.

✔️ Generación de insights comerciales para facilitar la toma de decisiones.

---

# 📈 Visualizaciones

El dashboard incluye diferentes recursos gráficos para facilitar la interpretación de los resultados:

- Line Charts
- Ribbon Charts
- Treemaps
- Geographic Maps
- Decomposition Tree
- KPI Cards
- Tables
- Interactive Slicers
- Year-to-Date Analysis
- Year-over-Year Comparison

---

# 🧠 Habilidades demostradas

- Business Intelligence
- Data Visualization
- Dashboard Development
- Data Modeling
- DAX
- Power Query
- KPI Development
- Sales Performance Analysis
- Sales Forecasting Concepts
- Time Intelligence
- Year-to-Date Analysis
- Year-over-Year Analysis
- Trend Analysis
- Seasonality Analysis
- Regional Sales Analysis
- Product Performance Analysis
- Interactive Reporting
- Data Storytelling
- Business Analytics
- Microsoft Power BI

---

# 📚 Herramientas y funcionalidades utilizadas

- Microsoft Power BI Desktop
- DAX Measures
- Power Query
- Data Modeling
- KPI Cards
- Line Charts
- Ribbon Charts
- Treemaps
- Geographic Maps
- Decomposition Tree
- Bookmarks
- Page Navigation
- Interactive Slicers
