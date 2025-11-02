🧠 Proyecto 8 – Aprendizaje No Supervisado con PCA y Clustering
📚 Descripción
Análisis práctico de aprendizaje automático no supervisado aplicado al dataset de hongos. El proyecto explora cómo identificar patrones y agrupaciones sin usar etiquetas, comparando los resultados con un modelo supervisado.
Técnicas Implementadas

🧩 PCA — Reducción de dimensionalidad preservando máxima varianza
🔷 K-Means — Agrupamiento automático por similitud
🌳 Random Forest — Modelo supervisado para comparación


🍄 Dataset: Mushroom Classification
Fuente: UCI Machine Learning Repository

📊 Registros: 8,124 hongos
🔢 Variables: 23 atributos categóricos (color, forma, olor, textura, etc.)
🎯 Clases: Comestible vs. Venenoso

Desafío: ¿Puede un modelo no supervisado separar hongos comestibles de venenosos usando solo características físicas?

🎯 Objetivos

Comprender la diferencia entre aprendizaje supervisado y no supervisado
Aplicar técnicas de preprocesamiento de datos categóricos
Implementar PCA para visualización y reducción dimensional
Aplicar K-Means y determinar el número óptimo de clusters
Comparar resultados con Random Forest


📂 Estructura del Notebook
Proyecto8_Monica_Gomez.ipynb

Fundamentos Teóricos - Conceptos de PCA y K-Means
Exploración de Datos - Carga y análisis del dataset
Preprocesamiento - Encoding y normalización de variables
PCA - Reducción dimensional y análisis de varianza explicada
K-Means - Clustering con método del codo y visualización
Random Forest - Modelo supervisado y comparación de métricas
Conclusiones - Interpretación y análisis comparativo


💻 Librerías Utilizadas
pythonimport pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.preprocessing import LabelEncoder, StandardScaler
from sklearn.decomposition import PCA
from sklearn.cluster import KMeans
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, confusion_matrix, silhouette_score

⚙️ Cómo Ejecutar
bash# Instalar dependencias
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Clonar repositorio
git clone [URL_DEL_REPOSITORIO]

# Abrir notebook
jupyter notebook Proyecto8_Monica_Gomez.ipynb
Ejecuta cada celda secuencialmente para reproducir el análisis completo.

📊 Resultados Esperados
✅ Reducción de 23 variables a 2-3 componentes (>85% varianza explicada)
✅ Identificación de 2 clusters principales sin supervisión
✅ Alta correspondencia entre clusters y clases reales (~90%)
✅ Visualizaciones 2D/3D interpretables de las agrupaciones
✅ Comparación cuantitativa: K-Means vs Random Forest

📈 Conclusiones
El proyecto demuestra que PCA + K-Means puede identificar estructuras naturales en los datos sin etiquetas previas. La comparación con Random Forest revela:

Supervisado: Mayor precisión predictiva, requiere datos etiquetados
No Supervisado: Descubre patrones intrínsecos, útil para exploración

Este enfoque es aplicable a segmentación de clientes, análisis médico exploratorio, detección de anomalías y clasificación de datos sin etiquetar.

👤 Autora
Mónica Gómez

📚 Referencias

UCI Machine Learning Repository - Mushroom Dataset
Scikit-learn Documentation


⭐ Si este proyecto te resulta útil, considera darle una estrella
