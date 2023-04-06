# Modelo para elegir la región petrolera con el mayor margen de beneficio

La compañía minera OilyGiant requiere encontrar el mejor lugar para un nuevo pozo. Para elegir la ubicación se debe:
- Recolectar los parámetros del pozo de petróleo en la región seleccionada: calidad del petróleo y volumen de reservas;
- Construir un modelo para predecir el volumen de reservas en los nuevos pozos;
- Selecciona los pozos de petróleo con los valores estimados más altos;
- Elige la región con el mayor beneficio total para los pozos de petróleo seleccionados.


## Objetivo

- Crear un modelo que ayude a elegir la región con el mayor margen de beneficio. 
- Analiza los beneficios y riesgos potenciales utilizando la técnica bootstrapping.

## Contenido 

* Introducción
* Prepara los datos
* Procesamiento los datos
* Exploración de datos
* Entrenamiento de modelos predictivos por región
* Cálculo de ganancias
* Evaluación de riesgos
* Conclusión general

## Librerias usadas

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

from sklearn.preprocessing   import StandardScaler
from sklearn.model_selection import train_test_split
from sklearn.linear_model    import LinearRegression
from sklearn.metrics         import mean_squared_error
from sklearn.metrics         import r2_score