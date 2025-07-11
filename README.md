# ML_Vehicle_Price
## Introducción
En este proyecto se busca poder predecir el precio de un vehículo mediante una serie de características del mismo para esto se utilizó el dataset público [Vehicle Price](https://www.kaggle.com/code/sahilislam007/vehicle-price-prediction/input) el cual mediante el enlace se puede acceder a la página en Kaggle.
Este dataset cuenta con 17 variables incluyendo al precio, y 1002 registros.
Mediante el uso de Python con tecnicas de Machine Learning y comparación de las mismas se ha logrado crear un módulo que pueda predecir con un Error Porcentual Absoluto Medio, mejor conocido como MAPE, del 11%.

## Desarrollo
En primer lugar se ha procedido a una limpieza del dataset, se han rellenado valores nulos en variables como cylinders, que se refiere a los cilindro que tiene un motor, con valores que coherentes como en este caso 0 debido a que los valores nulos eran porque en el dataset hay carros electricos los cuales no necesitan cilindros.
Luego de realizar una limpieza exhaustiva del dataset procedi a cambiar a "otros" algunos valores de variables categoricas que tenian una frecuencia relativa menor al 0.01 para así bajar la cardinalidad y poder trabajar mejor con las variables.
Al terminar procedí a la division del dataset para hacer los análisis univariante y bivariante de las variables sin verme muy sesgado por conocimientos previos.
De los analisis se puede destacar que los coches en su mayoría son nuevos, que el precio tiene una gran varianza por outliers y esta sesgado a la derecha. Por otro lado, predominan en el data set los de clase SUV, los que tienen 4 puertas y tienen color interior negro.

Luego gracias a la librería de scikit learn la cual permite usar Regresiones Lineales, Arboles de decisión y Radom Forest, y otras librerías como XGBoost, LightGBM y CatBoost que permiten entrenar modelos para que puedan hacer predicciones de una variable target que sea numérica, pude generar un modelo ganador que prediga con un MAPE del 11% el precio de un vehículo.

## Conclusión
Si quieres ver las comparaciones y sacar tus propias conclusiones te invito a ejecutar el notebook main el cual te ira guiando por los pasos realizados hasta llegar al modelo ganador.
