# Análisis de Ranks de Jugadores

Este repositorio contiene un cuaderno de Jupyter (Google Colab) diseñado para el análisis exhaustivo de los **ranks de jugadores** a lo largo de diferentes 'seasons' o cortes temporales. El objetivo es proporcionar una comprensión profunda de la evolución individual y colectiva de un grupo de jugadores.

## Características Principales

-   **Carga y Preprocesamiento de Datos**: Funciones robustas para cargar archivos CSV desde Google Drive, manejar valores nulos y transformar los rangos de texto a un formato numérico para facilitar el análisis.
-   **Análisis Longitudinal**: Convierte los datos a un formato largo para rastrear la evolución de cada jugador a través de múltiples seasons.
-   **Métricas Agregadas por Season**: Calcula promedios, medianas y distribuciones exactas de ranks por cada season, identificando la composición competitiva del grupo.
-   **Dinámica de Transición**: Analiza las incorporaciones, salidas y los cambios de rank (mejoras, mantenimientos, retrocesos) entre seasons consecutivas.
-   **Trayectoria Individual**: Genera una tabla con el primer y último rank observado para cada jugador, así como su mejora neta.
-   **Visualizaciones Clave**: Incluye gráficos para:
    -   Evolución del promedio y la mediana del rank del grupo.
    -   Distribución de ranks por season.
    -   Cambios de rank entre seasons (mejoras, sin cambio, empeoró).
    -   Dinámica de incorporaciones y salidas de jugadores.
    -   Slope chart de trayectorias individuales.
-   **Resumen Ejecutivo**: Un informe conciso en formato Markdown que consolida los hallazgos más importantes del análisis.

## Cómo Usar el Notebook

1.  **Montar Google Drive**: Asegúrate de que tu Google Drive esté montado en Colab para acceder a tus archivos CSV.
2.  **Configurar `file_path`**: En la sección de configuración, actualiza la variable `file_path` con la ruta a tu archivo CSV que contiene los datos de los jugadores.
3.  **Ejecutar las Celdas**: Corre todas las celdas del notebook en secuencia. El notebook está diseñado para guiarte a través del proceso de carga, análisis y visualización.
4.  **Interpretar los Resultados**: Revisa las tablas y gráficos generados en las secciones de 'Análisis' y 'Visualizaciones' para entender la evolución de los jugadores.

## Estructura del Archivo CSV Esperado

El archivo CSV debe contener al menos:
-   Una columna que identifique de forma única a cada jugador (ej. 'Nick').
-   Múltiples columnas representando los ranks de los jugadores en diferentes 'seasons' (ej. 'Rank 6', 'Rank 6.5', 'Rank 7', etc.).
-   Opcionalmente, columnas de referencia de ranks (ej. 'Rank Alto').

Los valores de rank deben seguir el formato '`[número]. [Nombre del Rank]`' (ej., '3. Celestial', '6. Platino') o 'N/A'/'No Rank' para jugadores sin rango en una season específica.

## Licencia

Este proyecto se distribuye bajo la **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

Esto significa que eres libre de:
-   **Compartir** — copiar y redistribuir el material en cualquier medio o formato.
-   **Adaptar** — remezclar, transformar y construir sobre el material.

Bajo los siguientes términos:
-   **Atribución** — Debes dar crédito apropiado, proporcionar un enlace a la licencia e indicar si se realizaron cambios. Puedes hacerlo de cualquier manera razonable, pero no de una manera que sugiera que el licenciante te respalda a ti o a tu uso.
-   **NoComercial** — No puedes utilizar el material con fines comerciales.
-   **CompartirIgual** — Si remezclas, transformas o construyes sobre el material, debes distribuir tus contribuciones bajo la misma licencia que el original.

Para ver la licencia completa, visita [https://creativecommons.org/licenses/by-nc-sa/4.0/](https://creativecommons.org/licenses/by-nc-sa/4.0/).