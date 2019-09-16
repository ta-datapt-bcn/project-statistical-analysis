
---
<div style="width: 200px;">![https://camo.githubusercontent.com/7b53865828a6796cb5f25926548e18dbf5e14de2/68747470733a2f2f6269742e6c792f32566e58577232](attachment:foo.svg)</div>
<img src="attachment:https://camo.githubusercontent.com/7b53865828a6796cb5f25926548e18dbf5e14de2/68747470733a2f2f6269742e6c792f32566e58577232" width="200">
---

# Análisis de House Prices
### Jorge Alvarez
## Contenido

- Descripción del proyecto
- Hypotesis / Preguntas
- Exploración y análisis del  DataSet
- Limpieza
- Test de Hipótesis
- PCA
- Probabilidad
- Links

## Descripción del proyecto

El proyecto se basa en datos de venta de casas en USA. Se pretenden buscar insigths que permitan entender mejor el mercado de compra/venta de casas.

## Hipotesis / Preguntas
- Que correlación tiene el precio de venta con las diferentes variables
- Cuál es el precio medio y los cuartiles por barrio
- Cuál es el precio medio por cantidad de habitaciones
- Como es la correlación y la línea regresión entre el SalePrice y el LotSize
- ¿El precio medio por FT2 de “NoRidge” es mayor a la del resto de barrios?
- Que probabilidad existe de que una casa tenga más de 2 habitaciones siendo que esta se encuentra en cada uno de los barrios.

## Exploración y análisis del  DataSet
- El SalePrice tiene correlación con LotArea, GrLiveArea, TotRmsAbvGrd, GarageArea, 1stFlrSF y 2ndFlrSF
- La distribución de precios posee una leve tendencia a tener precios más altos.
- La media de precio de cada barrio tiene demuestran una amplia variación entre sí.
- La correlación entre el precio y el tamaño del lote es positiva, al igual que el area

## Limpieza
Se eliminaron las columnas con muchos datos faltantes.

## Test de Hipótesis
H0 es igual a 120 dólares el Ft2 y el H1 es mayor igual a 132 dólares Ft2
El P-Value es menor que 0.05 por lo cual rechazo el H0

## PCA
Aparentemente todos los barrios comparten una cierta correlación entre sus dos Componentes principales.

## Links
[link text](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

