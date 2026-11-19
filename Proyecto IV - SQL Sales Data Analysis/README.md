🏢 Sales Data Management & Business Analysis | SQL Server

🎯 Objetivo

Desarrollar un proyecto de gestión, integración y análisis de datos comerciales utilizando Microsoft SQL Server, con el propósito de construir una base de datos relacional que permita almacenar, organizar y consultar información relacionada con productos, categorías, segmentos, calendario y ventas.

El proyecto consiste en la creación de una base de datos desde cero, definición de estructuras mediante sentencias SQL, importación de archivos CSV y ejecución de consultas para analizar el comportamiento de las ventas desde diferentes perspectivas comerciales.

El flujo de trabajo abarca desde la creación y carga de tablas, hasta la integración de información mediante operaciones JOIN y la generación de indicadores de ventas por categoría, marca, región y período.

🛠️ Tecnologías

🗄️ Microsoft SQL Server

💻 SQL Server Management Studio (SSMS)

📄 SQL (Structured Query Language)

📊 Archivos CSV

🔗 Relational Database Management

📈 Business Data Analysis

📌 Parte 1: Database Creation & Data Integration

🗄️ Creación de la base de datos

Se creó una base de datos denominada ProyectoVentas, utilizando Microsoft SQL Server.

Se definieron cinco tablas principales para organizar la información comercial:

DIM_CATEGORY: Información relacionada con las categorías de productos.

DIM_PRODUCT: Características de los productos, fabricantes, marcas, formatos y atributos.

DIM_SEGMENT: Clasificación de productos de acuerdo con sus características y segmentos comerciales.

DIM_CALENDAR: Información temporal organizada por semanas, años, meses y fechas.

FACT_SALES: Información relacionada con las ventas unitarias, valores de ventas, promedios semanales y regiones.

⚙️ Estructuración de tablas

Se utilizaron sentencias SQL para definir la estructura de cada tabla, estableciendo:

Tipos de datos.

Longitud de campos.

Claves primarias (Primary Keys).

Campos numéricos y descriptivos.

Estructura de las tablas dimensionales y de hechos.

Se utilizó un modelo de organización basado en tablas de dimensiones y una tabla de hechos para facilitar las consultas y el análisis comercial.

📂 Parte 2: Data Import & Transformation

📥 Importación de datos

Se realizó la carga de información desde archivos CSV hacia las tablas previamente creadas.

Se utilizó la instrucción BULK INSERT para importar los siguientes conjuntos de datos:

DIM_CATEGORY.csv

DIM_PRODUCT.csv

DIM_SEGMENT.csv

DIM_CALENDAR.csv

FACT_SALES.csv

Se configuraron parámetros de importación como:

FORMAT = CSV

FIRSTROW = 2

FIELDQUOTE = '"'

TABLOCK

Esto permitió importar los registros directamente desde los archivos CSV hacia SQL Server.

🔄 Transformación de datos

Para realizar la importación del calendario se creó una tabla temporal denominada DIM_CALENDAR_TEMP.

Se utilizó esta estructura intermedia para cargar inicialmente los campos como texto y posteriormente convertirlos a sus tipos de datos correspondientes.

Se realizaron:

Creación de una tabla temporal.

Importación de los registros del calendario.

Conversión de campos mediante TRY_CONVERT.

Transformación de variables de año, mes y número de semana a valores enteros.

Conversión de fechas utilizando el formato correspondiente.

Inserción de los registros transformados en DIM_CALENDAR.

Eliminación de la tabla temporal después de completar el proceso.

🔍 Parte 3: Data Validation & Relationship Analysis

✅ Validación de información

Se realizaron consultas SQL para comprobar que los datos se hubieran importado correctamente.

Se utilizaron consultas para:

Contabilizar los registros de cada tabla.

Verificar la información almacenada en DIM_PRODUCT.

Consultar los primeros diez registros de productos.

Comprobar coincidencias entre las tablas FACT_SALES y DIM_PRODUCT.

Validar las relaciones mediante campos de identificación de productos.

🔗 Integración de tablas (JOIN)

Se implementaron operaciones INNER JOIN para relacionar la información de ventas con las características de los productos.

Se utilizaron principalmente las siguientes relaciones:

FACT_SALES con DIM_PRODUCT mediante ITEM_CODE e ITEM.

FACT_SALES con DIM_CALENDAR mediante WEEK.

Estas relaciones permitieron combinar información comercial y temporal para realizar consultas más completas.

📊 Parte 4: Business Analysis & Sales Queries

🏷️ Análisis de ventas por categoría

Se desarrolló una consulta para identificar el comportamiento de las ventas según los atributos de los productos.

Se calcularon:

Unidades vendidas.

Ventas totales.

Distribución de ventas por categoría.

Se utilizaron las funciones:

SUM()

GROUP BY

ORDER BY

Los resultados se organizaron de mayor a menor según el valor total de ventas.

🛒 Análisis de ventas por marca

Se realizó una consulta para analizar el desempeño comercial de las diferentes marcas presentes en la base de datos.

Se identificaron:

Marcas comercializadas.

Unidades vendidas por marca.

Valor total de ventas por marca.

Se utilizó la agrupación de registros mediante GROUP BY y la función de agregación SUM() para calcular los indicadores comerciales.

🌎 Análisis de ventas por región

Se desarrolló una consulta para identificar las diferencias en el comportamiento comercial entre las distintas regiones.

Se analizaron:

Regiones comerciales.

Unidades vendidas por región.

Valor total de ventas por región.

Los resultados se ordenaron de acuerdo con el valor total de ventas, permitiendo identificar las regiones con mayor actividad comercial.

📅 Análisis de ventas por período

Se realizó un análisis temporal para estudiar el comportamiento de las ventas a lo largo de los diferentes años y meses.

Se integraron las tablas FACT_SALES y DIM_CALENDAR mediante la variable WEEK.

Se calcularon:

Año.

Mes.

Unidades vendidas.

Valor total de ventas.

Se utilizaron operaciones INNER JOIN, GROUP BY y ORDER BY para organizar la información cronológicamente y analizar la evolución de las ventas.

📊 Resultados principales

✔️ Creación de una base de datos relacional utilizando Microsoft SQL Server.

✔️ Diseño y estructuración de cinco tablas comerciales.

✔️ Definición de tipos de datos y claves primarias.

✔️ Importación de información mediante archivos CSV y BULK INSERT.

✔️ Transformación de datos temporales mediante tablas intermedias.

✔️ Conversión de tipos de datos utilizando TRY_CONVERT.

✔️ Validación de registros mediante consultas SQL.

✔️ Integración de tablas mediante operaciones INNER JOIN.

✔️ Análisis de unidades y valores totales de ventas.

✔️ Identificación del comportamiento comercial por categoría y marca.

✔️ Comparación de ventas entre diferentes regiones.

✔️ Análisis temporal de ventas por año y mes.

🧠 Habilidades demostradas

SQL Database Creation

Database Design

Relational Database Management

Data Modeling

Data Importation

BULK INSERT

Data Transformation

Data Type Conversion

Temporary Tables

Primary Keys

Data Validation

INNER JOIN

Aggregate Functions

GROUP BY

ORDER BY

SUM()

TRY_CONVERT()

Data Integration

Business Analysis

Sales Analysis

Temporal Analysis

Microsoft SQL Server

📚 Comandos y funciones SQL utilizados

CREATE DATABASE

USE

CREATE TABLE

PRIMARY KEY

BULK INSERT

INSERT INTO

SELECT

COUNT()

SUM()

INNER JOIN

WHERE

GROUP BY

ORDER BY

TRY_CONVERT()

DROP TABLE

UNION ALL
