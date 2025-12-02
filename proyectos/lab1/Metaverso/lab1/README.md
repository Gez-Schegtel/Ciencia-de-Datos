# MetaVerso — Capitulo 11

**Duración sugerida:** 20 min

## Timeline
- 00:00–05:00 — Contexto, objetivos, presentacion del tema
- 05:00–10:00 — *Mini‑notebook demostrativo* (`NotebookDemo.ipynb`)
- 10:00–20:00 — *Ejercicios guiados* (`ejercicios_metaverso_cap11.ipynb`)

## Como ejecutar
- Instalar python (3.11 o 3.12) 👉 https://www.python.org/downloads/ || Ejecutá el instalador y tildá la opción "Add Python to PATH" ✅ antes de darle a Install Now.
- Instalar Jupyter Notebook(en consola):  `pip install notebook`
- Instalar Librerias(en consola):  `pip install pandas numpy matplotlib seaborn`

## Archivos
- Demo: `NotebookDemo.ipynb`
- Ejercicios guiados: `ejercicios_metaverso_cap11.ipynb`
- Datasets: `COVID-19 Dataset`: Un conjunto de datos de Kaggle con información sobre la pandemia de COVID-19 a nivel mundial.
  `full_grouped.csv` (principal), `covid_19_clean_complete.csv`

## Requisitos
- Python 3.10+
- Jupyter Notebook (o Google Colab)
- Bibliotecas: pandas, numpy, matplotlib, seaborn

## Objetivos y tips
- Enfocar en el Índice: Destacar repetidamente que la clave del análisis de series temporales en pandas es que la columna de fechas sea el índice del DataFrame.
- Fomentar la Exploración: Animar a los participantes a cambiar los parámetros de las funciones (window en .rolling(), la frecuencia en .resample()) para ver cómo afectan los resultados.
