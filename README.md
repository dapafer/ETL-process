# 🔀**ETL-process**

![portada](https://github.com/dapafer/ETL-process/blob/main/images/ETL_process.png)

Este proyecto tiene como objetivo realizar un proceso ETL (Extracción-Transformación-Carga). Se realizará un proceso de análisis de datos correspondiente a las fuentes obtenidas. Se han utilizado diversas herramientas y librerías de Python para el procesamiento y análisis.

---
## 📉**Contenido.**
El proyecto cuenta con los siguientes archivos:

- analisis_clima.ipynb: un notebook de Jupyter donde se encuentra todo el análisis de datos climáticos.
gestion_pedidos.ipynb: un notebook de Jupyter donde se encuentra toda la gestión de pedidos.
conexion_db.ipynb: un notebook de Jupyter donde se realiza la conexión con la base de datos y se insertan las tablas generadas por los notebooks anteriores.
data/: una carpeta que contiene los archivos CSV con los datos climáticos y de los pedidos.
README.md: este archivo que estás leyendo.
Análisis de datos climáticos
En el notebook analisis_clima.ipynb se realiza un análisis de los datos climáticos correspondientes a un mes de un año específico, que se encuentra en la carpeta data/. Los datos son leídos desde el archivo CSV y se convierten a un dataframe de Pandas para su posterior procesamiento. Entre las operaciones realizadas se encuentran:

- Selección de columnas relevantes.
- Cambio de nombre de columnas.
- Conversión de tipos de datos.
- Limpieza de valores nulos y de registros duplicados.
- Conversión de fechas al formato adecuado.

El resultado final es un dataframe limpio y procesado que se exporta a una tabla de una base de datos MySQL mediante la librería SQLAlquemy.

---
## 🔄**Conexión con la base de datos.**
En el notebook `data_to_SQL.ipynb` se realiza la conexión con una base de datos MySQL y se insertan las tablas generadas por los notebooks anteriores. La conexión se realiza mediante la librería `SQLAlquemy`.

Para poder ejecutar el código de este notebook es necesario contar con MySQL Workbench o similar en la que se cree la base de datos correspondiente.

## ❗️**Resumen.**
Este proyecto muestra el uso de diversas herramientas y librerías de Python para el análisis de datos y la gestión de bases de datos MySQL. Además, se describe el proceso completo que se realiza en una situación similar.