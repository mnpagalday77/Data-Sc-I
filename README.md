# Análisis Económico y Modelado Predictivo en América del Sur (1960–2024)

Este repositorio contiene un análisis de indicadores económicos históricos de países sudamericanos y un modelo predictivo centrado en la inflación, basado en datos reales del Banco Mundial.

## Archivos incluidos

- `ProyectoParteIII_Pagalday.ipynb`: notebook con el desarrollo completo.
- `IndEconom_Data.xlsx`: base de datos con los indicadores económicos.
- `Metadata.xlsx`: diccionario de variables del dataset.

## Descripción del proyecto

Se analizó el desarrollo económico de seis países de América del Sur: Argentina, Brasil, Uruguay, Colombia, Venezuela y Paraguay, entre 1960 y 2024. El proyecto incluye:

- Limpieza de datos y tratamiento de valores faltantes
- Identificación y tratamiento de outliers
- Análisis de correlaciones entre variables
- Visualización de series temporales por país e indicador
- Comparación de indicadores macroeconómicos clave entre países
- Exploración de las siguientes variables:
  - PIB
  - Inflación
  - Desempleo
  - Tasa de interés
  - Importaciones y exportaciones (% del PIB)
  - Apertura comercial

## Modelado predictivo

Se utilizó `SelectKBest` con `f_regression` para identificar la variable más relevante para predecir la inflación: **Importaciones de bienes y servicios (% del PIB)**.

Con esta variable se entrenaron y compararon tres modelos de regresión:

- Regresión Lineal
- Árbol de Decisión
- Random Forest

Se evaluaron con las métricas:
- MAE (Error Absoluto Medio)
- MSE (Error Cuadrático Medio)
- RMSE

El modelo lineal fue el que mostró el mejor rendimiento general.

## Conclusión

Se completó de forma coherente todo el flujo de trabajo: análisis exploratorio, visualización, limpieza, selección de variables, modelado y validación. A pesar del tamaño reducido del conjunto de prueba, el proceso permitió extraer conclusiones útiles sobre la dinámica económica de la región.

Trabajo realizado por **Mathias Pagalday**
