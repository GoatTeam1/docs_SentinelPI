# Seeder SentinelPi

Este directorio contiene la documentación, respaldos y evidencias del proceso de generación de datos simulados para la base de datos de SentinelPi.

---

## Archivos incluidos

- `db_backup_onlystructure.json`: Respaldo con la estructura de las colecciones en MongoDB (sin datos).
- `db_backup_withdata.json`: Datos de ejemplo (muestra reducida generada con Faker).
- `endpoints_screenshot.png`: Captura de los endpoints de seeder disponibles en Swagger.
- `db_empty_screenshot.png`: Captura de la base de datos vacía antes del llenado.
- `README.md`: Este archivo de documentación.

---

## Código fuente del seeder

El seeder fue implementado dentro del mismo repositorio del backend utilizando **Spring Boot** y la librería **Faker**.  
El servicio principal se encuentra en:  
[SeederService.java](https://github.com/GoatTeam1/backend-sentinelpi/blob/main/src/main/java/com/sentinelpi/sentinelpi/seeders/SeederService.java)

---

## Respaldo de la base de datos

### Estructura (sin datos)
- Archivo: `db_backup_onlystructure.json`
- Evidencia: ![alt text](/img/image.png)

### Con datos generados
- Archivo: `data_backup_large.json`
  - Cabe mencionar que la estructura solo tiene 1 valor por cada colección

---

## Endpoints disponibles para seeder

> Nota: Estos endpoints están documentados en Swagger. Aquí se listan para referencia rápida.

### Attacks
- **POST** `/api/seed/{nombre_coleccion}/{cantidad}`
  - Genera `{cantidad}` registros de ataques simulados.
![alt text](/img/image-03.png)

Con un solo endpoint podemos utilizar el seeder al pasar como parametros el nombre de la colección y la cantidad de datos

### Ejemplo de uso
```bash
curl -X POST "http://localhost:8080/api/seed/attacks/1000000"
```

![alt text](/img/image-1.png)

Y en el gestor de Mongo se ve asi:

![alt text](/img/image-2.png)