
# Análisis No Supervisado – Sentinel Pi

Este notebook explora patrones y agrupamientos en los ataques sin usar etiquetas previas, detectando tendencias y anomalías.

## Objetivo
Identificar grupos de comportamiento similar y posibles anomalías entre los ataques.

## Proceso Breve
1. Selección de variables numéricas (`port`, `protocol`, `os`, `country`).
2. Escalado y reducción de dimensionalidad (PCA).
3. Clustering con K-Means y DBSCAN.

## Resultados
- K-Means agrupa los ataques en 3 clusters principales.
- DBSCAN detecta anomalías y ruido en los datos.
- Las visualizaciones muestran los patrones encontrados.

## Herramientas
Se utilizan pandas, scikit-learn, matplotlib y seaborn.

