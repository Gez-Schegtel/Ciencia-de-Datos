# 🍲 Indian Food Dataset

## Información general
- **Nombre:** Indian Food Dataset
- **Autor/es:** Neha Prabhavalkar (Owner)
- **Origen/URL:** https://www.kaggle.com/datasets/nehaprabhavalkar/indian-food-101
- **Fecha de descarga:** 10-10-2025
- **Licencia:** Data files © Original Authors
- **Versión:** 1

## 📖 Descripción
Este dataset recopila información sobre una amplia variedad de platos de la cocina india, incluyendo el nombre del plato, los ingredientes principales, el tipo de dieta (vegetariano/non-vegetariano), tiempos de preparación y cocción, perfil de sabor, la parte de la comida a la que pertenece (entrada, plato principal, postre, etc.), y su lugar de origen (estado y región).

Los datos provienen de recopilaciones y páginas de recetas (p. ej. Wikipedia, Hebbar's Kitchen, Archana's Kitchen) y son útiles para tareas de análisis exploratorio, procesamiento de texto (ingredientes), clasificación por región o tipo de plato, y estudios sobre diversidad culinaria regional.

> Nota: la presencia de `-1` en cualquier columna indica un valor faltante (NaN) en el dataset.

## 🗂️ Esquema del dataset
| Columna         | Tipo    | Descripción |
|-----------------|---------|-------------|
| name            | string  | Nombre del plato. |
| ingredients     | string  | Principales ingredientes usados (lista o texto separado por comas). |
| diet            | string  | Tipo de dieta: `vegetarian` o `non vegetarian`. |
| prep_time       | integer | Tiempo de preparación (en minutos). `-1` indica NaN. |
| cook_time       | integer | Tiempo de cocción (en minutos). `-1` indica NaN. |
| flavor_profile  | string  | Perfil de sabor: spicy, sweet, bitter, sour, etc. `-1` indica NaN o desconocido. |
| course          | string  | Curso de la comida: starter, main course, dessert, snack, etc. |
| state           | string  | Estado donde el plato es famoso o de origen. `-1` indica NaN. |
| region          | string  | Región de la India a la que pertenece el estado (North, South, East, West, North East, Central, etc.). `-1` indica NaN. |

## ⚠️ Limitaciones y sesgos conocidos
- Nada reportado.
