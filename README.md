# 📊 Proyecto 9 – Clustering

Proyecto desarrollado como parte del Bootcamp de Data Analytics enfocado en la aplicación de técnicas de **Machine Learning No Supervisado**, específicamente **Clustering**, para identificar patrones y segmentaciones dentro de un conjunto de datos.

---

## 📌 Descripción del Proyecto

El objetivo principal de este proyecto es aplicar algoritmos de clustering para descubrir grupos naturales dentro de los datos sin utilizar variables objetivo.

A lo largo del proyecto se desarrollan las siguientes fases:

- 🔍 Análisis exploratorio de datos (EDA)
- 🧹 Limpieza y preprocesamiento
- ⚙️ Escalado y transformación de variables
- 🤖 Aplicación de algoritmos de clustering
- 📈 Evaluación de métricas
- 📊 Visualización e interpretación de resultados

Este proyecto demuestra competencias en análisis de datos, preparación de datos y modelado no supervisado.

## 👩‍💻 Contribuyentes

  | Nombre           | GitHub | LinkedIn |
|------------------|--------|----------|
| Jaime Amuedo     | [![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JaimeAmuedoJAH) | [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jaime-amuedo-hidalgo-a432bb354/) |
---

## 🗂️ Estructura del Proyecto
```
Proyecto9-clustering/
├── clean_data/         # Scripts o notebooks de limpieza y preprocesamiento
├── notebooks/          # Análisis y modelado exploratorio
    ├── models/             # Modelos entrenados y resultados
├── utils/              # Funciones auxiliares (helpers, utils)
├── .gitignore          # Para ignorar archivos de subida
├── requirements.txt    # Dependencias del proyecto
└── README.md           # Documentación principal (este archivo)
```

> La estructura puede variar ligeramente dependiendo de la versión del repositorio.

---

## 🛠️ Tecnologías Utilizadas

- ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
- ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
- ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
- ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
- ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
- ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 🚀 Instalación y Uso

### 1️⃣ Clonar el repositorio

```
git clone https://github.com/Bootcamp-Data-Analyst/Proyecto9-clustering.git
cd Proyecto9-clustering
code .
```

### 2️⃣ Crear un entorno virtual

```
python -m venv venv
source venv/bin/activate   # Mac / Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Instalar dependencias

```
pip install -r requirements.txt
```

### 4️⃣ Ejecutar notebooks

```
jupyter notebook
```

---

## 📂 Descripción de los Datasets Generados

Durante el proceso de limpieza, transformación, reducción de dimensionalidad y modelado, se generaron los siguientes datasets intermedios y finales:

### 🧹 Limpieza de datos

- **`mushrooms_limpio.csv` & `mushrooms_limpio.parquet`**  
  Dataset limpio exportado del notebook **`ETL.ipynb`**

---

### 🧹 Datos Limpios e Imputados

- **`mushrooms_limpio_imputed.csv` & `mushrooms_limpio_imputed.parquet`**  
  Dataset imputado utilizando **KNN Imputer**, donde se reemplazaron valores nulos y se reconstruyeron las categorías originales.  
  📌 Listo para análisis estadístico y modelado.

- **`mushrooms_cleaned_advanced.csv`**  
  Versión con limpieza avanzada que incluye:
  - Eliminación de duplicados
  - Agrupación de niveles poco frecuentes
  - Imputación por moda (variables categóricas) y mediana (numéricas)

---

### 📉 Reducción de Dimensionalidad

- **`mushrooms_pca.csv`**  
  Representación mediante **PCA (Principal Component Analysis)**.  
  Contiene los componentes principales utilizados como entrada para modelos de clustering y reducción de dimensionalidad.

- **`mushrooms_tsne.csv`**  
  Embedding bidimensional obtenido con **t-SNE**, utilizado principalmente para visualización y análisis de la estructura local de los datos.

---

### 🤖 Clustering

- **`mushrooms_with_clusters.csv`**  
  Dataset original con una etiqueta de cluster generada mediante **KMeans** aplicado sobre un subconjunto de variables seleccionadas.

- **`mushrooms_pca_clustered.csv`**  
  Dataset basado en componentes PCA con múltiples algoritmos de clustering aplicados, incluyendo:
  - KMeans
  - Gaussian Mixture Model (GMM)
  - Agglomerative Clustering
  - DBSCAN  

  Cada algoritmo añade su correspondiente etiqueta de cluster para comparación.

---

### 📊 Evaluación de Modelos

- **`model_scores.csv`**  
  Contiene las métricas de evaluación de los modelos entrenados, incluyendo:

  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - MSE / R² (cuando aplica)

  Este archivo permite comparar el rendimiento entre diferentes enfoques y configuraciones.

---


## 📊 Metodología
### 🔎 1. Análisis Exploratorio (EDA)

Distribución de variables

Detección de outliers

Correlaciones

Visualizaciones descriptivas

### 🧹 2. Preprocesamiento

Tratamiento de valores nulos

Normalización / Estandarización

Selección de variables relevantes

### 🤖 3. Modelado con Clustering

Se aplican técnicas como:

K-Means

Método del Codo (Elbow Method)

Silhouette Score

### 📈 4. Evaluación

Inercia

Coeficiente de Silhouette

Visualización de clusters en 2D

### 📌 Resultados Esperados

Identificación de segmentos claramente diferenciados

Interpretación de características principales de cada cluster

Visualización clara para toma de decisiones

### 📚 Conceptos Aplicados

Machine Learning No Supervisado

Segmentación de datos

Reducción de dimensionalidad (si aplica)

Escalado de variables

Métricas de evaluación de clustering

## 🎯 Objetivo Académico

Este proyecto tiene como finalidad consolidar conocimientos en:

Preparación de datos

Modelado no supervisado

Interpretación de resultados

Comunicación de insights