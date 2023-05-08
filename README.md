# ETL-process

Este proyecto tiene como objetivo realizar un análisis de datos climáticos y la gestión de pedidos de una empresa. Se han utilizado diversas herramientas y librerías de Python para el procesamiento y análisis de los datos.

Contenido
El proyecto cuenta con los siguientes archivos:

analisis_clima.ipynb: un notebook de Jupyter donde se encuentra todo el análisis de datos climáticos.
gestion_pedidos.ipynb: un notebook de Jupyter donde se encuentra toda la gestión de pedidos.
conexion_db.ipynb: un notebook de Jupyter donde se realiza la conexión con la base de datos y se insertan las tablas generadas por los notebooks anteriores.
data/: una carpeta que contiene los archivos CSV con los datos climáticos y de los pedidos.
README.md: este archivo que estás leyendo.
Análisis de datos climáticos
En el notebook analisis_clima.ipynb se realiza un análisis de los datos climáticos correspondientes a un mes de un año específico, que se encuentra en la carpeta data/. Los datos son leídos desde el archivo CSV y se convierten a un dataframe de Pandas para su posterior procesamiento. Entre las operaciones realizadas se encuentran:

Selección de columnas relevantes.
Cambio de nombre de columnas.
Conversión de tipos de datos.
Limpieza de valores nulos y de registros duplicados.
Conversión de fechas al formato adecuado.
Análisis de estadísticas descriptivas de los datos.
Visualización de datos mediante gráficas.
El resultado final es un dataframe limpio y procesado que se exporta a una tabla de una base de datos MySQL mediante la librería SQLAlquemy.

Gestión de pedidos
En el notebook gestion_pedidos.ipynb se realiza la gestión de los pedidos de una empresa. Los datos correspondientes a los pedidos se encuentran en un archivo CSV que se encuentra en la carpeta data/. Los datos son leídos desde el archivo CSV y se convierten a un dataframe de Pandas para su posterior procesamiento. Entre las operaciones realizadas se encuentran:

Selección de columnas relevantes.
Cambio de nombre de columnas.
Conversión de tipos de datos.
Limpieza de valores nulos y de registros duplicados.
Agregación de los datos por fecha y país.
Análisis de estadísticas descriptivas de los datos.
Visualización de datos mediante gráficas.
El resultado final es un dataframe limpio y procesado que se exporta a una tabla de una base de datos MySQL mediante la librería SQLAlquemy.

Conexión con la base de datos
En el notebook conexion_db.ipynb se realiza la conexión con una base de datos MySQL y se insertan las tablas generadas por los notebooks anteriores. La conexión se realiza mediante la librería SQLAlquemy.

Para poder ejecutar el código de este notebook es necesario contar con una instancia de MySQL Workbench en la que se cree la base de datos correspondiente.

Conclusiones
Este proyecto muestra el uso de diversas herramientas y librerías de Python para el análisis de datos y la gestión de bases de datos MySQL. Además, se dem