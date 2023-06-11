El Consejo Nacional de Población (CONAPO) del gobierno mexicano, realiza cada 5 años un análisis sobre un estudio multidimensional de la pobreza y establece un índice de marginación.

En https://www.gob.mx/cms/uploads/attachment/file/685354/Nota_te_cnica_IMEyM_2020.pdf se puede consultar el documento de como se calculó el índice para la encuesta del 2020. El índice, por municipio, se puede consultar en :

https://www.gob.mx/conapo/documentos/indices-de-marginacion-2020-284372

Junto con los indicadores más importantes para la medición multidimensional de la pobreza.

Para este proyecto te pedimos lo siguiente:

1. Un repositorio en github para el proyecto. El repositorio deberá llevar un archivo readme.md en el que se explique lo que se hace y los archivos de código, pero no la base de datos. 
2. En el archivo (o los archivos) de jupyter realiza lo siguiente:
  * Descargar y Leer el archivo de Base de Datos por Municipio 2020 del índice de marginación desde la página de descargas del gobierno federal mexicano en un dataframe. Los datos se encuentran en la pestaña "IMM 2020".
  * Mostrar la descripción del DataFrame (medias, máximos mínimos, etc...) mostrart algunos hallazgos interesantes de la simple inspección visual y por estadísticas básicas de los datos.
  * Realizar una gráfica que permita ver el porcentaje de municipios por estado con índices de marginación "muy bajo", "bajo", "medio", "alto" y "muy alto". Guarda la gráfica en archivo png
  * Realizar una gráfica que muestre el porcentaje de la población, respecto a la población total de cada estado, con índices de marginación "muy bajo", "bajo", "medio", "alto" y "muy alto". Guarda la gráfica en formato jpg
  * ¿Hay coincidencias entra la gráficas anteriores?  ¿Algún hallazgo? Comenta tu análisis.
  * Grafica la relación de porcentaje de analfabetismo respecto al porcentaje de poblaciones en localidades de menos de 5,000 habitantes.
  * ¿Existe una relación? ¿Cómo podrías analizar con que variable tiene mñas corelación el porcentaje de analfabetismo en personas mayores de 15 años?
  * Desarrolla un nuevo DataFrame con indicadores interesantes por estado que se obtengan de los datos a nivel municipal y que pudieran ser de importancia a la hora de definir políticas públicas. Se va a calificar la originalidad de los indicadores. Justifica las decisiones que tomes, y guarda el nuevo dataframe en formato parquet
