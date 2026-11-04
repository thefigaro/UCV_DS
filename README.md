# Universidad Central de Venezuela [Diplomado en Ciencias de Datos](https://extensionciencias.ucv.ve/diplomado-ciencias-de-datos/)


[ ![Alt text](https://extensionciencias.ucv.ve/wp-content/uploads/2025/01/Formato-nuevo-06-1024x512.png)](https://extensionciencias.ucv.ve/diplomado-ciencias-de-datos/)

<div align="center">
  
[![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/try-jupyter/lab/)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](http://python.org)

</div>

## Asignacion_01 
   * Se realizó un conteo de ocurrencia de las categorías (i.e. el campo `Listed In`), por ejemplo: Comedy, Drama, etc.

   * **Fuente de datos** (archive_movies_csv.zip): [kaggle: data_set_movies_tv_shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
   * El dataset antes mencionado se encuentra para su uso en: [datasets/movies_tv_shows](datasets/movies_tv_shows) bajo el nombre de `movies_tv_shows.zip`

## Asignacion_02
   * Exploracion_Viz: 5 gráficos con matplotlib  de las películas y series
   
   * **Fuente de datos** (archive_movies_csv.zip): [kaggle: data_set_movies_tv_shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
   * El dataset antes mencionado se encuentra para su uso en: [datasets/movies_tv_shows](datasets/movies_tv_shows) bajo el nombre de `movies_tv_shows.zip`

## Asignacion_03 (algoritmo -random naive bayes-)
   * Clasificación Bayesiana (Naive)
   * Proyecto: Identificación según el género del público consumidor en filmes o peliculas 

Objetivo: Clasificación “automática”   
Nuestra clasificación consistirá en asignar un ***puntaje-score*** que adjudique si la película está orientada al público masculino 🚹 o femenino 🚺.

* A mayor puntaje en la escala positiva, mayor orientación masculina se percibe en la película. Por tanto, esta se clasifica como +1
* Asi mismo, a mayor puntaje en la escala negativa, mayor orientación femenina se percibe en la película. Y, por tanto, esta se clasifica como -1.
* Y finalmente, un puntaje cercano a 0 sugiere que la película no está sesgada hacia ningún género en particular, lo que la convierte en una opción neutral para ambos públicos

Para calcular el puntaje (score):
Tomaremos los campos `cast` y `listed_in`:

Pretendemos es identificar el género (masc ó fem) de los protagonistas `cast` en cada una de las películas.

Si los nombres (en ingles) en `cast` son masculinos o femeninos, se le adjudicará un puntaje de *+1/-1* respectivamente. Para adjudicar el género se tomará la última letra del nombre de los protagonistas. Las terminaciones en: *e, o, d, h, n, m, l, g*, ó sus combinaciones pares, por ej. *'en', 'hn','oh','on'*, etc. en cada uno de los nombres, serán clasificadas con un puntaje de *+1* (masculino). Todas las terminaciones distintas a las antes mencionadas, *e, o, h, n, m, l, g* serán clasificadas con un puntaje *-1* (femenino).

**Nota: Ciertamente, las reglas de pre-procesamiento para identificar el género del elenco de en la variable `cast` necesitan una elaboración más rigurosa. No obstante, para fines ilustrativos NO consideraremos ser más rigurosos en esta asignación.** 

## Analisis de Cluster (pendiente)

## Asignacion_04 (FP Growth) (Aproximación a un sistema de recomendación)
   * Algoritmos de asociación, en este caso se utilizó (Frequent Pattern Growth -FP Growth-). véase. [-FP Growth- wiki](https://es.wikipedia.org/wiki/Reglas_de_asociaci%C3%B3n)
   * Se realizó una propuesta para un sistema de recomendación de películas según las preferencias, el género (ie. Comedia, Drama,... )
   
   * **Fuente de datos** (archive_movies_csv.zip): ![data_set_movies_tv_shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
   * El dataset antes mencionado se encuentra para su uso en: [datasets/movies_tv_shows](datasets/movies_tv_shows) bajo el nombre de `movies_tv_shows.zip`

## Asignacion_05 (textmine)
   * Realizamos un conteo relativo de palabras y frases tanto en capítulo 10 como 11.
     
   * Fuente de datos: [Miguel de Cervantes - El Quijote - ](https://www.gutenberg.org/cache/epub/15115/pg15115.txt)
   * Se separaron el cap 10 y 11; (cap_10_cervantes.txt) (cap_10_cervantes.txt)
   * Los datasets antes mencionados se encuentran para su uso respectivamente en: [datasets/Cap_10_11_cervantes](datasets/Cap_10_11_cervantes) 
      
## Proyecto_Final_DS
  * Proyecto: Análisis de clasificatorio de tópicos en los distintos buscadores de internet en sus canales de noticias (news) según palabras clave.
  
  * Objetivo: Los buscadores de internet en sus canales de noticias utilizan una combinación compleja de algoritmos para determinar la relevancia y el orden de los resultados de búsqueda. En tal sentido, realizamos una busqueda de los topicos más importantes que influyen en la clasificación de los resultados para la consulta con la palabra "Venezuela". 
    
 Procedimiento de búsqueda de datos:
  * Las consultas se realizaron en el meta-buscador: [searx](https://metasearx.com/)
  * Realizamos consultas de la última semana de noticias dia '19-09-2023' con la palabra "Venezuela" y tomamos las 10 primeras apariciones: `http://searx.thegpm.org/?q=venezuela&categories=news&time_range=week&language=en`

<div align="center">
  
|Data_set               |      Dia de consulta "Venezuela"        |
|-----------------------|:---------------------------------------:|
|searx.thegpm.org_0.json|                         19-09-2023      |
|searx.thegpm.org_1.json|                         20-09-2023      |
|searx.thegpm.org_2.json|                         21-09-2023      |
|searx.thegpm.org_3.json|                         22-09-2023      |
|searx.thegpm.org_4.json|                         23-09-2023      |
|searx.thegpm.org_5.json|                         24-09-2023      |
|searx.thegpm.org_6.json|                         25-09-2023      |
</div>

* Las búsquedas resultantes en formato *.json para su uso encuentran en: [datasets/Projecto_final_DS_data_json](datasets/Projecto_final_DS_data_json)

