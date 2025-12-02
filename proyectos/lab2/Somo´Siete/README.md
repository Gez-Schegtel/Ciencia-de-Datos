# Laboratorio Capítulo 13 - Fundamentals of Data Visualization: Visualizing time series and other functions of an independent variable

### **Objetivos**

Este laboratorio tiene como objetivo explorar las **técnicas avanzadas de visualización de series temporales** basadas en el capítulo 13 de "Fundamentals of Data Visualization" de Claus O. Wilke. A través de ejercicios prácticos con datos reales de e-commerce y economía, aprenderemos:

- **Series temporales individuales**: Cómo contar historias con una sola variable a lo largo del tiempo
- **Múltiples series temporales**: Técnicas para comparar y contrastar varias métricas simultáneamente
- **Variables de respuesta múltiples**: Visualización de relaciones complejas entre dos o más variables
- **Connected scatter plots**: La técnica más avanzada para revelar dinámicas temporales ocultas
- **Buenas prácticas de visualización**: Do's y Don'ts para crear gráficos efectivos
- **Gradientes temporales**: Uso de color y opacidad para mostrar la dirección del tiempo

---

### **Cómo ejecutar**

#### 1. Crear entorno virtual
```bash
# Crear entorno virtual
python -m venv .venv

# Activar entorno virtual
# En Windows:
.venv\Scripts\activate
# En macOS/Linux:
source .venv/bin/activate
```

#### 2. Instalar dependencias
```bash
pip install -r requirements.txt
```

#### 3. Ejecutar el notebook
```bash
# Iniciar Jupyter desde la terminal
jupyter notebook

# O si prefieres Jupyter Lab
jupyter lab
```

Luego abre el archivo:
- `visualization_somo_siete_v0.ipynb` - Laboratorio completo de visualización de series temporales

---

### **Datasets utilizados**

#### **1. E-commerce Analysis UK Dataset**
- **Fuente**: [Kaggle - E-commerce Analysis UK](https://www.kaggle.com/datasets/atharvaarya25/e-commerce-analysis-uk)
- **Descripción**: Dataset de transacciones de comercio electrónico del Reino Unido
- **Características**:
  - **541,909 transacciones** de diciembre 2010 a diciembre 2011
  - **8 columnas**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
  - **Casos de uso**: Análisis de ventas mensuales, comportamiento por país, cálculo de revenue

#### **2. Monthly Inflation Rate UK Dataset**
- **Fuente**: [Kaggle - UK Inflation Data 1989-2022](https://www.kaggle.com/datasets/scarfsman/uk-inflation-data-1989-2022)
- **Descripción**: Datos mensuales de inflación del Reino Unido
- **Período**: 1989-2023
- **Formato**: Year, Month (JAN-DEC), Inflation (%)
- **Uso**: Comparación con revenue mensual para análisis de relaciones económicas

---

### **Estructura del proyecto**

```
SomoSiete/
├── README.md                           # Este archivo
├── requirements.txt                    # Dependencias del proyecto
├── visualization_somo_siete_v0.ipynb  # Notebook principal del laboratorio
├── viz_ejemplo.ipynb                  # Ejemplos de referencia
└── .venv/                             # Entorno virtual (creado localmente)
```

---

### **Contenido del laboratorio**

**Basado en el Capítulo 13 de "Fundamentals of Data Visualization" por Claus O. Wilke**

#### **Sección 1: Series Temporales Individuales**
- **Objetivo**: Mostrar la evolución de una sola variable a lo largo del tiempo
- **Técnicas exploradas**:
  1. **Puntos aislados (Mala práctica)**: Gráfico de dispersión sin conexión temporal
  2. **Puntos conectados**: Primer paso hacia la visualización correcta
  3. **Línea narrativa**: La forma canónica y efectiva
  4. **Énfasis en magnitud**: Gráfico de área para mostrar volumen
- **Dataset**: Ventas mensuales del e-commerce UK (2010-2011)
- **Conceptos clave**: Conexión temporal, ejes claros, etiquetas informativas

#### **Sección 2: Múltiples Series Temporales**
- **Objetivo**: Comparar la evolución de varias series simultáneamente
- **Técnicas exploradas**:
  1. **Puntos dispersos**: Visualización básica pero inefectiva
  2. **Líneas con marcadores**: Mejora visual pero puede ser ruidoso
  3. **Líneas limpias**: Comparación directa y clara
  4. **Etiquetas directas**: Técnica avanzada para evitar leyendas
- **Dataset**: Ventas por país (top 3 países excluyendo UK)
- **Conceptos clave**: Escalas compatibles, diferenciación visual, organización lógica

#### **Sección 3: Variables de Respuesta Múltiples**
- **Objetivo**: Revelar relaciones dinámicas entre dos variables a lo largo del tiempo
- **Técnicas exploradas**:
  1. **Gráficos separados**: Fácil lectura individual, difícil comparación
  2. **Connected scatter plot básico**: Muestra relación pero sin indicadores temporales
  3. **Gradiente de opacidad**: Indica dirección del tiempo con transparencia
  4. **Etiquetas temporales**: Puntos clave con fechas para máxima claridad
- **Dataset**: Revenue mensual vs Inflación UK (2010-2011)
- **Conceptos clave**: Flujo temporal, correlaciones dinámicas, indicadores visuales

---

### **Técnicas avanzadas implementadas**

#### **Gradientes Temporales**
```python
# Gradiente de opacidad para mostrar dirección del tiempo
alphas = np.linspace(0.3, 1.0, len(combined_data))
for i in range(len(combined_data)-1):
    plt.plot([x1, x2], [y1, y2], color='navy', alpha=alphas[i], linewidth=2)
```

#### **Formateo de Ejes**
```python
# Formatear ejes para valores monetarios
axes.yaxis.set_major_formatter(plt.FuncFormatter(lambda x, p: f'£{x/1e6:.1f}M'))
```

#### **Anotaciones Inteligentes**
```python
# Etiquetas en puntos clave con cajas de texto
plt.annotate(date, (x, y), xytext=(10, 10), 
             bbox=dict(boxstyle='round,pad=0.3', facecolor='white', alpha=0.8))
```

---

### **Principios de visualización aplicados**

#### **Do's (Qué SÍ hacer)**
- ✅ **Conectar puntos temporales**: La línea cuenta la historia
- ✅ **Indicar dirección del tiempo**: Gradientes, flechas o etiquetas
- ✅ **Usar escalas apropiadas**: Formateo claro para valores monetarios
- ✅ **Mantener consistencia**: Mismos rangos temporales para comparaciones
- ✅ **Etiquetas informativas**: Títulos descriptivos y ejes claros

#### **Don'ts (Qué NO hacer)**
- ❌ **Puntos aislados**: Pierde la narrativa temporal
- ❌ **Connected scatter plots sin indicadores**: Se convierte en "garabato sin sentido"
- ❌ **Escalas incompatibles**: Hace imposible la comparación
- ❌ **Sobrecarga visual**: Demasiadas líneas o elementos

---

### **Insights del análisis**

#### **Relación Revenue-Inflación**
- **Período analizado**: Diciembre 2010 - Noviembre 2011
- **Patrón observado**: Correlación negativa entre revenue e inflación
- **Interpretación**: Aumentos en inflación correlacionan con disminuciones en revenue
- **Técnica reveladora**: Connected scatter plot con gradiente de opacidad

#### **Ventas por País**
- **Países analizados**: Francia, Alemania, Países Bajos (top 3 excluyendo UK)
- **Patrón estacional**: Variaciones consistentes a lo largo del año
- **Diferencias regionales**: Comportamientos de compra distintivos por país

---

### **¿Por qué estas técnicas son fundamentales?**

#### **Series Temporales Individuales**
- **Base de la narrativa**: Establecen el contexto temporal
- **Identificación de tendencias**: Revelan patrones a largo plazo
- **Puntos de inflexión**: Marcan eventos económicos importantes

#### **Múltiples Series**
- **Comparación efectiva**: Permiten identificar divergencias y convergencias
- **Análisis relativo**: Contextualizan el rendimiento individual
- **Patrones emergentes**: Revelan interacciones no obvias

#### **Connected Scatter Plots**
- **Relaciones complejas**: Muestran dinámicas que los gráficos separados ocultan
- **Ciclos temporales**: Revelan patrones cíclicos y espirales
- **Cambios de correlación**: Identifican cuándo las relaciones cambian

---

### **Créditos**

**Equipo SomoSiete - Ciencia de Datos 2025**

- **Material base**: Capítulo 13 de "Fundamentals of Data Visualization" por Claus O. Wilke
- **Dataset principal**: E-commerce Analysis UK de Kaggle (atharvaarya25)
- **Dataset secundario**: Monthly Inflation Rate UK
- **Curso**: Ciencia de Datos 2025
- **Enfoque**: Aplicación práctica de principios de visualización científica

---

### **Notas adicionales**

- Asegúrate de tener Python 3.8+ instalado
- Los datasets incluidos contienen datos reales de comercio electrónico y economía
- El notebook incluye explicaciones teóricas seguidas de implementaciones prácticas
- Se recomienda ejecutar las celdas en orden secuencial
- Los gráficos están optimizados para presentaciones y análisis profesional

