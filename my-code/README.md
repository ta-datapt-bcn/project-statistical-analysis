
---
<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>
---

# Análisis de House Prices
*Jorge Alvarez - Data Analitics Part-Time*

## Contenido
- [Descripción del proyecto](#description)
- [Hypotesis / Preguntas](#question)
- [Exploración y Limpieza](#exp_clean)
- [Análisis del DataSet](#analytics)
- [Test de Hipótesis](#h_test)
- [PCA](#pca)
- [Probabilidad](#)
- [Links](#link)

<a name="description"></a>
## Descripción del proyecto

El proyecto se basa en un DatasSet de venta de casas. Se pretenden buscar insigths que permitan entender mejor el mercado de compra/venta de casas.

<a name="question"></a>
## Hipotesis / Preguntas
- Que correlación tiene el precio de venta con las diferentes variables
- Cuál es el precio medio y los cuartiles por barrio
- Cuál es el precio medio por cantidad de habitaciones
- Como es la correlación y la línea regresión entre el SalePrice y el LotSize
- ¿El precio medio por FT2 de “NoRidge” es mayor a la del resto de barrios?
- Que probabilidad existe de que una casa tenga más de 2 habitaciones siendo que esta se encuentra en cada uno de los barrios.

<a name="exp_clean"></a>
## Exploración y Limpieza

El DataSet presenta algunas columnas con una gran falta de datos (LotFrontage, Alley, Fence, FireplaceQu, PoolQC, MiscFeature) ninguna de las anteriores columnas representan datos significativamente importantes para este análisis, por esta razón serán eliminadas.

También se encuentran algunas columnas que con un faltante del entorno del 5% de los datos (entre 10 y 80 filas), estas columnas no son de extremada relevancia, por lo que se mantendrán para futuros análisis.

<a name="analytics"></a>
## Análisis del  DataSet

- La distribución de precios tiene una leve tendencia a la izquierda, observando una tendencia de precios más altos. Así como también una gran cantidad de valores outliers que superan el tercer cuartil.

- Respecto a la variable base "SalePrice" 

- **Variables con correlación ALTA:** 
- - OverallQual (Calidad de la construcción) - 79%
- - GrLiveArea (Area habitable) - 71%
- - GarageArea (Area de cochera) - 62%
- - 1stFlSF (Pies cuadrados habitables en primer piso) - 61%

- **Variables con correlación MEDIA o BAJA:**
- - TotRmsAbvGrd (Cantidad de habitaciones) - 53%
- - 2ndFlrSF (Pies cuadrados habitables en segundo piso) - 32%
- - LotArea (Area de terreno) - 26%
- - BedroomAbvGr (Cantidad de baños) - 17%

**Variables con correlación MUY BAJA o NEGATIVA:**
- - PoolArea (Area de piscina)
- - MSSubClass (Clase de construcción)
- - OverallCond (Calificación de condición general)
- - KitchenAbvGr (Cantidad de cocinas)

- Se aprecia que los top 3 barrios con precios mas elevados son NoRidge, NridgHt y StoneBr. **La media de los barrios anterior nombrados supera en un 77% la media global del Dataset**

- En general la discreción respecto a la variable base SalePrice con las 4 variables mas correlacionadas demuestran estar fuertemente alineadas. Siendo el GarageArea la variable con mayor discreción respecto al precio de venta.

<a name="h_test"></a>
## Hipótesis
H0 es igual a 120 dólares el Ft2 y el H1 es mayor igual a 132 dólares Ft2
El P-Value es menor que 0.05 por lo cual rechazo el H0

<a name="pca"></a>
## PCA
Aparentemente todos los barrios comparten una cierta correlación entre sus dos Componentes principales.

<a name="link"></a>
## Links
[Fuente del DataSet](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

