# PARTE 01: ANÁLISIS DE DATOS COVID-19 EN EL PERÚ
El presente proyecto tiene como objetivo analizar los datos masivos proporcionados por la [Plataforma Nacional de Datos Abiertos del MINSA](https://www.datosabiertos.gob.pe/). Entre los datos a analizar estan: [casos confirmados COVID-19](https://www.datosabiertos.gob.pe/dataset/casos-positivos-por-covid-19-ministerio-de-salud-minsa), [registro de fallecidos por COVID-19](https://www.datosabiertos.gob.pe/dataset/fallecidos-por-covid-19-ministerio-de-salud-minsa), [registro vacunación](https://www.datosabiertos.gob.pe/dataset/vacunaci%C3%B3n-contra-covid-19-ministerio-de-salud-minsa), entre otras.

### TECNOLOGÍAS Y HERRAMIENTAS EMPLEADAS:
#### ORALCE VIRTUALBOX:

<p align="center">
  <img src="https://th.bing.com/th/id/R.da15db6964f3d9d342d2640409acb815?rik=q%2bOWhHwrjenwfQ&pid=ImgRaw&r=0&sres=1&sresct=1"/>
</p>

#### PANDAS:

<p align="center">
  <img src="https://miro.medium.com/max/1620/1*b3P4rdrVHMIHbhQXnwRVew.jpeg"/>
</p>


#### PYSPARK:

<p align="center">
  <img src="https://www.staffworx.co.uk/wp-content/uploads/2021/07/pyspark-768x433.jpeg"/>
</p>

#### ORACLE DATABASE 19C:

<p align="center">
  <img src="https://1.bp.blogspot.com/-TpggTngsmGg/XpvB9il-51I/AAAAAAAAKfU/Ik-OV8eLhoQJjc5RTk_KWggsyan-pHYGACLcBGAsYHQ/s1600/19c_image.jpg"/>
</p>

#### ORACLE SQL DEVELOPER:

<p align="center">
  <img src="https://techgoeasy.com/wp-content/uploads/2016/07/oracle_sql_developer.png"/>
</p>

#### ORACLE SQL DEVELOPER DATA MODELER:

<p align="center">
  <img src="https://3.bp.blogspot.com/_JWosBXRVxhY/SmRTRCFsYBI/AAAAAAAADPY/0CjvoQOftVQ/s400/Oracle_sql_developer_data_modeler.jpg"/>
</p>

#### MICROSOFT POWER BI:

<p align="center">
  <img src="https://iexcel.in/wp-content/uploads/2020/05/Power-Bi-1-850x440.jpg"/>
</p>


#### VISUALIZACIÓN Y ANÁLISIS DE DATOS: POWER BI
Diseño de tableros para la eficaz visualización de los datos previamente procesados. Asimismo, la creación de indicadores a partir de funciones DAX para la óptima visualización de factores que puedan contribuir al desarrollo continuo de procesos que ayuden a detener la propagación del COVID-19 en el Perú.

- PANEL DE CONTROL CASOS POSITIVOS:

![DASHBOARD POSITIVOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/a72606c5-de21-476a-8c14-4f1d4c625c72)
  
- PANEL DE CONTROL REGISTROS DE VACUNACIÓN:

![DASHBOARD VACUNACION](https://github.com/Renzo1818/ETL-COVID/assets/93232895/8d0dcf45-d405-4520-8cab-d10d00935caf)

- PANEL DE CONTROL DE MORTALIDAD:

![DASHBOARD FALLECIDOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/46b41013-1648-48e3-83dd-b11ccb3e0211)


# PARTE 02: DATA PIPELINE Y ANALÍTICA COVID-19 EN EL PERÚ
El presente proyecto tiene como objetivo analizar los datos masivos proporcionados por la [Plataforma Nacional de Datos Abiertos del MINSA](https://www.datosabiertos.gob.pe/). Entre los datos a analizar estan: [casos confirmados COVID-19](https://www.datosabiertos.gob.pe/dataset/casos-positivos-por-covid-19-ministerio-de-salud-minsa), [registro de fallecidos por COVID-19](https://www.datosabiertos.gob.pe/dataset/fallecidos-por-covid-19-ministerio-de-salud-minsa), [registro vacunación](https://www.datosabiertos.gob.pe/dataset/vacunaci%C3%B3n-contra-covid-19-ministerio-de-salud-minsa), entre otras.


## ARQUITECTURA DE DATOS AZURE
<p align="center">
  <img src="https://learn.microsoft.com/de-de/azure/architecture/solution-ideas/media/azure-databricks-modern-analytics-architecture-diagram.png">
</p>

## IMPLEMENTACION DE SERVICIOS AZURE
#### AZURE DATA FACTORY: INGESTA Y ORQUESTADOR DE PROCESOS

![DATA FACTORY](https://github.com/Renzo1818/ETL-COVID/assets/93232895/c0d97bf2-3392-4559-9f67-66b198641445)

Creación de conjuntos de datos a partir de fuentes de datos On-Premises, extracción de estos mismos, invocación de notebooks de Databricks para la transformaciones necesarias y por último la carga masiva de datos a un Data Warehouse en Azure SQL Server.

#### AZURE DATA LAKE STORAGE

![DATA LAKE](https://github.com/Renzo1818/ETL-COVID/assets/93232895/4dc717f1-cfce-4638-baab-15ef79318cb1)

Diseño de un Data Lakehouse para almacenar los conjuntos de datos en su formato en bruto, datos semiprocesados y procesados para en consumo de otros servicios de Azure. Aplicación de la arquitectura de medallas: bronze, Silver y Gold para almacenar los datos por capa de calidad.

#### AZURE DATABRICKS
- ETL UBIGEO:

![DATABRICKS UBIGEO](https://github.com/Renzo1818/ETL-COVID/assets/93232895/35e12ec8-7cd6-48db-955e-08f7364bbe21)
  
- ETL CASOS POSITIVOS:

![DATABRICKS POSITIVOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/e1830078-9149-4fbb-9d56-9e3c17de4ea5)
  
- ETL FALLECIDOS:

![DATABRICKS FALLECIDOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/f617e037-6bb0-490e-86b4-cd6f0d978467)

- ETL VACUNACION:

![DATABRICKS VACUNACION](https://github.com/Renzo1818/ETL-COVID/assets/93232895/6d873022-133e-47af-8ef0-f996ce01dfc4)

#### AZURE SQL SERVER: DATA WAREHOUSE
- ESQUEMA DATA WARE HOUSE:

![DATA WAREHOUSE SCHEMA](https://github.com/Renzo1818/ETL-COVID/assets/93232895/a4973821-25fd-4cac-a795-5e4a06bd358d)
  
- ESQUEMA DATAMART CASOS POSITIVOS:

![DATAMART POSITIVOS SCHEMA](https://github.com/Renzo1818/ETL-COVID/assets/93232895/0a71a87d-5387-4482-901c-9782e824405e)
  
- ESQUEMA DATAMART FALLECIDOS:

![DATAMART FALLECIDOS SCHEMA](https://github.com/Renzo1818/ETL-COVID/assets/93232895/54059c6a-3546-4bed-b122-2353e162dcf1)
  
- ESQUEMA DATAMART VACUNACION:

![DATAMART VACUNACION SCHEMA](https://github.com/Renzo1818/ETL-COVID/assets/93232895/ff7fcbea-dc87-465b-8f1c-cb5952065cff)

#### VISUALIZACIÓN Y ANÁLISIS DE DATOS: POWER BI
Diseño de tableros para la eficaz visualización de los datos previamente procesados. Asimismo, la creación de indicadores a partir de funciones DAX para la óptima visualización de factores que puedan contribuir al desarrollo continuo de procesos que ayuden a detener la propagación del COVID-19 en el Perú.

- PANEL DE CONTROL CASOS POSITIVOS:

![DASHBOARD POSITIVOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/a72606c5-de21-476a-8c14-4f1d4c625c72)
  
- PANEL DE CONTROL REGISTROS DE VACUNACIÓN:

![DASHBOARD VACUNACION](https://github.com/Renzo1818/ETL-COVID/assets/93232895/8d0dcf45-d405-4520-8cab-d10d00935caf)

- PANEL DE CONTROL DE MORTALIDAD:

![DASHBOARD FALLECIDOS](https://github.com/Renzo1818/ETL-COVID/assets/93232895/46b41013-1648-48e3-83dd-b11ccb3e0211)
