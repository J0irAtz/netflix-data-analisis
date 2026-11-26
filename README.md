# Análisis exploratorio del catálogo de Netflix

Proyecto de portafolio de Jair Alfaro. Explora la duración de las películas en una muestra histórica del catálogo y compara las calificaciones de los títulos que pudieron cruzarse con IMDb.

## Qué analicé

- La duración promedio de las películas por año de estreno.
- Los títulos mejor calificados tras aplicar un umbral mínimo de votos.
- La calificación media por género y el número de títulos de cada grupo.

## Cómo lo hice

Usé Python, pandas y Matplotlib en Google Colab. Limpié valores faltantes y estandaricé la duración. Integré las calificaciones de IMDb con `merge()`, separé los géneros con `explode()` y calculé los resúmenes con `groupby()`. Los umbrales de votos y de tamaño de grupo son filtros descriptivos.

## Resultados y alcance

En el cruce analizado, los documentales promediaron 6.97 en 268 títulos y los especiales de stand-up 6.66 en 211 títulos. Estas calificaciones describen los títulos incluidos y a quienes votaron en IMDb. Para evaluar rentabilidad o satisfacción de suscriptores harían falta datos adicionales, como costos, consumo y retención.

La tendencia de duración describe la composición de la muestra por año de estreno. Para atribuirla al uso de redes sociales haría falta evidencia adicional sobre exposición y hábitos de audiencia.

## Notebook

- [Consultar el análisis en GitHub](Proyecto_Netflix.ipynb)
- [Abrir en Google Colab](https://colab.research.google.com/github/J0irAtz/netflix-data-analisis/blob/main/Proyecto_Netflix.ipynb)
