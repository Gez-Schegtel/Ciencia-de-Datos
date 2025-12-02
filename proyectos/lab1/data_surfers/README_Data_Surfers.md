# Data Surfers — Análisis de Ventas Adidas 📊

**Duración sugerida:** 45–60 min  
**Dataset:** Adidas Sales (Kaggle) - Análisis real de ~9,641 transacciones

## 🎯 Objetivos
- Aprender fundamentos de Python para ciencia de datos
- Dominar NumPy para análisis numérico eficiente  
- Explorar pandas para manipulación de DataFrames
- Aplicar técnicas de EDA (Exploratory Data Analysis) en datos reales

## ⏰ Timeline
- 00:00–05:00 — Contexto, objetivos, setup Jupyter
- 05:00–25:00 — *Notebook principal* (`data_surfers_mini_notebook.ipynb`)
- 25:00–35:00 — *Desafío rápido* (`desafio_corto.ipynb`) 
- 35:00–45:00 — Discusión de resultados y Q&A
- Cierre — Recap + próximos pasos

## 📁 Archivos del Proyecto
- **Notebook principal**: `data_surfers_mini_notebook.ipynb` - Análisis completo con NumPy y pandas
- **Desafío rápido**: `desafio_corto.ipynb` - Ejercicios prácticos (10 min)
- **Dataset**: `adidas_sales_kaggle.csv` - Datos reales de ventas Adidas
- **Dependencias**: `requirements.txt` - Librerías necesarias
- **Documentación**: Este README

## 📊 Dataset: Adidas Sales
- **Fuente**: [Kaggle](https://www.kaggle.com/datasets/ahmedabbas757/dataset)
- **Tamaño**: 9,641 transacciones de ventas
- **Columnas clave**:
  - `Retailer`: Tienda/canal de venta
  - `Product`: Producto vendido
  - `Total Sales`: Ventas totales en USD
  - `Operating Profit`: Ganancia operativa
  - `Region`: Región geográfica
  - `Sales Method`: Online/In-store/Outlet

## 🛠️ Requisitos Técnicos
```bash
# Instalar dependencias
pip install -r requirements.txt

# Ejecutar notebook principal
jupyter notebook data_surfers_mini_notebook.ipynb
```

**Librerías principales:**
- `numpy` - Análisis numérico y arrays
- `pandas` - DataFrames y manipulación de datos  
- `matplotlib` - Visualizaciones
- `jupyter` - Entorno interactivo

## 🚀 Contenido de los Notebooks

### 1. Notebook Principal (`data_surfers_mini_notebook.ipynb`)
**Secciones 1-5: Fundamentos Python**
- IPython/Jupyter tips y magics
- Estructuras de datos (listas, diccionarios, sets)
- Funciones y manejo de archivos
- Análisis CSV sin pandas

**Sección 6: NumPy**
- Arrays multidimensionales
- Operaciones vectorizadas
- Análisis estadístico eficiente
- Aplicación en datos de Adidas

**Sección 7: Pandas**
- DataFrames y exploración de datos
- Filtrado y agregaciones
- Análisis temporal
- Visualizaciones integradas

### 2. Desafío Rápido (`desafio_corto.ipynb`)
**Ejercicios prácticos (10 min):**
1. Exploración básica de datos
2. Cálculo de venta promedio
3. Top retailer por transacciones
4. Top producto por ventas
5. Función `top_k_productos()` personalizada

## 💡 Tips de Facilitación
- **Ejecución incremental**: Ejecutar celdas paso a paso
- **Pair programming**: Fomentar trabajo en duplas
- **Datos reales**: Enfatizar limpieza y validación de datos
- **Comparaciones**: Mostrar diferencias entre métodos manuales vs pandas
- **Visualización**: Destacar la importancia de gráficos claros

## 🏆 Resultados Esperados
Al finalizar, los estudiantes podrán:
- ✅ Cargar y limpiar datos CSV con Python
- ✅ Realizar análisis exploratorio básico
- ✅ Usar NumPy para cálculos eficientes
- ✅ Aplicar pandas para análisis de datos
- ✅ Crear visualizaciones informativas
- ✅ Implementar funciones reutilizables

## 👥 Equipo Data Surfers
*Presentación preparada para Ciencia de Datos - UTN*

¡Éxitos y a surfear datos! 🏄‍♂️🌊
