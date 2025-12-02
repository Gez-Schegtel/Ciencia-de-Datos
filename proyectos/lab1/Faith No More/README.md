# Faith No More – Data Cleaning & Preparation

Este repositorio contiene una **demostración práctica** y un conjunto de **ejercicios guiados** sobre **limpieza y preparación de datos** en Python, basados en el capítulo 7 *Data Cleaning and Preparation* del libro [*Python for Data Analysis* de Wes McKinney](https://wesmckinney.com/book/).

## Contenido

* 📓 **`demo_faith_no_more.ipynb`**
  Notebook de **demostración** en el que se aplican técnicas comunes de limpieza de datos utilizando **Pandas y Numpy**.

  * Dataset utilizado: **Titanic**, cargado directamente desde la librería `seaborn`.

* 📓 **`ejercicios_faith_no_more.ipynb`**
  Notebook con **7 ejercicios prácticos** diseñados para aplicar los conceptos de limpieza y preparación de datos.

  * Dataset utilizado: **Netflix Movies and TV Shows**, ubicado en:

    ```
    datasets/Alumnos/Equipo Faith No More/Netflix Movies and TV Shows/netflix_titles.csv
    ```
  * Ejercicios incluidos:

    1. **Relleno de valores faltantes** → Imputar valores vacíos en la columna `director`.
    2. **Normalización de texto** → Estandarizar nombres de países (`country`) en mayúsculas.
    3. **Conversión de fechas** → Transformar `date_added` a tipo `datetime` para análisis temporal.
    4. **Creación de variables derivadas** → Identificar si un título es un documental.
    5. **Creación de variables dummies** → Convertir la columna `type` (Movie/TV Show) en variables binarias.
    6. **Categorización explícita** → Definir `rating` como `Categorical` y explorar sus categorías.
    7. **Corrección de ratings** → Detectar y limpiar valores inválidos en la columna `rating`.

* 📄 **`requirements.txt`**
  Lista de dependencias necesarias para ejecutar los notebooks.

## Instalación de dependencias

Para instalar las librerías necesarias:

```bash
pip install -r requirements.txt
```

## Objetivo

El objetivo principal de este proyecto es **aprender y practicar técnicas de limpieza y preparación de datos** que resultan fundamentales antes de realizar análisis exploratorio o aplicar modelos de machine learning.
