# Tecnologías de información emergentes: NLP

# Actividad Integradora 2

_Clasificador de sentimientos de tweets (positivos y negativos)._

## Requerimientos ⚙️

El código está desarrollado en un Jupyter Notebook con Python 3. Igualmente, se pueden instalar las dependencias usando el archivo del repositorio requirements.txt

> pip install -r requirements.txt

* scikit-learn ***
* pandas ***
* numpy ***
* matplotlib ***

## ¿Qué hace el proyecto? 📄

El proyecto se trata de un analizador de sentimientos de tweets publicados en la red social "Twitter" en tiempo real. Específicamente, clasifica los tweets como positivos o negativos. Posteriormente, despliega una gráfica del análisis realizado a los tweets.

## ¿Cómo funciona el clasificador? 📄

### 1. Ingreso de datos de entrada  📦

D

Una vez que se descargan las imágenes, son guardadas en distintas carpetas que serán usadas para el resto del proceso. Los tweets de cada clasificación son separadas en carpetas train con 70% de datos, test con 20% de datos y validation con 10% de datos.

### 2. Data augmentation (no sé si aplique) 💻

El programa usa dos técnicas de data augmentation para generar más datos en el dataset de entrenamiento. Esta fase consta en buscar las imágenes ya ordenadas dentro de la carpeta train para cada una de las categorías hamburguer, pasta, pizza, salad y tuna. Por cada una de las imágenes que encuentra en las carpetas, usa las herramientas RandomFlip y RandomRotation para generar más imágenes de entrenamiento y las guarda en las mismas carpetas.

### 3. Modelos de entrenamiento 🛠️ 

Este clasificador tiene la opción de usar 2 modelos: VGG16 o MobileNet. Además, podrá elegir la cantidad de epochs para el entrenamiento.

**El usuario deberá escribir "1" para ver el modelo VGG16 o "0" para ver el modelo MobileNet. El usuario luego eligirá la cantidad de Epochs que se usarán para entrenar el modelo.**

En el modelo VGG16 se quitó la última capa, y se agregó una nueva capa de 5 nodos como salida para que genere las clasificaciones de las nuevas categorías "hamburguer, pasta, pizza, salad y tuna". Finalmente se dejó como entrenable únicamente la última capa.

En el modelo MobileNet se quitaron las últimas 5 capas, se agregó una nueva capa de 5 nodos como salida para las clasificaciones de las nuevas clases. Finalmente se dejaron como entrenables únicamente las últimas 23 capas.

### 4. Regularización del modelo 🚀

Este modelo usa regularización l1_l2. Esta estrategia penaliza los parámetros que causan overfitting en el modelo.

## ¿Por qué el proyecto es de utilidad? 📄

Por un lado, el proyecto es de gran utilidad para conocer la tendencia emocional en ciertas regiones en tiempo real. Por otro lado, sirve para conocer la utilidad y funcionamiento de distintas librerías enfocadas en el pre-procesamiento y análisis de textos; en especial, la librería NLTK.

## Observaciones

Ejemplo: Las pruebas se hicieron con los resultados de imágenes de shutterstock con las palabras "hamburger, pasta, pizza, salad, tuna", estas palabras deben ser usadas para que funcione el código como está escrito en el repositorio, ya que en algunas partes del código tiene escritas las palabras específicamente. Para mejorar los resultados de las búsquedas se puede usar un término de búsqueda mejor como "pasta food" que tendría que escribirse de igual manera en las partes del código que lo requieran para usar mejores resultados de imágenes.

## Autores 📝

_Equipo #3._

* **Carlos Adrián Guerra Vázquez**
* **Omar Osvaldo Hernández Díaz**
* **Jesús Carlos Martínez González**
* **Luis Miguel Maawad Hinojosa**
* **Juan Edgar Juarez Mendoza**
