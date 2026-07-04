# Predicciones_ventas_videojuegos
Análisis exploratorio de datos de ventas de videojuegos (1980–2016) para identificar patrones de plataforma, género y región que apoyen decisiones de marketing. Incluye limpieza de datos, ingeniería de características, visualización con Matplotlib/Seaborn y pruebas de hipótesis con SciPy.


## Descripción del proyecto
A partir de un conjunto de datos con información de ventas de videojuegos por región (Norteamérica, Europa, Japón y otras), plataforma, género, año de lanzamiento y calificaciones (críticos, usuarios y clasificación ESRB), se realizó un proceso completo de análisis de datos:


- Limpieza y preprocesamiento: tratamiento de valores ausentes en columnas críticas (name, year_of_release, genre, critic_score, user_score, rating), decisiones justificadas de imputación según el tipo y proporción de datos faltantes, y corrección de tipos de datos.
- Ingeniería de características: creación de la columna total_sales como suma de ventas por región.
- Análisis exploratorio y visualización: tendencias de lanzamientos por año, ciclo de vida de las plataformas, distribución de ventas por plataforma (boxplots), correlación entre calificaciones y ventas, comparación de ventas de un mismo juego entre plataformas, y análisis de géneros más rentables.
- Análisis por región: perfil de plataformas, géneros y clasificación ESRB más vendidos en NA, EU y JP.
- Pruebas de hipótesis: contraste estadístico (t-test) sobre si existen diferencias significativas en las calificaciones promedio de usuarios entre las plataformas Xbox One y PC, y entre los géneros de Acción y Deportes.


## Objetivo

Identificar qué plataformas y géneros resultan potencialmente más rentables para el año siguiente, entendiendo el ciclo de vida de las consolas y el comportamiento de ventas por región.

## Tecnologías utilizadas


- Python
- Pandas / NumPy — manipulación y limpieza de datos
- Matplotlib / Seaborn — visualización de datos
- SciPy — pruebas de hipótesis estadísticas


## Principales hallazgos


- El pico de lanzamientos de videojuegos ocurrió a finales de la década de 2000, con una tendencia a la baja desde entonces.
- Las plataformas tienen un ciclo de vida aproximado de 10 a 13 años; algunas de las plataformas identificadas como potencialmente rentables para el año siguiente fueron PS4, XOne, PC, PS3, X360 y 3DS.
- La mediana de ventas por videojuego es cercana a cero en casi todas las plataformas: la rentabilidad depende principalmente de un pequeño número de juegos con ventas atípicamente altas.
- No se encontró una correlación fuerte entre las calificaciones de usuarios/críticos y las ventas totales.
- Cada plataforma tiene un perfil de género predominante entre sus usuarios, lo cual es relevante para decidir en qué consola lanzar un juego según su género.
- Japón muestra un comportamiento de mercado distinto al de Norteamérica y Europa, lo que sugiere la necesidad de tratarlo por separado en futuros modelos.
- Existe una diferencia estadísticamente significativa entre las calificaciones de usuario de Xbox One y PC, pero no entre los géneros de Acción y Deportes.


## Estructura del notebook


1. Carga de datos
2. Preprocesamiento (nombres de columnas, duplicados, valores ausentes, tipos de datos)
3. Ingeniería de características
4. Visualización y análisis (lanzamientos por año, ventas por plataforma, correlaciones, géneros)
5. Perfil de usuario por región
6. Pruebas de hipótesis
7. Conclusiones


## Cómo ejecutar el proyecto

git clone <url-del-repo>
cd <nombre-del-repo>
pip install pandas numpy matplotlib seaborn scipy
jupyter notebook notebook_proyecto.ipynb


## Notas
Proyecto desarrollado como parte del programa de Ciencia de Datos de TripleTen (aprobado en primera revisión).
