# Proyecto ETL – Sentinel Pi

Este proyecto realiza el **proceso ETL** (Extracción, Transformación y Carga) sobre datos de intentos de ataque recopilados por Sentinel Pi.

## Objetivo
Procesar y limpiar los datos crudos para dejarlos listos para análisis supervisado y no supervisado, así como para alimentar otros procesos como seeder o dashboards.

## Proceso

1. **Extracción**  
   - Carga de datos desde un archivo JSON con información de ataques (IP, puerto, protocolo, sistema operativo, comportamiento, geolocalización, timestamp, etc.).

2. **Transformación**  
   - Normalización de datos anidados (`geolocation`, `timestamp`).  
   - Limpieza de columnas irrelevantes (`_id`, `_class`, `payload`, `tools`).  
   - Manejo de valores nulos y formatos de fecha.  
   - Renombrado de columnas para mayor claridad (`timestamp`, `country`, `city`).

3. **Carga**  
   - Generación de un dataset limpio (`ataques_limpios.json`) listo para análisis.  

## Ventajas del enfoque
- Facilita la **calidad y consistencia de los datos** antes de aplicar modelos de Machine Learning.  
- Permite **reutilización** de los datos limpios en otros notebooks o procesos ETL posteriores.  
- Simplifica el desarrollo de **modelos supervisados y no supervisados**, evitando errores por datos sucios o mal formateados.
