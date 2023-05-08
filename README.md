# 🔀 **ETL-process**

![portada](https://github.com/dapafer/ETL-process/blob/main/images/ETL_process.png)

Este proyecto tiene como objetivo realizar un proceso ETL (Extracción-Transformación-Carga). Se realizará un proceso de análisis de datos correspondiente a las fuentes obtenidas. Se han utilizado diversas herramientas y librerías de Python para el procesamiento y análisis.

---
## 📉 **Contenido.**
El proyecto cuenta con los siguientes archivos principales:

- `mercadona_data_scraping.ipynb`: un notebook de Jupyter donde se encuentra todo el proceso de "web scraping", a través de `Selenium`.
- `mercadona_data_transform.ipynb`: notebook donde se realiza el proceso de limpieza y transformación de los datos obtenidos, realizado con `Pandas`.
- `fruits_data_size_transform.ipynb`: limpieza y transformación del archivo "CSV" obtenido de un repositorio público.
- `AEMET_data_API.ipynb`: gestión de los datos obtenidos a través de peticiones realizadas a la `API` de "AEMET".
- `data_to_SQL.ipynb`: un notebook donde se realiza la conexión con la base de datos y se insertan las tablas generadas por los notebooks anteriores.

---
## 📊 **Análisis de datos.**
En el proceso, se realiza una extraccíon, y posterior análisis de datos obtenidos a través de diferentes fuentes de información. Los datos son leídos desde la web, archivo "CSV" y API. Se convierten a un dataframe a traves de Pandas para su posterior procesamiento. Entre las operaciones realizadas se encuentran:

- Selección de columnas relevantes.
- Cambio de nombre de columnas.
- Conversión de tipos de datos.
- Limpieza de valores nulos y de registros duplicados.
- Conversión de fechas al formato adecuado.

El resultado final son dataframes limpios y procesados, que se exportan a tablas de una base de datos MySQL mediante la librería SQLAlquemy.

---
## 🔄 **Conexión con la base de datos.**
En el notebook `data_to_SQL.ipynb` se realiza la conexión con una base de datos MySQL y se insertan las tablas generadas por los notebooks anteriores. La conexión se realiza mediante la librería `SQLAlquemy`.

Para poder ejecutar el código de este notebook es necesario contar con MySQL Workbench o similar en la que se cree la base de datos correspondiente.

---
## ❗️ **Resumen.**
Este proyecto muestra el uso de diversas herramientas y librerías de Python para el análisis de datos y la gestión de bases de datos MySQL. Además, se describe el proceso completo que se realiza en una situación similar.