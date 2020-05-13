# Proyecto Big Data 
Proyecto de la materia Tópicos en Telemática sobre el analisis de grandes cantidades de datos referentes a los casos de Covid-19 presentes en Colombia y en el mundo.

Cada carpeta contiene el notebook de Jupyter y su respectiva vista en HTML, para verla solo descargue el archivo y ábralo en su navegador.
Cada notebook puede ser ejecutado desde Jupyter con Kernel Spark.

**Tecnologías:** Python, Spark, Jupyter.

**Infraestructura**: Cluster EMR y Buckets S3 - Amazon Web Services.

## 1. Búsqueda de datasets
- Datos globales sobre el Covid 19 (3 archivos): https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases
- Casos nacionales de Covid-19 en Colombia (1 archivo): https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases
- Cifras diarias reportadas por el Ministerio de Salud  (1 archivo): http://datosabiertos.esri.co/datasets/782122624f364fbdbd7e287b96c4a358_6?page=7

## 2. Almacenamiento de datos

**Bucket S3:** bigdatacovid

Para acceder  los datos utilice la ruta: bigdatacovid.s3.amazonaws.com/<Global|Colombia>/<nombre_archivo>.csv

Por ejemplo: https://bigdatacovid.s3.amazonaws.com/Global/confirmed_narrow.csv

En la carpeta Datalake se encuentran los screeshhots de los datos existentes en S3.

## 3. Análisis exploratorio de datos

- **Situación Colombia:** Se analizaron los datos para obtener información relevante sobre ellos tales como: Situación actual colombiana, distribución geofráfica de los infectados y centros de contagio, estado y procedencia de los infectados actuales, casos por sexo y curva de casos confirmados, recuperados y muertos.

- **Situación Global:** Con los datos obetenidos a nivel mundial se lograron determinar los países con más y menos casos activos, recuperado y muertos, así como las curvas de crecimiento y crifras actuales de cada una de estas poblaciones en el tiempo.

- **Colombia vs El Mundo:** Una vez consolidados los datos a nivel mundial y a nivel Colombia se graficaron a la par para buscar una relación o patrón de comportamiento entre los datos que tenían en común ambos datasets: casos confirmados, recuperados y muertos.

## 4. Conclusiones

- **Situación Colombia:** De los datos examinados se puede evidenciar que el Covid-19 posee una alta tasa de recuperación frente a las muertes, con tasas del 24.3% contra un 4.12% de los 11.613 casos confirmados, de los cuales un 64.5% se encuentra en casa. Sin embargo, las cifras siguen siendo exponenciales a pesar de las medidas de aislamiento impuestas desde el mes de marzo, pasando de 100-200 casos diarios a cerca de 600 en aproxmadamente un mes y afectando ciudades capitales y con pocas restricciones sanitarias como lo son Bogotá, Cali, Villavicencio, Cartagena y Leticia. Estas cifras evidencian y justifican la emergencia sanitaria que atraviesa el país y las medidas drásticas que se han tenido en cuenta para frenar esta pandemia y evitar un colapso del frágil sistema de salud colombiano.

- **Situación Global:** Tras realizar el análisis de los datos tomados, se puede evidenciar que a pesar de que la tasa de contagios es muy alta en la mayoría de los países, es común que hayan menos casos de muertes en comparación a los recuperados. Se encontró que la tasa de muertes por Covid-19 es del 6.88% mientras que la de recuperados es del 34.82%. Además, en las gráficas presentadas se puede ver que la propagación del virus aún va en aumento exponencial y no se ha llegado al pico máximo de la curva, el cual es el momento en el que comienzan a disminuír los nuevos casos.

- **Colombia vs El Mundo:** Comparando las cifras mundiales de casos confirmados, muertes y recuperados es evidente que Colombia sigue el mismo comportamiento exponencial que el resto del mundo, en las gráficas de casos confirmados y recuperados las cifras difieren unicamente en la magnitud de la población tomada en cuenta, y la gráfica de muertes colombiana se acerca a la mundial pero conserva una mayor mesura. Este mismo comportamiento se ha dado en múltiples países y es por esto indispensable que para poder aplanar la curva de contagios cada gobierno aplique las medidas necesarias para disminuir sus contagios y muertes lo máximo posible.

