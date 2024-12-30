# Predicción_para_determinar_el_valor_de_mercado_de_un_coche
Creación de un modelo que determine el valor en el mercado de un coche para poder venderlo de segunda mano en una app
# Introducción
Rusty Bargain es un servicio de venta de coches de segunda mano que está desarrollando una app para atraer a nuevos clientes. Gracias a esta app, podemos averiguar rápidamente el valor de mercado de un coche. Tenemos acceso al historial, especificaciones técnicas, versiones de equipamiento y precios. La tarea es crear un modelo que determine el valor del mercado.

A Rusty Bargain le interesa:

- **La calidad de la predicción**
- **La velocidad de la predicción**
- **El tiempo requerido para el entrenamiento**
# Descripción de los datos
El dataset está almacenado en el archivo /datasets/car_data.csv

**Características:**

- `DateCrawled` — fecha en la que se descargó el perfil de la base de datos
- `VehicleType` — tipo de carrocería del vehículo
- `RegistrationYear` — año de matriculación del vehículo
- `Gearbox` — tipo de caja de cambios
- `Power`— potencia (CV)
- `Model` — modelo del vehículo
- `Mileage` — kilometraje (medido en km de acuerdo con las especificidades regionales del conjunto de datos)
- `RegistrationMonth`  — mes de matriculación del vehículo
- `FuelType`  — tipo de combustible
- `Brand` — marca del vehículo
- `NotRepaired`  — vehículo con o sin reparación
- `DateCreated` — fecha de creación del perfil
- `NumberOfPictures` — número de fotos del vehículo
- `PostalCode` — código postal del propietario del perfil (usuario)
- `LastSeen` — fecha de la última vez que el usuario estuvo activo

**Objetivo:**

- `Price` — precio (en euros)
# Habilidades técnicas
- `Phyton`
- `Pandas`
- `Numpy`
- `Matplotlib 
- `Scikit-learn`
- `Descenso de gradiente`
- `Potenciación de gradiente`
- `Calcular la complejidad computacional de los algoritmos`
# Conclusión General
## Comparativa de Modelos:

**1.Calidad del Modelo:**

- **Random Forest:** RMSE de 1527.11

- **XGBoost:** RMSE de 1528.07 (una unidad de diferencia)

**2.Tiempo de Entrenamiento:**

- **Random Forest:** 6.44 ms

- **XGBoost:** 6.44 ms

**3.Velocidad de Predicción:**

- Random Forest: 6.68 ms

- XGBoost: 6.2 ms (0.66 ms más rápido)

**4.Otros Modelos por Calidad:**

- CatBoost

- LightGBM

- DecisionTree

- LinearRegression

En resumen, **Random Forest** fue el mejor en términos de calidad con un RMSE más bajo, mientras que **XGBoost** fue más rápido en la predicción. CatBoost, LightGBM, DecisionTree y LinearRegression le siguieron en calidad, respectivamente.

