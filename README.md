# ML Disaster Tweets — NLP Classification

Proyecto de Machine Learning y Procesamiento de Lenguaje Natural (NLP) cuyo objetivo es
clasificar tweets según si refieren a un desastre real o no, utilizando distintos enfoques
de modelado y feature engineering.

El trabajo se basa en la competencia de Kaggle  
**Natural Language Processing with Disaster Tweets**  
https://www.kaggle.com/competitions/nlp-getting-started

---

## 📌 Objetivo

Dado un conjunto de tweets, predecir si el contenido está basado en un hecho real
(`target = 1`) o no (`target = 0`), utilizando técnicas de Machine Learning supervisado
y NLP.

---

## 📊 Dataset

El dataset provisto por Kaggle contiene las siguientes columnas:

- `id`: identificador único del tweet  
- `text`: texto del tweet  
- `location`: ubicación desde donde fue enviado (opcional)  
- `keyword`: palabra clave asociada al tweet (opcional)  
- `target`: variable objetivo (solo en `train.csv`)  

---

## 🧪 Estructura del Proyecto

El trabajo fue desarrollado de manera modular y reproducible, separando cada etapa
en notebooks independientes:

- **Exploratory Data Analysis (EDA)**  
  Visualizaciones para analizar la relación entre las variables y el target.

- **Baseline Model**  
  Modelo de regresión logística con features numéricas y categóricas, utilizado como
  referencia inicial.

- **Machine Learning Models**  
  Entrenamiento de modelos más complejos con búsqueda de hiperparámetros y validación
  basada en F1-score.

---

## 🔍 Parte I — Análisis Exploratorio

- Análisis del target y su distribución
- Visualizaciones explicativas y legibles
- Relación entre keywords, longitud del texto y ocurrencia de desastres

---

## ⚙️ Parte II — Baseline Model

- Regresión logística
- Features numéricas y categóricas
- Embedding del texto
- Búsqueda de hiperparámetros
- Validación reproducible
- Análisis de importancia de features

Este modelo se utilizó como referencia para evaluar la complejidad del problema y
comparar el desempeño de modelos más avanzados.

---

## 🤖 Parte III — Modelos de Machine Learning

Se entrenaron distintos modelos (excluyendo regresión logística), cumpliendo las
siguientes condiciones:

- Métrica de validación: **F1-score**
- Validación independiente del set de test
- Reproducibilidad garantizada
- Feature engineering con:
  - One-Hot Encoding
  - Mean Encoding
- Resultados superiores a **0.80 de F1 en validación**

Para los mejores modelos se analizaron:
- Curva ROC
- Matriz de confusión
- Importancia de features

---

## 🚀 Parte IV — Extensiones

Como parte adicional del trabajo, se exploraron enfoques avanzados como:

- Reducción del número de features manteniendo alto desempeño
- Modelos con embeddings de texto
- Visualización de embeddings mediante técnicas de reducción de dimensionalidad

---

## 📈 Resultados

Los modelos desarrollados alcanzaron un desempeño competitivo tanto en validación
como en la competencia de Kaggle, demostrando la efectividad del feature engineering
y la selección de modelos.

Los archivos de predicción (`submission.csv`) fueron generados siguiendo el formato
requerido por la competencia.

---

## 🛠️ Tecnologías Utilizadas

- Python
- Pandas, NumPy
- Scikit-learn
- NLP & Text Preprocessing
- Kaggle Notebooks

---

## 📚 Contexto Académico

Trabajo Práctico N.º 3 — **Ciencia de Datos**  
Cátedra Martinelli  
Universidad de Buenos Aires

---

## ✍️ Autor

**Manuel Pueyrredon**  
Estudiante de Ingeniería Informática (UBA)  
GitHub: https://github.com/ManuPueyUba
