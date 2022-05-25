# Predicción del Precio de Carros Usando Machine Learning.

Por: Susana Álvarez Zuluaga, Camilo Cossio Alzate, Juan Pablo Madrid Peláez y Mariajose Franco Orozco.

En este repositorio se pueden encontrar todos los recursos utilizados en el desarrollo del proyecto. El lenguaje de programación utilizado fue Python. Para la ejecución de los algoritmos solamente es necesario contar con los archivos .xlsx y .csv en la misma carpeta donde se encuentren los archivos a correr, no es necesario modificar nada. A continuación una breve descripción de los contenidos.

# Contenido

- **carData.csv:** Archivo con los datos obtenidos de la API de Mercado Libre.
- **datos_procesados.xlsx:** Archivo con las variables a tomar en cuenta para el estudio.
- **data.xlsx:** Archivo con los datos listos para ser usados en la realización de los modelos propuestos.
- **X_train.xlsx:** Archivo con los datos de las variables X del conjunto train. Este conjunto se obtuvo utilizando la función de train_test_split de la librería sklearn. El conjunto de train tiene el 75% de los datos. 
- **y_train.xlsx:** Archivo con los datos de la variable Y (precio) del conjunto train. 
- **X_test.xlsx:** Archivo con los datos de las variables X del conjunto test. Este conjunto tiene el 25% de los datos. 
- **y_test.xlsx:** Archivo con los datos de la variable Y (precio) del conjunto test. 
- **ProcesamientoDatosCrudos.ipynb:** Notebook utilizado para procesar los datos contenidos en "carData.csv" con el fin de dar formato a cada una de las variables de interés en el estudio. La salida del algoritmo es un archivo Excel llamado "datos_procesados.xlsx".
- **LimpiezaDatos.ipynb:** Notebook utilizado para preparar los datos con el fin de que puedan ser utilizados en la realización de modelos de prediccion. Se crean las variables Dummies necesarias, se pasa a binario las variables categóricas con 2 categorías, se transforman ciertas variables y se eliminan outliers. Recibe como entrada el archivo "datos_procesados.xlsx" y la salida es "data.xlsx".
- **Linear_Regression.ipynb:** En este notebook se encuentra la implementación del algoritmo Linear Regression. Este algoritmo se implementó como una base para comparar los resultados obtenidos con este modelo y con los demás modelos. 
- **random_forest.ipynb:** En este notebook se encuentra la implementación del algoritmo Random Forest Regression con el objetivo de estimar el precio de vehículos usados a partir de ciertas características, se calculan los errores y se realiza una validación cruzada usando k-folds. Recibe como entrada el archivo "data.xlsx" y la salida es el modelo.
- **Support_Vector_Regression.ipynb:** En este notebook se encuentra la implementación del algoritmo Support Vector Regression con el objetivo de estimar el precio de vehículos usados a partir de ciertas características. Se obtienen diferentes modelos variando hiper parametros. 

