# Fundamentals of Data Visualization: Capítulos 12 y 15

Este laboratorio abarca:

- **Capítulo 12**: Visualizing associations among two or more quantitative variables (obligatorio).
- **Capítulo 15**: Visualizing geospatial data (opcional).

Los gráficos generados en `presentation.ipynb` fueron exportadas a `images/` para ser usados en la presentación creada con Google Slides: [https://docs.google.com/presentation/d/1Vw3mghhjd8ac2N7EzxAfOL3qCYe625oi1tU_V2jggUo/edit](https://docs.google.com/presentation/d/1Vw3mghhjd8ac2N7EzxAfOL3qCYe625oi1tU_V2jggUo/edit).

## Instalación

1. Crear entorno virtual

**macOS/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

2. Instalar dependencias

```bash
pip install -r requirements.txt
```

3. Ejecutar

```bash
jupyter notebook presentation.ipynb
```

### Alternativa con `uv`

Utilizando [`uv`](https://docs.astral.sh/uv/pip/environments/) en lugar de `pip`:

```
uv sync
source .venv/bin/activate
```
