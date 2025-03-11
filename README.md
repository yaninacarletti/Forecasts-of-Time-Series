# Forecasts-of-Time-Series

El siguiente notebook busca analizar y comprender como las ventas de una empresa evolucionan a lo largo del tiempo.
Si existe o no algún patrón subyacente en los datos que determine la presencia de una estacionalidad. En caso de que ese fuese el caso, ¿con qué frecuancia se manifiesta? 
¿Los datos exiben alguna tendencia en el tiempo? ¿Creciente? ¿Decreciente?
¿Estamos tratando con una serie estacionaria o no estacionaria? Prerequisito indispensable para la aplicabilidad de muchos de los modelos de series temporales.

Concretamente, en una primera instacia se determina el período de tiempo que comprende la serie, para luego  
proseguir con su ploteo  y posterior descomposición de la misma.
En una segunda instancia se busca determinar si la serie temporal es estacionaria o no para luego indagar si posee alguna estacionalidad detectable. En base a lo anterior, se aplican tres enfoques distintos para su estudio, a saber:
1) Un modelado con ARIMA, previa determinación de parámetros mediante 'ADF Test' y gráficas 'ACF' y 'PACF'.
2) Un modelado con ARIMA junto a una optimización con Gridsearch buscando minimizar el criterio de información de akaike, AIC.
3) Un modelado con AutoARIMA.
  Finalmente, se presenta un reporte comparativos con las distintas métricas empleadas para evaluar el rendimiento de los modelos/ enfoques analizados.
  Se arriba a la conclusión de que la serie bajo estudio es estacionaria, es decir, sus propiesdades estadísticas no exiben variación con el tiempo. Presenta una estacionalidad anual, repitiéndose el mismo patrón en las ventas año trás año con una tendencia creciente. Siendo el primer enfoque analizado, el que presenta menor error y por ende, un mayor ajuste a los datos reales. Por lo que es el enfoque que se propone se emplee en la generación de nuevos pronosticos.
  
