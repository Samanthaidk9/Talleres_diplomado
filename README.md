#Talleres del Módulo 4: Machine Learning Aplicado

##Taller Regresión Lineal

Se trabajó con el dataset daily-bike-share, que muestra el número de bicicletas alquiladas por día.
Primero se exploraron los datos y se identificó la variable objetivo rentals.
Luego se seleccionaron variables numéricas relevantes: temp, atemp, hum y windspeed.

Se entrenó un modelo de regresión lineal multivariable para predecir rentals y se evaluó con métricas como MSE y RMSE, obteniendo un RMSE = 595, lo que indica una buena precisión.

También se probó un modelo con solo temp, cuyo RMSE fue 611 y R² = 0.26, demostrando menor exactitud.

##Taller Arboles de decision.

Se utilizó el Wine Dataset para predecir la clase de vino según variables químicas.
Se exploraron los datos con gráficos y una matriz de correlación, luego se dividieron en entrenamiento, validación y prueba.
Se entrenó un árbol de decisión y se evaluó con accuracy y matrices de confusión.
Tras ajustar parámetros como criterion="entropy" y max_depth=5, el modelo alcanzó un buen equilibrio entre precisión y generalización, clasificando correctamente la mayoría de los vinos.

##Taller K-Means

Se realizaron los siguientes cambios: 
###Corrección de Datos Esencial: Se corrigió la selección de características para incluir las 7 columnas de atributos geométricas (area hasta groove_length), en lugar de solo 6.
Esto garantiza que el modelo utilice toda la información disponible.
###Validación Metodológica de $K$: Se implementó el Método del Codo para validar objetivamente que $K=3$ es 
el número óptimo de clústeres, confirmando que el algoritmo encuentra las tres especies de trigo.
###Evaluación Cuantitativa: Se añadieron métricas de rendimiento numéricas 
como puntuación de la Silueta y el Índice de Rand Ajustado - ARI para cuantificar la calidad del agrupamiento y su coincidencia con las etiquetas reales.
