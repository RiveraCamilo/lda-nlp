
# Comparación de Topic Modeling (LDA) y Clustering (KMeans)

## Descripción 

Este proyecto corresponde a la Tarea 2 del curso de Procesamiento de Lenguaje Natural, cuyo objetivo es comparar la aplicación de técnicas de **Topic Modeling (LDA)** y **Clustering (KMeans)** sobre un subset del dataset **"El Chile que Queremos"**. Se busca explorar cómo la incorporación de **bigramas** en el análisis puede mejorar la interpretación de tópicos, y contrastar la agrupación temática obtenida con LDA frente a la segmentación estructural de KMeans.


## Estructura del Proyecto

📁 lda_nlp/<br>
├── notebooks/<br>
│ └── tarea2_camilo_rivera.ipynb # Código comentado en Jupyter Notebook<br>
├── data/<br>
│ └── ecqq.csv # Dataset "El Chile que Queremos"<br>
├── requeriments.txt<br>
└── README.md<br>

## Tecnologías Utilizadas

- **Gensim**: Librería para modelado de tópicos (LDA) y procesamiento de n-gramas.
- **Stanza**: Pipeline NLP desarrollado por Stanford para tokenización, POS-tagging y lematización.
- **NLTK**: Toolkit de procesamiento de lenguaje natural, utilizado para stopwords y tokenización.
- **Scikit**-learn: Librería de machine learning, utilizada para clustering (KMeans) y métricas de evaluación (Silhouette Score).

## Pasos del Análisis

### 1. Preprocesamiento del Texto
- Tokenización de los textos.
- Eliminación de stopwords en español.
- Generación de bigramas sobre el corpus.

### 2. Topic Modeling (LDA)
- Construcción de Diccionario y Corpus.
- Evaluación de coherencia para determinar el número óptimo de tópicos.
- Ejecución de LDA con el número seleccionado.
- Etiquetado de tópicos con justificación breve.

### 3. Clustering con KMeans
- Construcción de la Document-Term Matrix (DTM) con unigrams y bigrams.
- Evaluación del número óptimo de clusters utilizando Silhouette Score.
- Comparación de resultados frente al modelo LDA.

## Cómo Ejecutar
1. Clonar este repositorio.
2. Asegurarse de tener las librerías necesarias instaladas:
    ```bash
    pip install -r requirements.txt
    ```
3. Ejecutar el archivo Jupyter Notebook paso a paso.
4. Asegúrate de tener el dataset `el_chile_que_queremos_subset.csv` en la raíz del proyecto (por políticas de privacidad no se incluye en este repositorio).

## Referencias
- [Tutorial Gensim LDA](https://radimrehurek.com/gensim_3.8.3/auto_examples/tutorials/run_lda.html)
- [Scikit-learn Clustering Documentation](https://scikit-learn.org/stable/modules/clustering.html#k-means)

## Notas
Este repositorio fue creado como parte de una tarea académica. El código ha sido comentado para facilitar su comprensión y replicabilidad.

---