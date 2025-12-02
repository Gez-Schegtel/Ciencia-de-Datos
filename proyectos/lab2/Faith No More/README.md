# Tarea: Visualización de Múltiples Distribuciones

Este repositorio contiene una demostración práctica de los conceptos del **Capítulo 9: "Visualizing Many Distributions at Once"**. El proyecto analiza por qué algunas técnicas de visualización son superiores a otras al comparar múltiples distribuciones de datos.

## 📂 Archivos del Proyecto

-   **[📖 Jupyter Notebook](https://github.com/mminoli/cd2025/blob/faith_no_more/proyectos/lab2/Faith%20No%20More/cap9_faith_no_more.ipynb):** Contiene todo el código, el análisis y las visualizaciones.
-   **[📊 Presentación (PDF)](https://github.com/mminoli/cd2025/blob/faith_no_more/proyectos/lab2/Faith%20No%20More/Visualizacion-de-multiples-distribuciones.pdf):** Un resumen visual de los conceptos y resultados clave.
-   **[📦 requirements.txt](https://github.com/mminoli/cd2025/blob/faith_no_more/proyectos/lab2/Faith%20No%20More/requirements.txt):** Archivo con las dependencias de Python necesarias para replicar el entorno.
-   **[📘 Libro de Referencia (PDF)](https://github.com/mminoli/cd2025/blob/faith_no_more/material/Unidad%203%20-%20Visualizaci%C3%B3n%20y%20an%C3%A1lisis%20exploratorio%20de%20datos/Wilke%20-%20Fundamentals%20of%20Data%20Visualization.pdf):** El capítulo 9 del libro de Claus O. Wilke que sirve de base teórica para este trabajo.

---

## 💡 Conceptos Clave Demostrados

El notebook realiza una demostración a partir de los conceptos clave del capítulo 9 del libro (como el uso de _boxplots_, _violin plots_, _sina plots_, etc.), incluyendo ejemplos de gráficos: uno incorrecto, uno malo, uno feo y, finalmente, el correcto.

## 🚀 Instalación y Uso

Para ejecutar este notebook en tu máquina local, sigue estos pasos.

### Prerrequisitos

-   Python 3.8 o superior
-   Git

### Pasos

1.  **Clona el repositorio:**
    ```bash
    git clone https://github.com/mminoli/cd2025.git
    cd cd2025/proyectos/lab2/Faith\ No\ More/
    ```

2.  **Crea y activa un entorno virtual (Recomendado):**
    -   En macOS/Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    -   En Windows:
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```

3.  **Instala las dependencias:**
    El archivo [`requirements.txt`](https://github.com/mminoli/cd2025/blob/faith_no_more/proyectos/lab2/Faith%20No%20More/requirements.txt) contiene todas las librerías necesarias.
    ```bash
    pip install -r requirements.txt
    ```
    > **Nota sobre `ipykernel`**: Esta librería se incluye para asegurar que Jupyter Lab reconozca y utilice correctamente el Python y las librerías de este entorno virtual. Es el "motor" que conecta tu `venv` con el notebook.

4.  **Inicia Jupyter Lab:**
    ```bash
    jupyter lab
    ```
    Esto abrirá una nueva pestaña en tu navegador. Desde allí, simplemente abre el archivo `cap9_faith_no_more.ipynb` para ver y ejecutar el código.

    Alternativamente, podés usar también `jupyter notebook` con el siguiente comando:

    ```
    jupyter notebook

    ```

## 📄 Fuente de Datos

Los datos utilizados provienen del dataset [ **"tips"** ](https://www.kaggle.com/datasets/ranjeetjain3/seaborn-tips-dataset), que está incluido por defecto en la librería de visualización de Python [ **seaborn** ](https://seaborn.pydata.org/).
