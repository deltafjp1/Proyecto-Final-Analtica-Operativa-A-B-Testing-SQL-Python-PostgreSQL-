# Data Analytics Portfolio Project | Operational Analytics, A/B Testing & SQL

 🇪🇸 Proyecto de analítica de datos aplicado a operaciones, experimentación digital y consultas SQL de negocio.  
🇬🇧 Data analytics project focused on operations, digital experimentation, and SQL business queries.

**Autor:** Francisco Pinto  
**Stack:** Python (pandas, numpy), Jupyter, SQL (PostgreSQL)

## Acceso rápido a entregables / Quick Access to Deliverables

| Entregable / Deliverable | Enlace directo / Direct Link |
|---|---|
| 📓 Notebook principal — Analítica operativa / Main notebook — Operational Analytics | [Abrir notebook / Open notebook](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/Proyecto%20final%20merged/Proyecto_Final_Bootcamp_data_analitics.ipynb) |
| 🧪 Notebook y datasets — Prueba A/B / Notebook and datasets — A/B Testing | [Abrir carpeta / Open folder](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/Test%20AB) |
| 🗄️ Notebook SQL / SQL notebook | [Abrir notebook / Open notebook](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/proyecto%20final%20entrega%20SQL.ipynb) |
| 🗄️ Notebook SQL revisado / Revised SQL notebook | [Abrir notebook / Open notebook](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/entrega%20de%20proyecto%20final%20sql-%20version%20revisada.ipynb) |
| 🎞️ Presentación final / Final presentation | [Abrir PDF / Open PDF](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/presentacion%20proyecto%20Final%20telecomunicaciones.pdf) |
| 📈 Gráficas exportadas / Exported charts | [Abrir carpeta / Open folder](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/graficas_pdf) |

---

## Descripción / Overview

🇪🇸
Este repositorio reúne tres casos independientes de análisis de datos orientados a resolver preguntas de negocio mediante Python, SQL, análisis exploratorio, métricas operativas, pruebas estadísticas y visualización de resultados.

El proyecto está diseñado para demostrar habilidades clave de un Analista de Datos Junior: limpieza y preparación de datos, construcción de KPIs, análisis de comportamiento, validación de hipótesis, consultas SQL y comunicación de insights accionables.

🇬🇧
This repository contains three independent data analytics case studies focused on solving business questions using Python, SQL, exploratory data analysis, operational metrics, statistical testing, and result visualization.

The project demonstrates key Junior Data Analyst skills: data cleaning and preparation, KPI design, behavioral analysis, hypothesis testing, SQL querying, and communication of actionable insights.

---

## Casos incluidos / Included Case Studies

### 🇪🇸 Español

| Caso                                    | Enfoque                                                                                                                                                    | Herramientas                               | Valor de negocio                                                                                  |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| 1. Analítica operativa para Call Center | Evaluación del desempeño de operadores mediante KPIs operativos como tasa de llamadas perdidas, tiempo promedio de espera y volumen de llamadas salientes. | Python, pandas, análisis estadístico       | Priorización de coaching, mejora del servicio y monitoreo del desempeño operativo.                |
| 2. Prueba A/B para funnel de conversión | Análisis del comportamiento de usuarios dentro de un funnel digital y validación de hipótesis mediante pruebas estadísticas.                               | Python, pandas, z-test, análisis de funnel | Validación de decisiones de producto con evidencia estadística antes de implementar cambios.      |
| 3. Análisis SQL de negocio              | Consultas sobre una base relacional de libros, autores, editoriales, calificaciones y reseñas para responder preguntas de negocio.                         | PostgreSQL, SQL joins, agregaciones, CTEs  | Extracción de KPIs y generación de respuestas de negocio a partir de bases de datos relacionales. |

### 🇬🇧 English

| Case                                 | Focus                                                                                                                               | Tools                                     | Business Value                                                                           |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------- | ---------------------------------------------------------------------------------------- |
| 1. Call Center Operational Analytics | Evaluation of operator performance using operational KPIs such as missed call rate, average waiting time, and outbound call volume. | Python, pandas, statistical analysis      | Prioritization of coaching, service improvement, and operational performance monitoring. |
| 2. A/B Testing for Conversion Funnel | Analysis of user behavior within a digital funnel and hypothesis validation through statistical testing.                            | Python, pandas, z-test, funnel analysis   | Validation of product decisions with statistical evidence before implementing changes.   |
| 3. SQL Business Analytics            | Queries on a relational database of books, authors, publishers, ratings, and reviews to answer business questions.                  | PostgreSQL, SQL joins, aggregations, CTEs | Extraction of KPIs and business insights from relational databases.                      |

## 1. Analítica operativa para Call Center / Call Center Operational Analytics

### Objetivo / Objective

🇪🇸
Identificar operadores con posibles patrones de bajo desempeño en un call center mediante el análisis de métricas operativas como tasa de llamadas perdidas, tiempo promedio de espera y volumen de llamadas salientes.

🇬🇧
Identify operators with potential low-performance patterns in a call center by analyzing operational metrics such as missed call rate, average waiting time, and outbound call volume.

---

### Pregunta de negocio / Business Question

🇪🇸
¿Qué operadores presentan señales de ineficiencia operativa y deberían ser priorizados para seguimiento, retroalimentación o coaching?

🇬🇧
Which operators show signs of operational inefficiency and should be prioritized for monitoring, feedback, or coaching?

---

### Datos / Data

🇪🇸
El análisis utiliza datos operativos de llamadas del servicio CallMeMaybe, incluyendo información sobre llamadas entrantes, llamadas salientes, duración de llamadas, tiempos de espera, llamadas perdidas, operadores y fechas de actividad.

🇬🇧
The analysis uses operational call data from the CallMeMaybe service, including information about inbound calls, outbound calls, call duration, waiting times, missed calls, operators, and activity dates.

---

### Proceso / Process

🇪🇸

1. Limpieza y revisión inicial de los datos.
2. Validación de tipos de datos, fechas y valores ausentes.
3. Separación de métricas relevantes para llamadas entrantes y salientes.
4. Construcción de KPIs operativos:

   * Missed rate.
   * Average waiting time.
   * Outbound call volume.
5. Segmentación de operadores según criterios cuantitativos.
6. Identificación de operadores potencialmente ineficientes.
7. Comparación estadística entre operadores eficientes e ineficientes.
8. Comunicación de hallazgos mediante notebook, gráficos y presentación.

🇬🇧

1. Initial data cleaning and review.
2. Validation of data types, dates, and missing values.
3. Separation of relevant metrics for inbound and outbound calls.
4. Creation of operational KPIs:

   * Missed rate.
   * Average waiting time.
   * Outbound call volume.
5. Operator segmentation using quantitative criteria.
6. Identification of potentially inefficient operators.
7. Statistical comparison between efficient and inefficient operators.
8. Communication of findings through notebook, charts, and presentation.

---

### Insights clave / Key Insights

🇪🇸

* Los operadores con mayor tasa de llamadas perdidas representan un riesgo para la calidad del servicio y la experiencia del cliente.
* El tiempo promedio de espera permite detectar posibles cuellos de botella operativos.
* La combinación de varios KPIs ofrece una visión más justa del desempeño que analizar una sola métrica de forma aislada.
* La segmentación por percentiles ayuda a priorizar operadores para acciones de mejora.

🇬🇧

* Operators with higher missed call rates represent a risk to service quality and customer experience.
* Average waiting time helps detect potential operational bottlenecks.
* Combining multiple KPIs provides a fairer performance view than analyzing a single metric in isolation.
* Percentile-based segmentation helps prioritize operators for improvement actions.

---

### Recomendación / Recommendation

🇪🇸
En un contexto laboral real, este análisis podría utilizarse para construir un sistema periódico de monitoreo operativo, priorizar sesiones de coaching, reducir tiempos de espera y mejorar la calidad del servicio al cliente.

🇬🇧
In a real business context, this analysis could be used to build a recurring operational monitoring system, prioritize coaching sessions, reduce waiting times, and improve customer service quality.

---

### Entregables / Deliverables

* Notebook principal / Main notebook: [Proyecto_Final_Bootcamp_data_analitics.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/Proyecto%20final%20merged/Proyecto_Final_Bootcamp_data_analitics.ipynb)
* Presentación / Presentation: [presentacion proyecto Final telecomunicaciones.pdf](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/presentacion%20proyecto%20Final%20telecomunicaciones.pdf)
* Gráficas exportadas / Exported charts: [graficas_pdf/](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/graficas_pdf)


## 2. Prueba A/B para funnel de conversión / A/B Testing for Conversion Funnel

### Objetivo / Objective

🇪🇸
Evaluar el desempeño de una prueba A/B para determinar si una nueva experiencia dentro del funnel digital mejora la conversión de usuarios frente al grupo de control.

🇬🇧
Evaluate the performance of an A/B test to determine whether a new digital funnel experience improves user conversion compared to the control group.

---

### Pregunta de negocio / Business Question

🇪🇸
¿La nueva experiencia del funnel genera una mejora significativa en la conversión de usuarios y debería implementarse como versión definitiva?

🇬🇧
Does the new funnel experience generate a statistically significant improvement in user conversion, and should it be implemented as the final version?

---

### Datos / Data

🇪🇸
El análisis utiliza datos de un experimento digital con usuarios asignados a dos grupos:

* **Grupo A:** grupo de control.
* **Grupo B:** grupo experimental con la nueva experiencia del funnel.

Los datos incluyen información sobre usuarios, eventos del funnel, fechas de actividad, grupo experimental y comportamiento dentro de etapas como visualización de producto, carrito y compra.

🇬🇧
The analysis uses data from a digital experiment with users assigned to two groups:

* **Group A:** control group.
* **Group B:** experimental group with the new funnel experience.

The data includes information about users, funnel events, activity dates, experiment group, and behavior across stages such as product view, cart, and purchase.

---

### Proceso / Process

🇪🇸

1. Revisión inicial de los datasets del experimento.
2. Validación de fechas de inicio, finalización y periodo válido de análisis.
3. Identificación de usuarios por grupo experimental.
4. Revisión de consistencia entre usuarios, eventos y participantes.
5. Construcción del funnel de conversión.
6. Cálculo de tasas de conversión por etapa.
7. Comparación entre grupo A y grupo B.
8. Aplicación de pruebas estadísticas de proporciones para validar diferencias.
9. Interpretación de resultados desde una perspectiva de negocio.

🇬🇧

1. Initial review of the experiment datasets.
2. Validation of start date, end date, and valid analysis period.
3. Identification of users by experiment group.
4. Consistency checks between users, events, and participants.
5. Construction of the conversion funnel.
6. Calculation of conversion rates by stage.
7. Comparison between Group A and Group B.
8. Application of proportion statistical tests to validate differences.
9. Interpretation of results from a business perspective.

---

### Métricas analizadas / Metrics Analyzed

🇪🇸

* Usuarios por grupo experimental.
* Conversión por etapa del funnel.
* Conversión de visualización de producto a carrito.
* Conversión de carrito a compra.
* Conversión final a compra.
* Diferencias porcentuales entre grupo A y grupo B.
* Significancia estadística mediante pruebas de hipótesis.

🇬🇧

* Users by experiment group.
* Conversion by funnel stage.
* Conversion from product view to cart.
* Conversion from cart to purchase.
* Final purchase conversion.
* Percentage differences between Group A and Group B.
* Statistical significance through hypothesis testing.

---

### Insights clave / Key Insights

🇪🇸

* El análisis del funnel permite identificar en qué etapa se pierden más usuarios.
* La comparación entre grupos ayuda a evaluar si el cambio propuesto realmente mejora el comportamiento del usuario.
* Las pruebas estadísticas permiten diferenciar entre una variación aleatoria y una mejora significativa.
* El resultado del experimento no debe evaluarse solo por diferencias porcentuales, sino también por significancia estadística y contexto de negocio.

🇬🇧

* Funnel analysis helps identify which stage loses the most users.
* Group comparison helps evaluate whether the proposed change actually improves user behavior.
* Statistical testing helps distinguish between random variation and significant improvement.
* The experiment result should not be evaluated only through percentage differences, but also through statistical significance and business context.

---

### Recomendación / Recommendation

🇪🇸
En un contexto laboral real, este análisis permitiría decidir si una nueva funcionalidad o experiencia digital debe implementarse, descartarse o seguir iterándose. Si el grupo experimental no muestra una mejora estadísticamente significativa, la recomendación sería no lanzar el cambio de forma definitiva y revisar posibles ajustes en diseño, segmentación o experiencia de usuario.

🇬🇧
In a real business context, this analysis would support the decision of whether a new feature or digital experience should be implemented, discarded, or further iterated. If the experimental group does not show a statistically significant improvement, the recommendation would be not to fully launch the change and to review possible adjustments in design, segmentation, or user experience.

---

### Entregables / Deliverables

* Notebook y datasets de análisis A/B / A/B testing notebook and datasets: [Test AB/](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/Test%20AB)
* Análisis de funnel / Funnel analysis
* Pruebas estadísticas / Statistical testing


## 3. Análisis SQL de negocio / SQL Business Analytics

### Objetivo / Objective

🇪🇸
Resolver preguntas de negocio mediante consultas SQL sobre una base de datos relacional, aplicando joins, filtros, agregaciones y métricas para extraer información útil sobre libros, autores, editoriales, calificaciones y reseñas.

🇬🇧
Solve business questions through SQL queries on a relational database, applying joins, filters, aggregations, and metrics to extract useful information about books, authors, publishers, ratings, and reviews.

---

### Pregunta de negocio / Business Question

🇪🇸
¿Cómo se puede utilizar SQL para extraer KPIs y responder preguntas clave sobre desempeño editorial, comportamiento de usuarios, calificaciones y reseñas?

🇬🇧
How can SQL be used to extract KPIs and answer key questions about publishing performance, user behavior, ratings, and reviews?

---

### Datos / Data

🇪🇸
El análisis utiliza una base de datos relacional compuesta por tablas relacionadas con libros, autores, editoriales, calificaciones y reseñas de usuarios.

Las tablas permiten analizar información como:

* Libros publicados.
* Autores asociados.
* Editoriales.
* Calificaciones promedio.
* Reseñas textuales.
* Usuarios que califican y escriben reseñas.

🇬🇧
The analysis uses a relational database composed of tables related to books, authors, publishers, user ratings, and user reviews.

The tables allow the analysis of information such as:

* Published books.
* Associated authors.
* Publishers.
* Average ratings.
* Text reviews.
* Users who rate and write reviews.

---

### Proceso / Process

🇪🇸

1. Exploración inicial del esquema de la base de datos.
2. Identificación de tablas, relaciones y llaves principales.
3. Traducción de requerimientos de negocio en consultas SQL.
4. Uso de filtros para segmentar información relevante.
5. Aplicación de joins para combinar datos entre tablas.
6. Uso de agregaciones para calcular métricas.
7. Agrupación de resultados por autores, editoriales, libros y usuarios.
8. Ordenamiento de resultados para identificar rankings y patrones.
9. Interpretación de los resultados desde una perspectiva de negocio.

🇬🇧

1. Initial exploration of the database schema.
2. Identification of tables, relationships, and primary keys.
3. Translation of business requirements into SQL queries.
4. Use of filters to segment relevant information.
5. Application of joins to combine data across tables.
6. Use of aggregations to calculate metrics.
7. Grouping results by authors, publishers, books, and users.
8. Ordering results to identify rankings and patterns.
9. Interpretation of results from a business perspective.

---

### Consultas y métricas desarrolladas / Queries and Metrics Developed

🇪🇸

* Conteo de libros publicados después de una fecha determinada.
* Identificación de editoriales con mayor número de publicaciones relevantes.
* Cálculo de calificaciones promedio por autor.
* Análisis de usuarios con mayor actividad en calificaciones y reseñas.
* Cálculo del promedio de reseñas para usuarios altamente activos.
* Uso de joins para conectar libros, autores, editoriales, ratings y reviews.

🇬🇧

* Count of books published after a specific date.
* Identification of publishers with the highest number of relevant publications.
* Calculation of average ratings by author.
* Analysis of users with the highest rating and review activity.
* Calculation of average reviews for highly active users.
* Use of joins to connect books, authors, publishers, ratings, and reviews.

---

### Insights clave / Key Insights

🇪🇸

* SQL permite responder preguntas de negocio directamente desde una base de datos relacional sin depender únicamente de archivos planos.
* Los joins son fundamentales para conectar entidades como libros, autores, editoriales y usuarios.
* Las agregaciones permiten construir KPIs útiles, como conteos, promedios y rankings.
* El análisis SQL facilita identificar autores, editoriales y usuarios con mayor relevancia dentro del conjunto de datos.

🇬🇧

* SQL makes it possible to answer business questions directly from a relational database without relying only on flat files.
* Joins are essential to connect entities such as books, authors, publishers, and users.
* Aggregations make it possible to build useful KPIs such as counts, averages, and rankings.
* SQL analysis helps identify authors, publishers, and users with higher relevance within the dataset.

---

### Recomendación / Recommendation

🇪🇸
En un contexto laboral real, este tipo de análisis podría utilizarse para construir reportes automatizados, monitorear desempeño editorial, identificar usuarios valiosos, evaluar catálogos de contenido y apoyar decisiones comerciales basadas en datos almacenados en bases relacionales.

🇬🇧
In a real business context, this type of analysis could be used to build automated reports, monitor publishing performance, identify valuable users, evaluate content catalogs, and support commercial decisions based on data stored in relational databases.

---

### Entregables / Deliverables

* Notebook SQL / SQL notebook: [proyecto final entrega SQL.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/proyecto%20final%20entrega%20SQL.ipynb)
* Notebook SQL revisado / Revised SQL notebook: [entrega de proyecto final sql- version revisada.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/entrega%20de%20proyecto%20final%20sql-%20version%20revisada.ipynb)
* Base de datos relacional / Relational database
* Consultas SQL / SQL queries
* Respuestas a requerimientos de negocio / Business requirement answers

## Entregables principales / Main Deliverables

🇪🇸
Este repositorio incluye notebooks, presentación, gráficas exportadas y datasets organizados según cada caso de análisis.

🇬🇧
This repository includes notebooks, a presentation, exported charts, and datasets organized according to each analysis case.

* 📓 **Notebook principal — Analítica operativa / Main notebook — Operational Analytics:**
  [Proyecto final merged/Proyecto_Final_Bootcamp_data_analitics.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/Proyecto%20final%20merged/Proyecto_Final_Bootcamp_data_analitics.ipynb)

* 🧪 **Notebook y datasets — Prueba A/B / Notebook and datasets — A/B Testing:**
  [Test AB/](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/Test%20AB)

* 🗄️ **Notebooks SQL / SQL notebooks:**
  [proyecto final entrega SQL.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/proyecto%20final%20entrega%20SQL.ipynb)  
  [entrega de proyecto final sql- version revisada.ipynb](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/entrega%20de%20proyecto%20final%20sql-%20version%20revisada.ipynb)

* 🎞️ **Presentación final / Final presentation:**
  [presentacion proyecto Final telecomunicaciones.pdf](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/blob/main/presentacion%20proyecto%20Final%20telecomunicaciones.pdf)

* 📈 **Gráficas exportadas / Exported charts:**
  [graficas_pdf/](https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-/tree/main/graficas_pdf)

---

## Estructura del repositorio / Repository Structure

```text
Proyecto-Final-Analitica-Operativa-A-B-Testing-SQL/
├── Proyecto final merged/
│   └── Proyecto_Final_Bootcamp_data_analitics.ipynb
│
├── Test AB/
│   └── Notebooks and datasets for the A/B test
│
├── graficas_pdf/
│   └── Exported charts used in the final presentation
│
├── proyecto final entrega SQL.ipynb
├── entrega de proyecto final sql- version revisada.ipynb
├── presentacion proyecto Final telecomunicaciones.pdf
├── requirements.txt
└── README.md
```

🇪🇸
La estructura del repositorio separa los archivos según el tipo de análisis: analítica operativa, prueba A/B, SQL, presentación y visualizaciones exportadas.

🇬🇧
The repository structure separates the files by type of analysis: operational analytics, A/B testing, SQL, final presentation, and exported visualizations.

---

## Cómo ejecutar el proyecto localmente / How to Run Locally

### 1. Clonar el repositorio / Clone the repository

```bash
git clone https://github.com/deltafjp1/Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-.git
```

### 2. Entrar a la carpeta del proyecto / Enter the project folder

```bash
cd Proyecto-Final-Analtica-Operativa-A-B-Testing-SQL-Python-PostgreSQL-
```

### 3. Crear un entorno virtual / Create a virtual environment

#### Windows PowerShell

```bash
python -m venv .venv
.venv\Scripts\Activate.ps1
```

#### macOS / Linux

```bash
python -m venv .venv
source .venv/bin/activate
```

### 4. Instalar dependencias / Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Abrir Jupyter / Open Jupyter

```bash
jupyter lab
```

O también / Or:

```bash
jupyter notebook
```

### 6. Ejecutar los notebooks / Run the notebooks

🇪🇸
Puedes comenzar por el notebook principal de analítica operativa:

```text
Proyecto final merged/Proyecto_Final_Bootcamp_data_analitics.ipynb
```

Luego puedes revisar los notebooks correspondientes a la prueba A/B y al análisis SQL.

🇬🇧
You can start with the main operational analytics notebook:

```text
Proyecto final merged/Proyecto_Final_Bootcamp_data_analitics.ipynb
```

Then you can review the notebooks related to the A/B test and the SQL analysis.

---

## Notas / Notes

🇪🇸

* Los tres casos de uso son independientes.
* Cada carpeta o notebook corresponde a un análisis distinto.
* Los datasets de cada caso no están relacionados entre sí.
* El proyecto está orientado a demostrar habilidades de análisis de datos aplicadas a problemas de negocio.
* Algunas rutas y nombres de archivo conservan la estructura original del proyecto académico.

🇬🇧

* The three case studies are independent.
* Each folder or notebook corresponds to a different analysis.
* The datasets from each case are not related to each other.
* The project is designed to demonstrate data analysis skills applied to business problems.
* Some paths and file names preserve the original academic project structure.
