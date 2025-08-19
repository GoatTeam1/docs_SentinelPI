
# Análisis Supervisado – Sentinel Pi

Este notebook realiza análisis supervisado sobre intentos de ataque, clasificándolos según su tipo (`behavior`) usando características de los ataques.

## Objetivo
Predecir patrones y riesgos de ataques para priorizar alertas y acciones automáticas.

## Proceso Breve
1. Limpieza y transformación de datos.
2. Visualización de variables clave.
3. Modelado supervisado aplicando tres algoritmos:
	- Árbol de Decisión
	- Random Forest
	- Regresión Logística

## Resultados
- Los modelos logran buena precisión en la clasificación de ataques.
- Se identifican las variables más relevantes para la predicción.
- Las gráficas muestran la distribución de los ataques por protocolo, sistema operativo y país.

## Herramientas
Se utilizan pandas, scikit-learn, matplotlib y seaborn.
