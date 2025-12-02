# 😀 World Happiness Report 2019 Dataset

## Información general
- **Nombre:** World Happiness Report 2019  
- **Autor/es:** Sustainable Development Solutions Network (SDSN)  
- **Origen/URL:** [Kaggle - World Happiness Report 2019](https://www.kaggle.com/datasets/unsdsn/world-happiness)  
- **Fecha de descarga:** 14-09-2025  
- **Licencia:** Datos abiertos para uso académico e investigativo (según SDSN)  
- **Versión:** 2019  

## 📖 Descripción
Este dataset recopila los resultados del **World Happiness Report 2019**, un informe anual que mide el bienestar subjetivo en distintos países del mundo.  
Las puntuaciones provienen de encuestas globales (Gallup World Poll) y se relacionan con factores como **PIB per cápita, apoyo social, esperanza de vida saludable, libertad para tomar decisiones vitales, generosidad y percepción de corrupción**.  

Es ampliamente utilizado en **análisis exploratorio, visualización, regresión y modelos predictivos** para estudiar el impacto de variables socioeconómicas en la felicidad de los países.

## 🗂️ Esquema del dataset
| Columna                         | Tipo    | Descripción |
|---------------------------------|---------|-------------|
| Overall rank                    | integer | Posición del país en el ranking de felicidad (1 = más feliz). |
| Country or region               | string  | Nombre del país o región. |
| Score                           | float   | Puntaje de felicidad (0–10). |
| GDP per capita                  | float   | Logaritmo del PIB per cápita. |
| Social support                  | float   | Percepción de apoyo social (0–1). |
| Healthy life expectancy         | float   | Esperanza de vida saludable (años). |
| Freedom to make life choices    | float   | Libertad percibida para tomar decisiones (0–1). |
| Generosity                      | float   | Índice de generosidad (donaciones, ayuda, etc.). |
| Perceptions of corruption       | float   | Nivel de corrupción percibida (0–1, menor = menos corrupción). |

## ⚠️ Limitaciones y sesgos conocidos
- El índice se basa en **percepciones subjetivas**, por lo que pueden existir sesgos.
