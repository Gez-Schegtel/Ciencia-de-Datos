# Laboratorio Capítulo 4 - NumPy Basics: Arrays and Vectorized Computation

### **Objetivos**

Este laboratorio tiene como objetivo explorar **NumPy como la piedra angular fundamental del análisis de datos en Python**. A través de ejercicios prácticos con un dataset real de e-commerce, aprenderemos:

- **Fundamentos de NumPy**: Comprender por qué NumPy es la base del ecosistema científico de Python
- **Arrays multidimensionales (ndarray)**: Crear, manipular y operar con arrays de manera eficiente
- **Computación vectorizada**: Realizar operaciones matemáticas en bloques de datos sin bucles explícitos
- **Indexación y slicing**: Técnicas avanzadas para acceder y modificar datos
- **Operaciones estadísticas**: Funciones matemáticas y estadísticas aplicadas a arrays
- **Performance**: Comparar la eficiencia de NumPy vs Python puro
- **Álgebra lineal**: Operaciones matriciales fundamentales para análisis de datos

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

#### 3. Ejecutar los notebooks
```bash
# Iniciar Jupyter desde la terminal
jupyter notebook

# O si prefieres Jupyter Lab
jupyter lab
```

Luego abre los siguientes archivos en orden:
1. `demo_somo_siete_v0.ipynb` - Demostración teórica y ejemplos
2. `ejercicios_somo_siete_v1.ipynb` - Ejercicios prácticos

---

### **Dataset utilizado**

**E-commerce Analysis UK Dataset**
- **Fuente**: [Kaggle - E-commerce Analysis UK](https://www.kaggle.com/datasets/atharvaarya25/e-commerce-analysis-uk)
- **Descripción**: Dataset de transacciones de comercio electrónico del Reino Unido
- **Características**:
  - **541,909 transacciones** de diciembre 2010 a diciembre 2011
  - **8 columnas**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
  - **Casos de uso**: Análisis de ventas, comportamiento de clientes, análisis temporal

**Columnas del dataset**:
- `InvoiceNo`: Número de factura
- `StockCode`: Código de producto
- `Description`: Descripción del producto
- `Quantity`: Cantidad comprada
- `InvoiceDate`: Fecha y hora de la transacción
- `UnitPrice`: Precio unitario
- `CustomerID`: ID del cliente
- `Country`: País de la transacción

---

### **Estructura del proyecto**

```
Somo´Siete/
├── README.md                           # Este archivo
├── requirements.txt                    # Dependencias del proyecto
├── data.csv                           # Dataset de e-commerce UK
├── demo_somo_siete_v0.ipynb          # Notebook de demostración
├── ejercicios_somo_siete_v1.ipynb    # Notebook de ejercicios
└── .venv/                             # Entorno virtual (creado localmente)
```

---

### **Contenido del laboratorio**

**Basado en el Capítulo 4 de "Python for Data Analysis, 3rd Edition"**

1. **Introducción a NumPy**: La piedra angular del ecosistema científico
2. **El objeto ndarray**: Arrays multidimensionales eficientes
3. **Creación de arrays**: Diferentes métodos y técnicas
4. **Tipos de datos**: Optimización de memoria y rendimiento
5. **Operaciones aritméticas**: Computación vectorizada
6. **Indexación y slicing**: Acceso eficiente a los datos
7. **Indexación booleana**: Filtrado avanzado de datos
8. **Funciones universales**: Operaciones elemento por elemento
9. **Programación orientada a arrays**: Lógica condicional sin bucles
10. **Métodos estadísticos y matemáticos**: Análisis descriptivo
11. **Álgebra lineal**: Operaciones matriciales
12. **Ejemplo práctico**: Random walks y simulaciones

---

### **¿Por qué NumPy es fundamental?**

- **Performance**: 10-100x más rápido que Python puro
- **Memoria eficiente**: Almacenamiento contiguo en memoria
- **Interoperabilidad**: Base común para todo el ecosistema científico
- **API en C**: Conexión con librerías de bajo nivel
- **Vectorización**: Operaciones en bloques de datos sin bucles

---

### **Créditos**

**Equipo SomoSiete - Ciencia de Datos 2025**

- **Material base**: Capítulo 4 de "Python for Data Analysis, 3rd Edition" por Wes McKinney
- **Dataset**: E-commerce Analysis UK de Kaggle (atharvaarya25)
- **Curso**: Ciencia de Datos 2025

---

### **Notas adicionales**

- Asegúrate de tener Python 3.8+ instalado
- El dataset incluido (`data.csv`) contiene más de 500k registros
- Los notebooks incluyen ejercicios progresivos desde conceptos básicos hasta aplicaciones avanzadas
- Se recomienda ejecutar los notebooks en orden secuencial


