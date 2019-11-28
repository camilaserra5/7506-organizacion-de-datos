# 7506-organizacion-de-datos tp2

Los features están dentro de la carpeta features. Hay una notebook general que es la que genera el csv final a usar como modelo: feature-main.
Para crear un nuevo features, evaluar si va dentro de alguna de las notebooks ya existentes, y si no crear una nueva: feature_xxx
Todas las notebooks de features tienen una estructura similar. Primero, unen los datasets de train y test, luego hacen las columnas con los features a utilizar. Por último, estas columnas de exportan a un csv con el nombre de la notebook. 
Importante: este df a exportar tiene que tener la columna id, y no tiene que tener la columna precio. Van a ser de la forma: id|feature1|feature2|.. . Estos features deben ser columnas numéricas.

Para general el modelo final con todos estos features, ir a feature-main y agregar para que la notebook se corra, se lea el csv generado y se concatene con los demás. Nota: el df de todos los features debe tener 300000 filas (shape = 300000 x lo que sea)

En la carpeta modelos, estarán los distintos algoritmos utilizados. En general, para no perder los modelos, lo ideal es crear notebooks nuevas hasta estar seguros d que funciona. Por ej: ya hay un xgboost pero yo lo quiero mejorar, copió la notebook, la renombro, y hago mis modificaciones / agregaciones sobre esa. 

catboost
naive bayes
random forest

Posibles a hacer:
adaboost
light gbm
logistic regression
ensambles d algunos
feature selection (forward o backward)
xgboost con mas variaciones


Respecto de las features:
-

Normalizar los datos para modelos que funcionen mejor con valores entre 0 y 1 (Cuando pueda lo implemento)
Generar variaciones sobre las features más importantes (Cuando pueda lo implemento)
Tratamiento de Outliers (Cuando pueda lo implemento)
