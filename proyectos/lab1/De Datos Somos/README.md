# 📘 Capítulo 8: Data Wrangling: Join, Combine, and Reshape

El objetivo de este laboratorio es poner en práctica los conceptos del Capítulo 8: Data Wrangling: Join, Combine, and Reshape del libro Python for Data Analysis (3rd Ed.) para ello usaremos el siguiente [notebook](demo_de_datos_somos.ipynb).
Los pasos a continuación permiten clonar el repositorio, preparar el entorno y comenzar a trabajar sin complicaciones.

## 🔹 1. Requisitos previos

- **Python 3.8+** instalado → [Descargar Python](https://www.python.org/downloads/)
- **Visual Studio Code** instalado → [Descargar VS Code](https://code.visualstudio.com/)
- Extensiones necesarias en VS Code:
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
  - [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

## 🔹 2. Clonar el repositorio

```bash
git clone https://github.com/mminoli/cd2025.git
cd cd2025/proyectos/lab1/De\ Datos\ Somos
```

## 🔹 3. Crear y activar entorno virtual

### Linux / macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Windows (CMD. Ejecutar como administrador.)

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Windows (PowerShell. Ejecutar como administrador.)

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Cuando el entorno esté activo, deberías ver algo así en tu terminal:

```
(.venv) $
```

## 🔹 4. Instalar dependencias

Con el entorno virtual activado:

```bash
pip install -r requirements.txt
```

Esto instalará todas las librerías necesarias.

## 🔹 5. Abrir el proyecto en VS Code

Abrir la carpeta del proyecto en VS Code:

```bash
code .
```

## 🔹 6. Seleccionar el entorno virtual en VS Code

1. Abrí el archivo `demo_de_datos_somos.ipynb` o `ejercicios_de_datos_somos.ipynb` con celdas.
2. En la parte superior derecha de VS Code, buscá el menú que dice **"Seleccionar kernel"** o **"Select Kernel"**.
3. Elegí el kernel que corresponde a tu entorno virtual `.venv`.  
   Normalmente aparecerá como:
   ```
   Python 3.x ('./.venv')
   ```
4. Una vez seleccionado, podés ejecutar celdas con:
   - `Shift + Enter` → Ejecutar celda y pasar a la siguiente.
   - `Ctrl + Enter` → Ejecutar celda sin avanzar.

## 🔹 7. Desactivar el entorno virtual (opcional)

Cuando termines de trabajar, podés salir del entorno con:

```bash
deactivate
```

## 🔹 8. Datasets utilizados

Para los ejercicios contenidos en `ejercicios_de_datos_somos.ipynb`, se emplearon datos oficiales de elecciones presidenciales en la Provincia del Chaco, Argentina, disponibles en el portal de la [Dirección Nacional Electoral](https://resultados.mininterior.gob.ar/).

Estos datasets permiten practicar técnicas de **join**, **merge**, **concatenación** y **reshaping** de datos con ejemplos reales de resultados electorales por distrito, categoría y año.

## ✅ Resumen rápido

1. `git clone https://github.com/mminoli/cd2025.git`
2. `cd cd2025/proyectos/lab1/De\Datos\Somos`
3. `python -m venv .venv && source .venv/bin/activate`
4. `pip install -r requirements.txt`
5. `code .` → abrir en VS Code
6. **Seleccionar kernel `.venv` en VS Code**
7. Ejecutar celdas (`Shift+Enter`)

¡Y listo! 🎉 Ya podés correr las celdas de Jupyter directamente en VS Code.
