# Tecnologías de información emergentes: NLP

# Actividad Integradora 2

_Clasificador de sentimientos de tweets_

## Requerimientos ⚙️

El código está desarrollado en un Jupyter Notebook con Python 3. Igualmente, las siguientes dependencias son requeridas:

* import nltk
* import pickle
* from nltk.classify.scikitlearn import SklearnClassifier
* from sklearn.naive_bayes import MultinomialNB, GaussianNB, BernoulliNB
* from sklearn.linear_model import LogisticRegression, SGDClassifier
* from sklearn.svm import SVC, LinearSVC, NuSVC
* from nltk.classify import ClassifierI
* from statistics import mode

## ¿Qué hace el proyecto? 📄

El proyecto se trata de un analizador de sentimientos de tweets publicados en la red social "Twitter" en tiempo real. Específicamente, clasifica los tweets como positivos o negativos. Posteriormente, despliega una gráfica del análisis realizado a los tweets.

## ¿Cómo funciona el clasificador? 📄

El clasificador recibe como entrada los tweets de la red social "Twitter" para ulteriormente dividerlos en sets de datos de entrenamiento y validación. Los clasifica de acuerdo a una herramienta de filtrado especial encontrada en la librería NLTK. Finalmente, los gráfica.

## ¿Por qué el proyecto es de utilidad? 📄

Por un lado, el proyecto es de gran utilidad para conocer la tendencia emocional en ciertas regiones en tiempo real. Por otro lado, sirve para conocer la utilidad y funcionamiento de distintas librerías enfocadas en el pre-procesamiento y análisis de textos; en especial, la librería NLTK.

## Observaciones

La ultima parte del projecto de graficar los resultados del clasificador en tiempo real no se pudo ejecutar en una jupyter notebook, pero se agregó el código en su propio archivo "animation.py" el cual se puede correr mientras se ejecuta la clasificación de los tweets para asi poder ver en tiempo real los resultados. 

Para la correcta ejecución del código, se necesita del archivo "./pickled_algos/featuresets.pickle". Este archivo era muy grande para subir a github, y por lo tanto se tiene que descargar desde este link: https://drive.google.com/file/d/1czdguArJIUFA0dW-hL-bau6nKrZRKDTb/view?usp=sharing
Cabe destacar que, "featuresets.pickle" se debe de agregar al directorio "./pickled_algos".

## Autores 📝

_Equipo #3:_

* **Carlos Adrián Guerra Vázquez**
* **Omar Osvaldo Hernández Díaz**
* **Jesús Carlos Martínez González**
* **Luis Miguel Maawad Hinojosa**
* **Juan Edgar Juarez Mendoza**
