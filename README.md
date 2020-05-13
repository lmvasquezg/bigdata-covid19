# Proyecto Big Data 
Proyecto de la materia Tópicos en Telemática sobre el analisis de grandes cantidades de datos referentes a los casos de Covid-19 presentes en Colombia y en el mundo.

Cada carpeta contiene le notebook de Jupyter y su respectiva vista en HTML, para verla solo descargue el archivo y ábralo en su navegador.
Cada notebook puede ser ejecutado desde Jupyter con Kernel Spark.

**Técnologías:** Python, Spark, Jupyter.
**Infraestructura**: Cluster EMR - Amazon Web Services.

1. Busqueda de datasets 
- Datos globales sobre el Covid 19 ( 3 archivos): https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases
- Casos nacionales de Covid-19 en Colombia (1 archivo): https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases
- Cifras diarias reportadas por el Ministerio de Salud  (1 archivo): 
http://datosabiertos.esri.co/datasets/782122624f364fbdbd7e287b96c4a358_6?page=7

2. Almacenamiento de datos

URL de bucket S3: http://bigdatacovid.s3-website-us-east-1.amazonaws.com/
