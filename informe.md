# `Explorando los Hilos de la Conexión: Un Análisis de la Comunicación en Argentina`

Exploratory Data Analysis: Conectividad y Medios de Comunicación en Argentina

## Descripción del repositorio 
En primer lugar, vamos a describir el contenido de cada archivo en este repositorio. En la estructura inicial, encontramos dos carpetas principales. La primera, llamada "internet", contiene todos los datos relacionados con el análisis principal de este proyecto: información sobre el uso de Internet. La segunda carpeta se denomina "otros medios de comunicación" y contiene un conjunto de datos relevante sobre servicios de mensajería o correo postal, así como datos relacionados con las suscripciones de televisión. Cada conjunto de datos se organiza por año, que se divide en trimestres, y estos a su vez se desglosan por provincias, lo cual permite rastrear la evolución de los datos a lo largo del tiempo. En estas carpetas, encontrarás el archivo que contiene las transformaciones y el análisis de los datos. Por último, también está disponible el archivo README que estás leyendo, donde se brinda una breve explicación del análisis realizado y las conclusiones obtenidas.

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

## Resultados y Conclusiones

- Se observa que la provincia de Buenos Aires tiene la mayor cantidad de conexiones a Internet, seguida de otras provincias como Córdoba, Santa Fe y Mendoza.
- El cable módem es la tecnología más utilizada para acceder a Internet en la mayoría de las provincias, seguido de ADSL y fibra óptica.
- Se encuentra una distribución más frecuente de velocidades de conexión a Internet de media baja en comparación con velocidades de media alta.
- No se encuentra una correlación clara entre las suscripciones de televisión por provincia y las conexiones a Internet.
- A medida que pasan los años, se observa una disminución en la utilización de servicios postales en Argentina, sin una correlación significativa con las conexiones a Internet.

Estas conclusiones brindan una visión general de la situación de las comunicaciones en Argentina, destacando la importancia de las conexiones a Internet y la evolución de las tecnologías de conexión. Además, se evidencia una tendencia hacia la disminución en la utilización de servicios postales. Estos hallazgos pueden ser útiles para comprender el panorama de las comunicaciones en el país y tomar decisiones informadas en el ámbito de las telecomunicaciones.

## Requisitos de Instalación y Uso

- Python 3.5 o superior
- Librerías necesarias: pandas, numpy, matplotlib

## Instrucciones de Uso

1. Descargar los conjuntos de datos del sitio web del ENACOM.
2. Guardar los archivos CSV en la carpeta correspondiente en el proyecto.
3. Ejecutar el código del proyecto en un entorno de desarrollo Python compatible.
4. Seguir las instrucciones y comentarios en el código para realizar el análisis exploratorio de los datos.
