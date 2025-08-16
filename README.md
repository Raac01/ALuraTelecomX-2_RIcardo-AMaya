# ALuraTelecomX-2_RIcardo-Amaya
*Propósito del análisis*

El objetivo principal de este proyecto es predecir la cancelación de clientes (churn) en base a variables relevantes, identificando los factores que más influyen en la decisión de los usuarios de dejar el servicio.
Este análisis busca no solo generar un modelo predictivo, sino también proponer estrategias de retención basadas en los resultados obtenidos.

 # Proceso de preparación de los datos

1.Clasificación de variables

* Categóricas: género, tipo de contrato, método de pago, uso de servicios adicionales, etc.

* Numéricas: tiempo de permanencia (tenure), cargos mensuales, cargos totales, etc.

2.Normalización y codificación

* Se aplicó One-Hot Encoding para variables categóricas nominales.

* Se aplicó Label Encoding en variables binarias (por ejemplo: género, churn).

* Las variables numéricas fueron escaladas con StandardScaler para mejorar el rendimiento en algoritmos sensibles a la magnitud.

3.Separación en conjuntos de datos

* 80% entrenamiento y 20% prueba, para evaluar el rendimiento real de los modelos.

* Se usó stratified split para mantener la proporción de clases (churn/no churn).

4.Justificación de decisiones

* La codificación de variables categóricas se eligió según el tipo (nominal u ordinal).

* La normalización se aplicó porque algunos modelos (ej. SVM, KNN) son sensibles a escalas distintas.

* Se evaluaron diferentes modelos (Regresión Logística, Random Forest) para comparar desempeño.

# Estrategias de retención propuestas

En base al análisis, se sugieren las siguientes acciones:

* Fidelización con contratos anuales o semestrales, reduciendo la dependencia de contratos mensuales.

* Incentivos para clientes nuevos, dado que el tenure bajo está asociado a mayor churn.

* Planes flexibles y promociones para clientes con cargos mensuales altos, reduciendo la percepción de costo.

* Fomentar métodos de pago automáticos, que mostraron menor tasa de cancelación.

# Librerias Utilizadas
* pandas

* numpy

* matplotlib / seaborn

* sklearn
