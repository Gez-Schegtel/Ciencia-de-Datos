# Laboratorio 1 - Equipo Lambda

Este es el laboratorio 1 del equipo Lambda. Explora el Capítulo 9 **Gráficos y visualización** del libro _Python for Data Analysis, 3rd Edition_ de **Wes McKinney**.

- `exercises.ipynb`: contiene una guía de ejercicios. Cada ejercicio tiene una solución propuesta.
- `presentation.ipynb`: presentación del capítulo 9.

## Instalar dependencias

### Con [uv](https://docs.astral.sh/uv/getting-started/)

```bash
uv sync   # Instalar dependencias definidas en pyproject.toml
```

### Con pip

Crear el entorno virtual:

```bash
python -m venv .venv
```

Activar el entorno:

- En Linux / macOS

  ```bash
  source .venv/bin/activate
  ```

- En Windows (PowerShell)

  ```bash
  .venv\Scripts\Activate
  ```

Instalar dependencias:

```bash
pip install -r requirements.txt
```
