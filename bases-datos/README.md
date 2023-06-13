## Aquí presentamos el proyecto de bases de datos

-Conectamos un cuaderno de Google Colab con una base de datos de Google CloudSQL en una manera eficiente y con toda la buena vibra de un notebook de jupyter
- Para esto haremos uso de un conector de Python SQL en la nube: para conectarnos a nuestras instancias de nuestra base de datos SQL en la nube sin tener que lidiar con certificados SSL y manualmente administrar lista de IP's permitidos.

## Requisitos:
- un proyecto de Google cloud existente


## parte 1: Crear una instancia de mysql en la nube de Googel y conectarnos a través de un cuaderno de Google colab.
ver [enlace](https://github.com/CuteLoop/MCD-Propedeutico/blob/main/bases-datos/mysql_python_connector.ipynb)

## parte 2: Importar un archivo de tipo csv a una base de datos SQL hospedada en la nube de google:
1. Crear proyecto de Google cloud y una instancia de una base de datos mysql en la nube
2. Crear una tabla de sql con el formato necesario para almacenar los datos a importar
3. Crear un bucket para almacenar el archivo csv con los datos y el código para crear la tabla .
4. Desde el dashboard de google importar primero *create_table.sq*l código para crear tabla seguido de importar el archivo csv *flights-table.csv*
5. Conectarse a la base de datos y verificar importación correcta.
