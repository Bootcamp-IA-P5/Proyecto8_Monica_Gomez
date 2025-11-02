🧠 Proyecto 8 – Aprendizaje No Supervisado con PCA y Clustering
📚 Descripción del Proyecto

Este repositorio contiene un taller práctico orientado al aprendizaje automático no supervisado, usando técnicas de:

🧩 PCA (Análisis de Componentes Principales) — para reducir la dimensionalidad de los datos.

🔷 Clustering (K-Means) — para agrupar observaciones similares sin usar etiquetas.

🌳 Comparativa con Random Forest (supervisado) — para contrastar resultados entre enfoques supervisados y no supervisados.

El objetivo principal es explorar cómo los algoritmos pueden encontrar patrones y agrupaciones dentro de un conjunto de datos sin conocer las etiquetas, y luego comparar estos resultados con un modelo supervisado tradicional.

🍄 Dataset Utilizado: Mushroom Dataset

El proyecto utiliza el Mushroom Dataset, un conjunto de datos muy conocido en el ámbito educativo que contiene información sobre diferentes tipos de hongos.

Cada registro describe las características físicas de un hongo (color, forma, tamaño, olor, etc.) junto con su clasificación como comestible o venenoso.

🔹 Fuente: UCI Machine Learning Repository
🔹 Tamaño: 8124 registros y 23 variables categóricas
🔹 Objetivo: entender cómo un modelo no supervisado puede separar las clases sin conocer la etiqueta “comestible/venenoso”.

🎯 Objetivos de Aprendizaje

Comprender la diferencia entre aprendizaje supervisado y no supervisado.

Aplicar técnicas de preprocesamiento de datos: normalización, escalado y codificación.

Implementar PCA para reducir la dimensionalidad y facilitar la visualización.

Realizar agrupamiento (K-Means) y analizar la distribución de los grupos.

Comparar los resultados del modelo no supervisado con un modelo supervisado (Random Forest).

Interpretar los resultados y visualizar las agrupaciones obtenidas.

🧩 Contenido del Notebook

El archivo Proyecto8_Monica_Gomez.ipynb está estructurado en las siguientes secciones:

1️⃣ Introducción Teórica

Breve explicación de los conceptos de aprendizaje supervisado vs. no supervisado y los fundamentos de PCA y K-Means.

2️⃣ Carga y Exploración de Datos

Carga del Mushroom Dataset.

Exploración de sus variables y valores únicos.

Limpieza y codificación de variables categóricas.

3️⃣ Preprocesamiento

Label Encoding / One Hot Encoding para variables categóricas.

Estandarización para normalizar los datos antes de aplicar PCA o K-Means.

4️⃣ Reducción de Dimensionalidad (PCA)

Aplicación de PCA para reducir la cantidad de variables.

Visualización de los componentes principales.

Análisis de la varianza explicada por cada componente.

5️⃣ Agrupamiento (K-Means)

Implementación de K-Means con distintos valores de k.

Evaluación del número óptimo de grupos mediante el método del “codo”.

Visualización de los clusters obtenidos con los componentes principales.

6️⃣ Comparativa con Modelo Supervisado (Random Forest)

Entrenamiento de un modelo Random Forest usando las etiquetas verdaderas.

Comparación de métricas con los resultados del modelo no supervisado.

Reflexión sobre las ventajas y desventajas de ambos enfoques.

7️⃣ Conclusiones

Análisis final de los resultados obtenidos, interpretación de los grupos y discusión sobre las diferencias entre los modelos supervisados y no supervisados.

💻 Librerías Utilizadas
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.preprocessing import LabelEncoder, StandardScaler
from sklearn.decomposition import PCA
from sklearn.cluster import KMeans
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, confusion_matrix

⚙️ Cómo Ejecutar el Proyecto

Clona o descarga este repositorio.

Abre el archivo Proyecto8_Monica_Gomez.ipynb en Jupyter Notebook, JupyterLab o Google Colab.

Ejecuta cada celda en orden para reproducir los resultados.

Observa cómo los datos se transforman, se agrupan y se comparan los modelos paso a paso.

🧠 Conceptos Clave
Concepto	Explicación Simple
Aprendizaje No Supervisado	El modelo aprende sin etiquetas, buscando patrones o agrupaciones.
PCA (Análisis de Componentes Principales)	Reduce la cantidad de variables manteniendo la información más importante.
K-Means	Agrupa los datos según su similitud en k grupos distintos.
Random Forest	Modelo supervisado que utiliza muchos árboles de decisión para clasificar datos.
Escalado	Ajusta los valores numéricos para que tengan una escala similar.
Label/One Hot Encoder	Transforma texto en números para que el modelo pueda procesarlo.
📊 Resultados Esperados

Reducción efectiva de la dimensionalidad mediante PCA.

Agrupamiento visible de hongos comestibles y venenosos sin usar etiquetas.

Comparación clara entre resultados de K-Means y Random Forest.

Comprensión visual de los grupos en los gráficos 2D y 3D de PCA.

📝 Conclusiones

El proyecto demuestra cómo los algoritmos de aprendizaje no supervisado (PCA + K-Means) pueden identificar estructuras ocultas dentro de los datos sin conocer las etiquetas.

Al comparar estos resultados con Random Forest, se observa cómo ambos enfoques ofrecen perspectivas distintas sobre el mismo conjunto de datos:

El modelo supervisado busca la mejor predicción.

El modelo no supervisado busca los patrones naturales que existen en los datos.

Este taller es una excelente forma de comprender cómo funciona el aprendizaje automático desde dos enfoques complementarios.
