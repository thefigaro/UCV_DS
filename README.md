[![](https://extensionciencias.ucv.ve/wp-content/uploads/2025/01/Formato-nuevo-06-1024x512.png)](https://extensionciencias.ucv.ve/diplomado-ciencias-de-datos/)

[![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/try-jupyter/lab/)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)

[![Website](https://img.shields.io/badge/Universidad-Central%20de%20Venezuela-blue?style=for-the-badge)](https://extensionciencias.ucv.ve/diplomado-ciencias-de-datos/)

Este repositorio reúne las actividades, análisis y proyectos desarrollados dentro del Diplomado en Ciencias de Datos de la Universidad Central de Venezuela (Cohorte 2023-01). Aquí se aplican técnicas de exploración de datos, visualización, minería de texto, clasificación supervisada, reglas de asociación y análisis de noticias.

## Índice

- [Objetivo del repositorio](#objetivo-del-repositorio)
- [Tecnologías utilizadas](#tecnologías-utilizadas)
- [Datasets](#datasets)
- [Asignación 01](#asignación-01)
- [Asignación 02](#asignación-02)
- [Asignación 03](#asignación-03)
- [Asignación 04](#asignación-04)
- [Asignación 05](#asignación-05)
- [Proyecto final](#proyecto-final)
- [Estado del proyecto](#estado-del-proyecto)

## Objetivo del repositorio

El propósito de este repositorio es documentar y compartir las actividades realizadas durante el diplomado, con foco en:

- Análisis exploratorio de datos,
- Visualización de información,
- Clasificación automática,
- Minería de texto,
- Reglas de asociación para recomendación,
- Análisis de datos no estructurados y extracción de información.

## Tecnologías utilizadas

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Mining de texto
- Técnicas de asociación (FP Growth)

## Datasets

A continuación se listan los principales conjuntos de datos utilizados en las actividades del repositorio.

### 1) Películas y series
- Fuente: [Kaggle - Movies and TV Shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
- Archivo disponible en: [datasets/movies_tv_shows](datasets/movies_tv_shows)
- Nombre del archivo: `movies_tv_shows.zip`

Este conjunto se utilizó para tareas de conteo de categorías, visualización exploratoria, clasificación y análisis de asociación.

### 2) Capítulos de El Quijote
- Fuente: [Miguel de Cervantes - El Quijote](https://www.gutenberg.org/cache/epub/15115/pg15115.txt)
- Archivos disponibles en: [datasets/Cap_10_11_cervantes](datasets/Cap_10_11_cervantes)
- Archivos principales:
  - `cap_10_cervantes.txt`
  - `cap_11_cervantes.txt`

Este conjunto se empleó para análisis de frecuencia de palabras y extracción de patrones léxicos.

### 3) Datos de búsqueda de noticias
- Fuente: consultas realizadas en [searx](https://metasearx.com/)
- Datos almacenados en: [datasets/Projecto_final_DS_data_json](datasets/Projecto_final_DS_data_json)

Se utilizaron búsquedas de noticias con la palabra clave “Venezuela” durante varios días para su posterior análisis de tópicos.

---

## Asignación 01

### Descripción
Se realizó un conteo de ocurrencias de las categorías del campo `Listed In`, como por ejemplo: Comedy, Drama, Action, entre otras.

### Objetivo
Identificar la frecuencia de cada categoría dentro del dataset para entender la distribución de géneros y temáticas presentes en las películas y series.

### Datos
- Fuente: [Kaggle - Movies and TV Shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
- Dataset: [datasets/movies_tv_shows](datasets/movies_tv_shows)

---

## Asignación 02

### Descripción
Se realizó una exploración visual con gráficos generados con `matplotlib`, representando diferentes aspectos de las películas y series.

### Objetivo
Comprender mejor la distribución de los datos mediante visualizaciones intuitivas que permitan identificar tendencias, patrones y anomalías.

### Datos
- Fuente: [Kaggle - Movies and TV Shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
- Dataset: [datasets/movies_tv_shows](datasets/movies_tv_shows)

---

## Asignación 03

### Descripción
Se implementó un algoritmo de clasificación bayesiana con enfoque Naive Bayes.

### Objetivo
Clasificar automáticamente si una película parece estar orientada más hacia el público masculino o femenino, según la información del reparto (`cast`) y las categorías (`listed_in`).

### Concepto
Se asigna un puntaje de orientación:

- Puntaje positivo: mayor orientación hacia público masculino
- Puntaje negativo: mayor orientación hacia público femenino
- Puntaje cercano a cero: mayor neutralidad

### Observación
Las reglas de preprocesamiento para inferir género a partir de nombres del elenco requieren mayor rigor analítico. No obstante, este ejercicio se desarrolló con fines ilustrativos y didácticos.

---

## Asignación 04

### Descripción
Se trabajó con algoritmos de asociación, específicamente **FP Growth**, como una aproximación a un sistema de recomendación.

### Objetivo
Proponer un sistema que recomiende películas según las preferencias del usuario, tomando como referencia el género o categoría de las producciones.

### Referencia
- [FP Growth - Wikipedia](https://es.wikipedia.org/wiki/Reglas_de_asociaci%C3%B3n)

### Datos
- Fuente: [Kaggle - Movies and TV Shows](https://www.kaggle.com/datasets/krishnaraj30/movies-and-tv-shows)
- Dataset: [datasets/movies_tv_shows](datasets/movies_tv_shows)

---

## Asignación 05

### Descripción
Se realizó un análisis de frecuencia relativa de palabras y frases en los capítulos 10 y 11 de El Quijote.

### Objetivo
Aplicar técnicas de text mining para cuantificar la repetición de términos y patrones léxicos dentro del texto.

### Datos
- Fuente: [Proyecto Gutenberg - El Quijote](https://www.gutenberg.org/cache/epub/15115/pg15115.txt)
- Dataset: [datasets/Cap_10_11_cervantes](datasets/Cap_10_11_cervantes)

---

## Proyecto Final DS

### Descripción
Proyecto final centrado en el análisis de tópicos en distintos buscadores de internet y sus canales de noticias, utilizando palabras clave relevantes como “Venezuela”.

### Objetivo
Evaluar cómo los buscadores ordenan y priorizan resultados de noticias, así como estudiar la relevancia temática de los contenidos asociados a una consulta específica.

### Procedimiento
Las búsquedas se realizaron en el meta-buscador [searx](https://metasearx.com/) durante una semana, tomando las primeras 10 apariciones por día para la palabra clave `Venezuela`.

### Fechas de consulta

| Dataset | Fecha |
|--------|------|
| `searx.thegpm.org_0.json` | 19-09-2023 |
| `searx.thegpm.org_1.json` | 20-09-2023 |
| `searx.thegpm.org_2.json` | 21-09-2023 |
| `searx.thegpm.org_3.json` | 22-09-2023 |
| `searx.thegpm.org_4.json` | 23-09-2023 |
| `searx.thegpm.org_5.json` | 24-09-2023 |
| `searx.thegpm.org_6.json` | 25-09-2023 |

### Datos
- Ubicación: [datasets/Projecto_final_DS_data_json](datasets/Projecto_final_DS_data_json)

---

## Estado del proyecto

- [x] Exploración y preprocesamiento de datos
- [x] Análisis de categorías
- [x] Visualización exploratoria
- [x] Clasificación bayesiana
- [x] Reglas de asociación (FP Growth)
- [x] Text mining
- [x] Proyecto final
- [ ] Análisis de clustering (pendiente)

---

## Repositorio

Este repositorio está orientado a la práctica de conceptos fundamentales de ciencia de datos aplicados a problemas reales y académicos, con un enfoque didáctico y experimental.

Si quieres contribuir, mejorar el análisis o extender alguna de las tareas, puedes hacer fork del repositorio y enviar tus propuestas.
