Sistema de Recomendación Básico con Similitud del Coseno

Este proyecto implementa un sistema sencillo de recomendación de películas basado en la similitud del coseno entre sus géneros.

Objetivo

Comparar películas según sus géneros y calcular su nivel de similitud, mostrando los resultados en forma de matriz y gráficos comparativos.

Dataset

El archivo utilizado es Peliculas.csv, que contiene una lista de películas junto a sus géneros representados en formato binario (0 o 1).

Ejemplo:

Película	Amor	Aventura	Acción	Comedia	Terror	Animación
Misión Imposible	0	1	1	0	0	0
Piratas del Caribe	0	1	1	1	0	0
Librerías utilizadas

numpy

pandas

matplotlib

scikit-learn

Flujo del proyecto

Importación de librerías: numpy, pandas, matplotlib, sklearn.

Lectura del DataFrame desde Google Drive (Peliculas.csv).

Procesamiento de datos: extracción de columnas de géneros.

Cálculo de similitud usando la función cosine_similarity de scikit-learn.

Generación de matriz de similitud en un DataFrame que muestra los valores de similitud entre todas las películas.

Visualización mediante gráficos de barras comparativos de similitud para cada película.

Resultados

Se obtiene una matriz de similitud del coseno que muestra qué películas son más cercanas entre sí en función de sus géneros.

Se generan gráficos de barras que ilustran visualmente el nivel de similitud entre una película y el resto.

Ejemplo de salida:

Similitud del Coseno entre Películas:
                   Mision Imposible  Piratas del Caribe  Resacon en las Vegas ...
Mision Imposible            1.000000            0.816497               0.000000
Piratas del Caribe          0.816497            1.000000               0.577350
Resacon en las Vegas        0.000000            0.577350               1.000000
...

Autores

Fabián Vidal
