🍿 Análisis de Datos de Netflix: Estrategia de Contenido y Satisfacción de la Audiencia

📌 Resumen del Proyecto

Este proyecto tiene como objetivo proporcionar recomendaciones basadas en datos para la estrategia de adquisición y producción de contenido de Netflix. Al analizar el catálogo histórico de Netflix y enriquecerlo con las calificaciones de la audiencia global extraídas de IMDb, este análisis descubre qué es lo que realmente impulsa la satisfacción del espectador e identifica los géneros más rentables para futuras inversiones.

🎯 Preguntas de Negocio Respondidas

El Verdadero Top 10: ¿Cuáles son las películas mejor valoradas en la plataforma cuando filtramos el ruido estadístico (películas de nicho con muy pocos votos)?

Estrategia de Inversión: ¿Qué categorías de contenido ofrecen consistentemente la mayor satisfacción a la audiencia?

El "Efecto TikTok": ¿Cómo está cambiando la tendencia en la duración del contenido a lo largo del tiempo?

🛠️ Tecnologías y Metodología

Lenguaje: Python

Librerías: Pandas, Matplotlib

Entorno: Google Colab

Técnicas Aplicadas:

Limpieza de Datos: Tratamiento de valores nulos (NaN) y estandarización de tipos de datos.

Enriquecimiento de Datos (Data Enrichment): Fusión de bases de datos relacionales utilizando pd.merge() para integrar calificaciones externas de IMDb al catálogo principal de Netflix.

Significancia Estadística: Implementación de indexación lógica para filtrar películas con menos de 10,000 votos, evitando sesgos en los promedios.

Transformación de Datos: Uso de .explode() para desanidar variables categóricas (géneros) y permitir un análisis granular.

Agrupación y Agregación: Uso de .groupby() y .agg() para calcular promedios confiables en categorías con tamaños de muestra significativos (>50 producciones).

📊 Hallazgos Clave y Recomendaciones de Negocio

1. El Verdadero Top 10 (Umbral de Significancia: >10k votos)

Al cruzar el catálogo con IMDb y exigir un umbral mínimo de votos, los datos revelan que los documentales aclamados por la crítica y los éxitos de taquilla mundiales dominan la preferencia de la audiencia.

#1 Global: David Attenborough: A Life on Our Planet (9.0 / +31k votos)

Películas Destacadas: Inception, Django Unchained y éxitos internacionales como 3 Idiots.

2. Recomendación de Inversión por Categoría

Al analizar los géneros con un historial de producción sólido (+50 títulos), los datos muestran ganadores claros para la asignación de presupuesto:

🥇 Documentales (Documentaries): El promedio de calificación más alto (6.97) en 268 títulos.

🥈 Stand-Up Comedy: El segundo promedio más alto (6.66) en 211 especiales (ej. Bo Burnham, Dave Chappelle).

Insight de Negocio: Aunque los "Dramas" conforman la mayor parte del volumen de la plataforma (1,035 títulos), su calidad promedio se diluye a 6.36. Recomendación: Desviar presupuesto marginal de dramas genéricos hacia Documentales y especiales de Stand-Up de alta calidad para impulsar la percepción general de la plataforma.

🚀 Cómo Ejecutar el Proyecto

Puedes ver el código completo, los DataFrames interactivos y las visualizaciones haciendo clic en la insignia "Open in Colab" (si Colab la generó) o abriendo el archivo .ipynb incluido en este repositorio. No se requiere instalación local.

Creado por Jair Eduardo Alfaro Ahuatzin como parte de un portafolio de Análisis de Datos.
