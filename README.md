# 🎵 Spotify Tracks — Análisis Exploratorio de Datos

Proyecto académico grupal de **Python para Análisis de Datos**. Analiza características musicales y su relación descriptiva con la popularidad de canciones de Spotify.

## Objetivo
Explorar la asociación entre **popularidad** (escala 0–100) y bailabilidad, contenido explícito, colaboraciones y valencia; además de explorar diferencias entre géneros y artistas.

## Dataset
`spotify-tracks-dataset-detailed.csv`: **114 000 filas y 20 columnas** en el archivo original. Se encontraron **450 filas completamente duplicadas** y **3 valores faltantes** en columnas de metadatos. El notebook elimina filas con nulos y duplicados antes del análisis. Este es un dataset de terceros, no datos internos de Spotify; verificar licencia y procedencia antes de publicarlo públicamente.

## Herramientas
Python, pandas, NumPy, Matplotlib y Seaborn. El análisis del notebook es **exploratorio (EDA)**, no un modelo predictivo entrenado.

## Hallazgos e interpretación
- Bailabilidad y popularidad: correlación positiva **muy débil** (~0.035 en datos originales). Las diferencias entre grupos no prueban causalidad.
- Valencia y popularidad: correlación negativa **muy débil** (~−0.041 reportada en el notebook).
- Se comparan promedios de popularidad por contenido explícito y colaboraciones. Las asociaciones observadas pueden depender de otros factores.
- La presentación del grupo muestra una comparación de modelos de regresión, **pero el código de entrenamiento/evaluación no forma parte de este notebook**. Por ello, los resultados predictivos no se presentan aquí como reproducidos.

## Cómo ejecutarlo
1. Instala Python 3.10+ y las dependencias: `pip install -r requirements.txt`.
2. Abre `GRUPO 7 - SPOTIFY Final.ipynb` en JupyterLab, VS Code o Google Colab.
3. Mantén el CSV en la misma carpeta y ejecuta todas las celdas en orden.

## Archivos
- `GRUPO 7 - SPOTIFY Final.ipynb`: análisis y visualizaciones.
- `spotify-tracks-dataset-detailed.csv`: datos originales (revisar licencia antes de publicar).
- `requirements.txt`: dependencias.

## Créditos
**Trabajo académico del Grupo 7:** Evamaria Castillo, Kevin Martinez Gambini, Jhon Giraldo, Rodrigo Astupinaro y Josealejandro Preguntegui Pasco. Para atribuir contribuciones individuales, añadir solo tareas efectivamente realizadas por cada integrante.

## Limitaciones
Este análisis es observacional: las asociaciones no demuestran causalidad. Popularidad depende de múltiples factores no incluidos. Las métricas predictivas de las diapositivas requieren código y metodología de validación para poder verificarse.
