# `Explorando los Hilos de la Conexión: Un Análisis de la Comunicación en Argentina`

Exploratory Data Analysis: Conectividad y Medios de Comunicación en Argentina

<p align='center'>
<img src ="https://media1.giphy.com/media/xTiTnxpQ3ghPiB2Hp6/giphy.gif?cid=ecf05e47fyek0ystm0tff44j0f2pqb86wxqydww3yiuntayv&ep=v1_gifs_search&rid=giphy.gif&ct=g" height=250>
<p>


## Repositorio de Proyecto: Análisis de Conectividad e Infraestructura de Comunicaciones

Este repositorio contiene datos y análisis relacionados con la conectividad a Internet y otros medios de comunicación. A continuación, se describe la estructura de las carpetas y archivos disponibles:

### Carpeta "Internet"

En esta carpeta, encontrarás diversos archivos CSV que contienen información detallada sobre la conectividad a Internet en diferentes provincias. Los datos incluyen la velocidad de Internet, el tipo de tecnología utilizada para las conexiones y el desglose de los tipos de conexiones utilizadas. El archivo "datos_internet.csv" reúne todos estos datos en un único archivo.

### Carpeta "Otros medios de comunicación"

Dentro de esta carpeta, se encuentran datos relacionados con las suscripciones a servicios de televisión y los servicios postales utilizados en cada provincia.

### Carpeta "KPI"

Dentro de esta carpeta, se encuentran datos relacionados Con los elementos restantes de la elaboración y análisis de los KPI

### Notebooks de Análisis

En la carpeta principal del repositorio, se encuentran los archivos de "notebooks" que contienen el proceso de Extracción, Transformación y Carga (ETL) de los datos, así como el Análisis Exploratorio de Datos (EDA). Estos notebooks contienen el flujo de trabajo seguido y se presentan algunas conclusiones basadas en los hallazgos realizados.

### Archivo "README"

El archivo README proporciona una descripción general del proyecto, la estructura del repositorio y las instrucciones de uso. También se explica el propósito e interés del proyecto, así como cualquier información relevante para el lector.

¡No dudes en explorar los datos y utilizar el código proporcionado para realizar análisis adicionales!

Si tienes alguna pregunta o necesitas más información, no dudes en contactarme. ¡Disfruta del proyecto!

## Descripción del Proyecto

Este proyecto tiene como objetivo analizar la conectividad a Internet, las suscripciones de televisión y los servicios postales en cada provincia de Argentina. Se realiza un análisis exploratorio de los datos obtenidos del Ente Nacional de Comunicaciones de Argentina (ENACOM) para comprender la situación de las comunicaciones en el país.
La página de donde se obtuvieron los datos es: 

https://datosabiertos.enacom.gob.ar/home

## Conjuntos de Datos Utilizados

- `historico_velocidad_internet.csv`: Contiene información sobre la velocidad media de bajada de Internet por provincia.
- `Internet_Accesos-por-tecnologia.csv`: Proporciona datos sobre la utilización de diferentes tecnologías de conexión a Internet según la provincia.
- `Internet_BAF.csv`: Contiene información sobre el acceso a Internet mediante banda ancha fija o dial-up por provincia.
- `servicios_postales_provincias_personal.csv`: Contiene datos sobre la adquisición de servicios postales por provincia.
- `Television.csv`: Proporciona información sobre los accesos a televisión por suscripción por provincia.

## Estructura del Proyecto

El proyecto se divide en las siguientes secciones:

1. Importación de librerías y carga de los conjuntos de datos.
2. Análisis individual de cada conjunto de datos:
   - Verificación de la información básica, detección de datos nulos y eliminación de columnas innecesarias.
   - Comprobación de la consistencia y coherencia de los datos.
   - Conversión de tipos de datos y limpieza de los valores.
   - Creación de visualizaciones para comprender mejor los datos.
3. Unión de los conjuntos de datos relacionados y creación de un nuevo dataset.
4. Conclusiones obtenidas a partir del análisis exploratorio de los datos.
5. Creación de un informe README para describir el proyecto y sus resultados.

## Resultados y Conclusiones del EDA

- Se observa que la provincia de Buenos Aires tiene la mayor cantidad de conexiones a Internet, seguida de otras provincias como Córdoba, Santa Fe y Mendoza.
- El cable módem es la tecnología más utilizada para acceder a Internet en la mayoría de las provincias, seguido de ADSL y fibra óptica.
- Se encuentra una distribución más frecuente de velocidades de conexión a Internet de media baja en comparación con velocidades de media alta.
- No se encuentra una correlación clara entre las suscripciones de televisión por provincia y las conexiones a Internet.
- A medida que pasan los años, se observa una disminución en la utilización de servicios postales en Argentina, sin una correlación significativa con las conexiones a Internet.

- Existe una posible relación entre la infraestructura telefónica y la disminución en la utilización de las tecnologías de conexión Dial Up y DSL. A medida que avanza el tiempo, se observa una tendencia decreciente en la utilización de estas tecnologías más antiguas. Esto puede deberse a una mejora en la infraestructura de telecomunicaciones, como la expansión de redes de fibra óptica y el despliegue de tecnologías más modernas. La disponibilidad de conexiones de mayor velocidad, como el cable módem y la fibra óptica, puede haber llevado a una disminución en la demanda de tecnologías más lentas y menos eficientes como Dial Up y DSL.

Estas conclusiones brindan una visión general de la situación de las comunicaciones en Argentina, destacando la importancia de las conexiones a Internet y la evolución de las tecnologías de conexión. Además, se evidencia una tendencia hacia la disminución en la utilización de servicios postales. Estos hallazgos pueden ser útiles para comprender el panorama de las comunicaciones en el país y tomar decisiones informadas en el ámbito de las telecomunicaciones.

## KPIs

## KPI 1: Crecimiento Porcentual de Conexiones de Internet

**Objetivo:** Evaluar el crecimiento o decrecimiento en porcentaje de las conexiones de internet por año.

**Fórmula:** (Valor actual - Valor anterior) / Valor anterior * 100.

**Conclusiones del KPI:** En cuanto a las conexiones de internet, podemos observar un patrón de crecimiento constante en los años anteriores. Los valores muestran un crecimiento positivo año tras año, lo cual indica un incremento de las conexiones a internet en comparación con el año anterior.

Recordemos que el año 2022 solo llega hasta el tercer trimestre, por lo que la falta de los datos del cuarto trimestre afecta el comportamiento de dicha variable.

Este caso no se repite con los otros datos referentes a televisión y servicios postales. En cuanto a la televisión, podemos observar que si bien tiene un crecimiento en números positivos, este es menor al de internet e incluso llega al punto en donde su crecimiento deja de ser mayor a los años anteriores. Se mantiene en parámetros similares, observando estabilidad.

Por otra parte, los servicios postales muestran constantemente una disminución e incluso sus porcentajes se evidencian en números negativos, lo que quiere decir que los servicios postales utilizados año tras año son menores que en el año anterior.

## KPI 2: Distribución de Tipos de Conexión de Internet

**Objetivo:** Medir el porcentaje de conexiones de internet de un tipo específico en relación con el total de conexiones anuales.

**Fórmula:** (Número de conexiones de un tipo específico / Total de conexiones anual) * 100.

**Conclusiones del KPI:** Al analizar el KPI de Distribución de tipos de conexión, se evidencia claramente que el tipo de conexión de banda ancha fija predomina frente al tipo de conexión dial-up. Además, se observa un crecimiento constante de la banda ancha fija en comparación con la conexión dial-up, lo que indica una clara preferencia por conexiones más rápidas y estables.

Esta conclusión es válida y respalda la idea de que la distribución de tipos de conexiones no es uniforme, ya que hay una clara diferencia en la utilización de diferentes tecnologías de conexión. La creciente preferencia por la banda ancha fija y la disminución del uso de la conexión dial-up son tendencias que muestran una evolución hacia conexiones más eficientes y avanzadas.

## KPI 3: Penetración de Banda Ancha Fija

**Objetivo:** Analizar cómo la conexión de banda ancha fija ha penetrado en relación con la población de cada provincia.

**Fórmula:** (Número de usuarios con banda ancha fija en una provincia / Total de habitantes en la provincia) * 100.

**Conclusiones del KPI:** En este KPI, podemos observar cómo la penetración de la conexión banda ancha, por lo general, está por encima del 50% en cada una de las provincias. Considerando que no están los datos completos, puesto que falta los datos que corresponden al cuarto trimestre, nos da a inferir que el crecimiento de la utilización de dicha conexión va en aumento.
