Tutulo:  Análisis de precios de medicamentos en Colombia usando datos abiertos

Descripción del proyecto: 

El acceso equitativo a los medicamentos es un componente fundamental de la salud pública. En Colombia, los precios de los medicamentos pueden variar significativamente dependiendo de múltiples factores, lo que puede afectar la disponibilidad y el acceso por parte de la población. Este proyecto tiene como objetivo realizar un análisis exploratorio y estadístico de los precios de medicamentos en Colombia, utilizando datos abiertos oficiales, con el fin de identificar patrones, variabilidad de precios y posibles concentraciones de valores atípicos que puedan tener implicaciones en la gestión y regulación farmacéutica.

Preguntas de investigación:

¿Cuál es el comportamiento general de los precios de los medicamentos en Colombia?
¿Qué medicamentos presentan los precios promedio más altos?
¿Existe una alta dispersión en los precios de ciertos medicamentos?
¿Se observan valores atípicos que indiquen variabilidad significativa en el mercado farmacéutico?

Origen de los datos.
- Nombre del conjunto de datos: Precios de Medicamentos
- Plataforma: Datos Abiertos Colombia
- Entidad: Ministerio de Salud y Protección Social
- URL del dataset:https://www.datos.gov.co/Salud-y-Protecci-n-Social/Precios-Medicamentos/3t73-n4q9 
- Formato de consumo: JSON
- URL de extracción de datos:https://www.datos.gov.co/resource/3t73-n4q9.json
- Fecha de descarga: 18 de diciembre de 2025
  
Descripción del dataset: El conjunto de datos contiene información relacionada con los precios reportados de medicamentos en Colombia, incluyendo variables asociadas al producto farmacéutico y valores económicos que permiten realizar análisis estadísticos sobre su comportamiento en el mercado.

Metodología.
El desarrollo del proyecto se llevó a cabo siguiendo un enfoque de análisis de datos estructurado, utilizando herramientas de ciencia de datos en Python y datos abiertos oficiales de Colombia. La metodología se dividió en las siguientes etapas:

Carga de datos:
Los datos fueron obtenidos directamente desde la plataforma Datos Abiertos Colombia, consumiendo el conjunto de datos Precios de Medicamentos en formato JSON mediante su URL oficial. La carga se realizó utilizando la librería Pandas, transformando la información en un DataFrame para su análisis.

Exploración de datos:
Se realizó un análisis exploratorio inicial con el fin de comprender la estructura del dataset, identificar las variables disponibles, revisar los tipos de datos, evaluar la presencia de valores nulos y obtener estadísticas descriptivas preliminares. Esta etapa permitió detectar posibles inconsistencias y definir las acciones de limpieza necesarias.

Limpieza de datos (Pandas + NumPy).
El proceso de limpieza incluyó:
- Normalización de los nombres de las columnas.
- Conversión de la variable precio_por_tableta a formato numérico.
- Eliminación de registros con valores nulos en variables clave.
- Identificación y eliminación de valores atípicos mediante el método del rango intercuartílico (IQR).
- Filtrado de los datos relevantes para el análisis farmacéutico.
Las funciones de limpieza se documentaron para garantizar la reproducibilidad del proceso.

Análisis estadístico.
Se realizaron los siguientes análisis estadísticos descriptivos:
- Medidas de tendencia central: media, mediana y moda de los precios.
- Medidas de dispersión: varianza, desviación estándar y rango.
- Tablas de frecuencias para identificar medicamentos con mayor número de registros.
- Cálculo de porcentajes y proporciones sobre la distribución de precios.
- Análisis de correlación entre variables numéricas relevantes.

Visualizaciones.
Se generaron visualizaciones utilizando Matplotlib y Seaborn para facilitar la interpretación de los resultados, incluyendo gráficos de barras, boxplots y mapas de calor de correlación. Todas las visualizaciones cuentan con títulos y ejes rotulados para una presentación clara de la información.

Resultados y hallazgos principales.
El análisis evidenció una amplia variabilidad en los precios de los medicamentos, con presencia de valores atípicos que sugieren diferencias significativas entre productos. Algunos medicamentos presentan precios promedio considerablemente más altos, lo que podría tener implicaciones en el acceso y la regulación del mercado farmacéutico.
Asimismo, se identificaron patrones de concentración de precios y una dispersión notable en ciertos grupos de medicamentos.

Conclusiones.
- Se identificó una alta variabilidad en los precios de medicamentos en Colombia.
- La presencia de valores atípicos indica posibles diferencias en regulación, presentación o mercado.
- El dataset presenta limitaciones relacionadas con la falta de algunas variables clínicas o de consumo.
- Este análisis puede servir como base para estudios más profundos sobre acceso a medicamentos y políticas de control de precios.
- Futuras investigaciones podrían incorporar datos de consumo, regiones o EPS para ampliar el análisis.
