# vc2_tpfinal
CEIA FIUBA - Visión por Computadora 2 - TP FINAL

Link de descarga: https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset
 
**Descripción:**
El dataset comprende una serie de imágenes de plantas de diferentes especies en estado sano "healthy" y con diversas patologías.

El objetivo del presente trabajo es la aplicación de modelos de Deep Learning de Visión por Computadora para clasificación de imágenes.

El enfoque aplicado para el dataset en cuestión consiste en hacer una Clasificación Multi-Output donde una de las salidas es la especie de planta (Multi-label, 14 opciones disponibles) y la otra, su estado de salud (Binario: Healthy o Diseased).

Este repositorio presenta 2 notebooks:

- **Plant_Disease_Detection_v2.ipynb**. Se enfoca el modelo multi-output con un único modelo que devuelve las dos clasificaciones (especie de planta y estado de salud). Contiene:
1) EDA
2) Modelo #1: Baseline Simple CNN
3) Modelo #2: Baseline Simple CNN with RandAugmentation.
4) Modelo #3: Pre-Trained RESNET 18. Se mantienen congeladas las capas convoluciones y se entrenan solo las cabezas de clasificación (feature extraction approach).
5) Modelo #4: RESNET18 Fully-trained. Se entran toda la red completamente. Se presenta la matriz de confusión y el classification report.
7) Comparación de modelos y conclusiones.

- **Proportional_separated.ipynb**. Se enfoca el problema de manera desacoplada, teniendo dos modelos independientes para clasificar la especie de planta y el estado de salud, respectivamente.

