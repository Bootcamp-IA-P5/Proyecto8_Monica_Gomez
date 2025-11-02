# 🧠 Aprendizaje No Supervisado con PCA y Clustering

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Latest-orange.svg)
![License](https://img.shields.io/badge/License-Educational-green.svg)

*Descubriendo patrones ocultos en datos sin etiquetas*

[Descripción](#-descripción) • [Dataset](#-dataset) • [Instalación](#️-instalación) • [Resultados](#-resultados)

</div>

---

## 📚 Descripción

Análisis práctico de **aprendizaje automático no supervisado** aplicado a la clasificación de hongos. Este proyecto explora cómo identificar patrones naturales en los datos sin necesidad de etiquetas previas.

### 🔬 Técnicas Implementadas

| Técnica | Propósito |
|---------|-----------|
| 🧩 **PCA** | Reducción de dimensionalidad preservando varianza |
| 🔷 **K-Means** | Agrupamiento automático por similitud |
| 🌳 **Random Forest** | Benchmark supervisado para validación |

---

## 🍄 Dataset

### Mushroom Classification Dataset

> 📍 **Fuente:** UCI Machine Learning Repository

```
📊 8,124 registros de hongos
🔢 23 atributos categóricos
🎯 2 clases: Comestible | Venenoso
```

**Características:** color del sombrero, forma del tallo, olor, textura, hábitat, tamaño de anillo, tipo de branquias...

**Pregunta clave:** *¿Puede un algoritmo separar hongos tóxicos de comestibles basándose únicamente en patrones visuales, sin conocer las etiquetas?*

---

## 🎯 Objetivos del Proyecto

- [x] Comprender aprendizaje supervisado vs no supervisado
- [x] Aplicar preprocesamiento de variables categóricas
- [x] Implementar PCA para reducción dimensional
- [x] Determinar clusters óptimos con método del codo
- [x] Validar resultados con modelo supervisado

---

## 📂 Contenido del Notebook

```
Proyecto8_Monica_Gomez.ipynb
│
├── 1️⃣ Fundamentos Teóricos
│   └── Conceptos de PCA y K-Means
│
├── 2️⃣ Exploración de Datos
│   └── Análisis y visualización inicial
│
├── 3️⃣ Preprocesamiento
│   └── Encoding y normalización
│
├── 4️⃣ Análisis PCA
│   └── Reducción dimensional y varianza
│
├── 5️⃣ Clustering K-Means
│   └── Agrupamiento y evaluación
│
├── 6️⃣ Random Forest
│   └── Modelo supervisado y comparación
│
└── 7️⃣ Conclusiones
    └── Interpretación de resultados
```

---

## 🛠️ Stack Tecnológico

```python
# Data Science Stack
pandas | numpy | matplotlib | seaborn

# Machine Learning
scikit-learn
  ├── PCA
  ├── K-Means
  ├── Random Forest
  └── Preprocessing Tools
```

---

## ⚙️ Instalación

### Requisitos

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Ejecución

```bash
# 1. Clonar repositorio
git clone [URL_DEL_REPOSITORIO]
cd proyecto8-pca-clustering

# 2. Abrir notebook
jupyter notebook Proyecto8_Monica_Gomez.ipynb

# 3. Ejecutar celdas secuencialmente
```

---

## 📊 Resultados

### Métricas Alcanzadas

| Métrica | Valor |
|---------|-------|
| 📉 Reducción dimensional | 23 → 2-3 componentes |
| 📈 Varianza explicada | >85% |
| 🎯 Concordancia clusters-clases | ~90% |
| 🌟 Accuracy Random Forest | >95% |

### Visualizaciones Clave

- ✅ Gráficos 2D/3D de componentes principales
- ✅ Método del codo para selección de k
- ✅ Distribución de clusters vs clases reales
- ✅ Matriz de confusión comparativa

---

## 💡 Conclusiones

### Hallazgos Principales

🔍 **Separabilidad Natural**  
Los hongos comestibles y venenosos presentan patrones distinguibles en sus características físicas, detectables sin supervisión.

🎯 **Validación Cruzada**  
Alta correspondencia entre clusters no supervisados y clases reales, confirmando la calidad del agrupamiento.

⚖️ **Comparativa de Enfoques**

| Aspecto | No Supervisado | Supervisado |
|---------|----------------|-------------|
| Precisión | ~90% | >95% |
| Etiquetas necesarias | ❌ No | ✅ Sí |
| Descubrimiento | ✅ Patrones nuevos | ❌ Solo predicción |
| Uso ideal | Exploración | Clasificación |

### Aplicaciones

Este framework es útil para:
- 🧬 Segmentación de datos médicos sin diagnóstico
- 🛒 Clustering de comportamiento de clientes
- 🔬 Análisis exploratorio de datasets científicos
- 🌐 Detección de anomalías en sistemas

---

## 📖 Glosario Rápido

| Término | Definición |
|---------|------------|
| **PCA** | Proyección de datos en direcciones de máxima varianza |
| **K-Means** | Particiona datos en k grupos minimizando distancias |
| **Encoding** | Conversión de categorías a valores numéricos |
| **Escalado** | Normalización de features a rangos comparables |
| **Método del Codo** | Técnica para determinar número óptimo de clusters |

---

## 👤 Autora

**Mónica Gómez**  
*Data Science Project | Machine Learning*

---

## 📚 Referencias

- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/mushroom)
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [PCA Explained](https://scikit-learn.org/stable/modules/decomposition.html#pca)

---

## 📄 Licencia

Este proyecto tiene fines educativos. Dataset bajo licencia UCI ML Repository.

---

<div align="center">

**⭐ Si este proyecto te resulta útil, considera darle una estrella ⭐**

*Desarrollado con* 💜 *para aprender Machine Learning*

</div>
