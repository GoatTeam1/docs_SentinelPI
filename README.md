
---
# Sentinel Pi
### Sentinel PI
<p align="justify"> El aumento de los ciberataques a nivel mundial ha generado la necesidad urgente de contar con mecanismos de detección temprana que permitan mitigar riesgos y reforzar la seguridad en redes y sistemas críticos. En este contexto surge Sentinel Pi, un proyecto innovador diseñado como un honeypot inteligente basado en Raspberry Pi, cuyo propósito principal es actuar como una herramienta de bajo costo, accesible y adaptable para la detección temprana de amenazas informáticas. Este sistema busca no solo identificar y registrar intentos de intrusión, sino también ofrecer un entorno de análisis que permita comprender mejor los patrones de ataque y, a partir de ello, fortalecer la ciberdefensa de instituciones y organizaciones que requieran un monitoreo constante.

<p align="justify"> La arquitectura de Sentinel Pi está pensada de manera modular y escalable. En su núcleo, la Raspberry Pi funciona como un honeypot capaz de simular servicios comunes como SSH, FTP o Telnet, con el objetivo de atraer a potenciales atacantes y recopilar información sobre los intentos de acceso no autorizados. Todos los registros generados son procesados mediante una API centralizada desarrollada en Spring Boot, que asegura un flujo estructurado de datos hacia una base de datos confiable. Este enfoque permite manejar información sensible de manera segura y ordenada, garantizando la integridad de los registros y la consistencia de los eventos capturados.

<p align="justify"> Una de las características diferenciadoras de Sentinel Pi es su enfoque en la visualización distribuida de datos. Además de la interfaz web, el sistema incluye una aplicación desarrollada en Kotlin para Smart TV, lo que permite a los equipos de seguridad consultar de forma inmediata las métricas más relevantes en entornos de trabajo colaborativo o salas de monitoreo. De esta manera, los datos obtenidos del honeypot no permanecen ocultos en registros técnicos, sino que son expuestos como herramientas estratégicas para la toma de decisiones.

<p align="justify"> El proyecto también contempla requisitos no funcionales clave como la escalabilidad mediante contenedores en Docker Compose, la comunicación segura usando HTTPS y JWT, la portabilidad hacia diferentes dispositivos y navegadores, y la tolerancia a fallos frente a desconexiones o interrupciones temporales. Estos atributos garantizan que Sentinel Pi no sea una solución rígida, sino un sistema adaptable a diversos contextos institucionales, desde universidades hasta pequeñas empresas o dependencias gubernamentales que buscan robustecer su postura de seguridad sin invertir en costosas infraestructuras.

<p align="justify"> Sentinel Pi se apoya en prácticas ágiles y herramientas de modelado como UML, DFD y Redes de Petri, que han permitido definir de manera clara los casos de uso, los componentes principales y la interacción entre módulos. Asimismo, la documentación asociada al proyecto sigue los lineamientos del estándar IEEE 830, asegurando que los requisitos, restricciones y escenarios futuros estén formalmente especificados y disponibles para la comunidad.
 </p>

## LOGOTIPOS

<table>
   <td>Logo de la Aplicacion</td>
   <td>Logo de empresa</td>
  <tr>
    <td>  <img src="img/img2.jpeg" width="80%" style="padding: 10px;" />  </td>
    <td>   <img src="img/img1.jpeg" width="80%" style="padding: 10px;" /> </td>
   
  </tr>
 
</table>

### DESCRIPCION
<p align="justify">
Sentinel Pi es un sistema de ciberseguridad basado en Raspberry Pi que funciona como un honeypot inteligente, diseñado para la detección temprana de amenazas y el análisis de intentos de intrusión. Su objetivo es proporcionar una solución accesible, escalable y adaptable que permita a instituciones, empresas y organizaciones contar con una primera línea de defensa contra ciberataques.

El proyecto combina diferentes tecnologías en un ecosistema integral:

En la capa de detección, Raspberry Pi emula servicios comunes como SSH, FTP o HTTP, atrayendo posibles atacantes en un entorno controlado y seguro.

En la capa de procesamiento, los eventos capturados son enviados a una API central desarrollada en Java con Spring Boot, donde se procesan, validan y almacenan en una base de datos como MongoDB o MySQL.

<p align="justify"> En la capa de análisis y visualización, se utilizan herramientas como Python para análisis de datos y un frontend en React con TailwindCSS que permite monitorear en tiempo real los ataques registrados, así como explorar estadísticas históricas mediante gráficos interactivos.

<p align="justify"> Se desarrolló una aplicación para Smart TV en Kotlin, que facilita la consulta de datos de seguridad en pantallas inteligentes, pensando en centros de monitoreo y salas de control.

<p align="justify"> El proyecto también integra un componente de monitoreo y visualización avanzada con Grafana, permitiendo que los administradores puedan correlacionar los intentos de intrusión con métricas de red y comportamiento en tiempo real. La arquitectura está soportada en contenedores Docker, lo que facilita la escalabilidad, la portabilidad y la implementación modular en distintos entornos.

<p align="justify"> Sentinel Pi no solo busca detectar ataques, sino también convertirse en una herramienta educativa y de investigación, brindando información sobre patrones de ataque, vectores de intrusión más utilizados y métodos de evasión empleados por ciberdelincuentes. Con esta propuesta, se fomenta una cultura de ciberseguridad más sólida, accesible y aplicada a escenarios reales, aportando valor tanto a pequeñas organizaciones como a instituciones de gran escala.
</p>

---

### PLANTEAMIENTO DEL PROBLEMA

<p align="justify">
Sentinel Pi es un sistema honeypotimplementado sobre Raspberry Pi, diseñado para detectar y registrar intentos de intrusión, analizar amenazas con Python, y visualizarlas mediante un panel web en React y una app para Smart TV con Kotlin. Este proyecto combina bajo costo, portabilidad y escalabilidad para ofrecer una solución accesible en entornos de ciberseguridad.

<p align="justify"> La arquitectura del sistema se centra en la Raspberry Pi como dispositivo principal, simulando servicios vulnerables para atraer atacantes y recopilar datos de sus actividades. Estos registros son enviados a una API desarrollada en Spring Boot, que centraliza la información, la almacena en bases de datos seguras y permite el análisis posterior. El uso de contenedores Docker y un diseño modular asegura que el sistema pueda adaptarse fácilmente a distintas instituciones sin comprometer su funcionamiento.

<p align="justify"> El panel web en React proporciona visualización en tiempo real de intentos de acceso, estadísticas históricas y patrones de ataque, utilizando librerías de gráficos como Recharts. Por su parte, la aplicación en Smart TV, desarrollada en Kotlin, está orientada a salas de monitoreo, facilitando la supervisión colaborativa.

<p align="justify"> En conjunto, Sentinel Pi democratiza la ciberseguridad, brindando a universidades, empresas y gobiernos una herramienta práctica, flexible y confiable para fortalecer su defensa digital.

</p>

---

### PROPUESTA DE SOLUCION
<p align="justify">
En respuesta al creciente número de ciberataques que amenazan diariamente la integridad de empresas, instituciones y servicios públicos, se plantea el desarrollo de Sentinel Pi, una solución práctica, accesible y orientada a la detección temprana de posibles intrusiones mediante el uso de dispositivos Raspberry Pi configurados como honeypots personalizados. Este enfoque busca ofrecer una herramienta tangible para monitorear y analizar el comportamiento de posibles atacantes antes de que logren comprometer activos críticos, reforzando así la seguridad en infraestructuras tecnológicas con bajo costo de implementación.

<p align="justify"> El proyecto contempla la creación de una plataforma web en React y una aplicación para dispositivos inteligentes, incluyendo Smart TV con Kotlin, que permitirán la visualización en tiempo real de los intentos de intrusión captados por el honeypot. Estos entornos ofrecerán reportes interactivos y estadísticas generadas con Python y librerías de análisis de datos, facilitando la comprensión de patrones de ataque, su frecuencia y los vectores más comunes utilizados por los atacantes.

<p align="justify"> La configuración del honeypot será adaptable a las necesidades particulares de cada organización, con el objetivo de atraer atacantes en un entorno controlado y seguro que no ponga en riesgo la infraestructura operativa. Toda la información recolectada será enviada a una API centralizada en Spring Boot, que se encargará de procesar, almacenar y clasificar los registros en una base de datos MongoDB para garantizar escalabilidad y eficiencia.

<p align="justify"> Sentinel Pi considera aspectos de seguridad avanzados, como la comunicación cifrada mediante HTTPS y autenticación con JWT, además de una arquitectura modular desplegada con Docker Compose para facilitar la portabilidad y el escalamiento en distintos entornos institucionales.

<p align="justify"> En conjunto, esta propuesta representa una solución integral que combina detección temprana, análisis forense y visualización intuitiva, otorgando a las instituciones una gran herramienta para reforzar sus defensas cibernéticas y anticiparse a posibles amenazas.

</p>

---

### OBJETIVO GENERAL

<p align="justify">Diseñar e implementar un sistema de seguridad pasiva basado en Raspberry Pi, que funcione como un honeypot para detectar y registrar intentos de intrusión en redes informáticas, proporcionando a las empresas e instituciones una interfaz web accesible para visualizar y analizar los intentos de ataque en tiempo real, con el fin de fortalecer sus medidas de ciberseguridad de manera proactiva.
</p>


---

### OBJETIVOS ESPECIFICOS

<p align="justify">Configurar el Raspberry Pi como un honeypot capaz de detectar y registrar intentos de intrusión.</p>

<p align="justify">Mapa interactivo: Desarrollar una plataforma web que permita visualizar en tiempo real los intentos de acceso captados por el sistema.</p>

<p align="justify">Implementación de alertas: Implementar un sistema centralizado que recopile, almacene y analice los datos generados por el dispositivo.</p>

<p align="justify">Implementación de reportes eficiente: Facilitar a las instituciones el monitoreo y la comprensión de los ataques mediante gráficos, reportes y estadísticas.</p>

<p align="justify">Desarrollar una aplicación para dispositivos inteligentes que permita la consulta de los datos de seguridad capturados por el honeypot desde diferentes entornos.</p>

<p align="justify">Validar el sistema mediante pruebas en un entorno controlado simulando escenarios reales de ataque.</p>

<p align="justify">Asegurar que el sistema pueda escalar o adaptarse a distintas instituciones con necesidades específicas.</p>

---

### TABLA DE COLABORADORES

| Nombre                          | Usuario                                               | Puesto                                 |
| ------------------------------- | ----------------------------------------------------- | -------------------------------------- |
| Leslie Janet Aparicio Castro    | [leslie-aparicio](https://github.com/leslie-aparicio) | Documentadora                          |
| Carlos Armando Aranda Hernández | [Carlicsus](https://github.com/Carlicsus)             | Desarrollador Backend                  |
| José Alejandro Briones Arroyo   | [alexba2004](https://github.com/alexba2004)           | Desarrollador del Honeypot y DecSecOps |
| Diego Hernández Mota            | [MotaBytes](https://github.com/MotaBytes)             | Desarrollador Frontend                 |
| Jazziel Rodríguez López         | [JazzoLopez](https://github.com/JazzoLopez)           | Desarrollador Backend                  |

---

### ORGANIGRAMA DEL EQUIPO
  <img src="img/Organigrama Sentinel Pi (2).png" width="80%" style="padding: 10px;" />


---

### DIAGRAMA DE GANTT

  <img src="img/gantt_sentinel.drawio.png" width="80%" style="padding: 10px;" />

---

### LISTA DE TECNOLOGIAS

## 🚀 Tecnologías utilizadas en Sentinel Pi

### Backend
![Spring Boot](https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

### Smart TV App
![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)

### Base de Datos
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

### DevOps & Monitoreo
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)


### Modelado & Diagramas
![draw.io](https://img.shields.io/badge/draw.io-F08705?style=for-the-badge&logo=diagrams.net&logoColor=white)

### Control de versiones
![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

### 🫐 Tecnologías utilizadas en el Honeypot

### Hardware & SO (Raspberry Pi)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=for-the-badge&logo=raspberrypi&logoColor=white)
![ARM (ARMv7/ARM64)](https://img.shields.io/badge/ARM-ARMv7%2FARM64-0091BD?style=for-the-badge&logo=arm&logoColor=white)
![Raspberry Pi OS](https://img.shields.io/badge/Raspberry%20Pi%20OS-(Debian%2012%2B)-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Ubuntu Server ARM](https://img.shields.io/badge/Ubuntu%20Server-ARM64-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

> Modelos recomendados: Pi 2B o superior (2 GB RAM mínimo). SO recomendado: Raspberry Pi OS 64‑bit o Ubuntu Server ARM64.

---

### Contenedores & Orquestación
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![network_mode: host](https://img.shields.io/badge/Docker-network__mode%3A%20host-555?style=for-the-badge)

- Despliegue reproducible multi‑arquitectura (arm64/armv7/amd64).
- `network_mode: host` para exponer puertos “bien conocidos” sin NAT.

---

### Honeypots y Emulación
![OpenCanary](https://img.shields.io/badge/OpenCanary-Emulaci%C3%B3n%20de%20servicios-222?style=for-the-badge)
![Cowrie](https://img.shields.io/badge/Cowrie-SSH%2FTelnet%20alta%20interacci%C3%B3n-555?style=for-the-badge)
![T--Pot](https://img.shields.io/badge/T--Pot-Suite%20de%20honeypots-777?style=for-the-badge)

- **OpenCanary** (principal): HTTP, Telnet, MySQL, FTP, SMB, RDP, TFTP, NTP, SSH (opcional).
- **Cowrie**: captura de sesiones SSH/Telnet de alta interacción.
- **T‑Pot**: suite integrada de honeypots.

---

### Lenguajes & Runtime
![Python 3.13.7](https://img.shields.io/badge/Python-3.13.7-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-121011?style=for-the-badge&logo=gnubash&logoColor=white)

- *Entrypoint* en **Python** para generar `opencanary.conf` desde plantilla/variables de entorno.
- Script de endurecimiento de egreso en **Bash** (`hardening/outbound-lockdown.sh`).

---

### Red & Seguridad (host)
![iptables](https://img.shields.io/badge/iptables-nftables-6E9F18?style=for-the-badge&logo=linux&logoColor=white)
![Syslog](https://img.shields.io/badge/Syslog-UDP%2FTCP%20514-4B7F52?style=for-the-badge)
![VLAN/DMZ](https://img.shields.io/badge/Red-VLAN%2FDMZ-0F766E?style=for-the-badge)

- Aislamiento en VLAN/DMZ, límites de egreso mediante **iptables/nftables**.
- Verificación de colisiones de puertos con `ss`, `netstat` o `lsof`.

---

### Logging & Alertas
![JSON Lines](https://img.shields.io/badge/Logs-JSONL-000?style=for-the-badge)
![SMTP](https://img.shields.io/badge/Alertas-SMTP-6A5ACD?style=for-the-badge)
![Webhook](https://img.shields.io/badge/Alertas-Webhook-2E7D32?style=for-the-badge)
![Syslog](https://img.shields.io/badge/Alertas-Syslog-4B7F52?style=for-the-badge)

- **Archivo**: `./data/opencanary.log` (JSON por línea).
- **SMTP**: envío de correo (App Password recomendado con Gmail).
- **Webhook**: HTTP/HTTPS POST hacia un ingestor.
- **Syslog**: envío a colector UDP/TCP 514.

---

### Utilidades de verificación
![nmap](https://img.shields.io/badge/nmap-2C3E50?style=for-the-badge)
![curl](https://img.shields.io/badge/curl-073551?style=for-the-badge)
![telnet](https://img.shields.io/badge/telnet-555?style=for-the-badge)
![mysql client](https://img.shields.io/badge/mysql%20client-005C84?style=for-the-badge&logo=mysql&logoColor=white)

- **nmap** para escaneo de puertos/servicios.
- **curl/telnet/mysql** para generar eventos de prueba.

---

## Sentinel PI - Documentación Técnica

Sistema de gestión y monitoreo desarrollado con arquitectura basada en microservicios, autenticación JWT y despliegue en contenedores.

### 1. Herramientas y Versiones

El proyecto está construido utilizando las siguientes tecnologías:

- **Java**: 17
- **Spring Boot**: 3.5.0
- **Maven**: 3.9.x
- **Angular**: 17
- **Node.js**: 20.x (para frontend Angular)
- **Yarn**: 1.22.x
- **MongoDB**: 6.0
- **Docker**: 24.x
- **Dockerfile**: definido en el proyecto para construcción de imágenes
- **Docker Compose**: 2.x (para orquestación de servicios)
- **JWT (JSON Web Token)**: JJWT 0.11.5
- **Spring Security**: última versión compatible con Spring Boot 3.5.0
- **Lombok**: 1.18.x
- **Postman**: 10.x (colecciones de pruebas de API)
- **Git**: 2.40+

### 2. Variables de Configuración

El proyecto utiliza variables de entorno para separar credenciales y configuraciones sensibles.
Estas variables deben definirse en un archivo `.env` (no versionado en Git) o como configuración en el servidor.

#### Backend (Spring Boot)

```properties
SERVER_PORT=8080
MONGO_URI=mongodb://<usuario>:<password>@<host>:<puerto>/<database>
MONGO_DATABASE=sentinel_db
JWT_SECRET=<clave-secreta-no-compartir>
JWT_EXPIRATION=3600000
LOG_LEVEL=INFO
```

#### Frontend (Angular)

```typescript
// environment.ts
export const environment = {
  production: false,
  apiUrl: "http://localhost:8080/api"
};
```

#### Docker

```properties
DOCKER_IMAGE_NAME=sentinel-pi
DOCKER_IMAGE_TAG=latest
MONGO_INITDB_ROOT_USERNAME=admin
MONGO_INITDB_ROOT_PASSWORD=<password>
MONGO_INITDB_DATABASE=sentinel_db
```

### 3. Ejemplos de Buenas Prácticas con Variables

**No subir credenciales reales a GitHub.**

Ejemplo correcto:
```
MONGO_URI=mongodb://<usuario>:<password>@localhost:27017/sentinel_db
```

Ejemplo incorrecto:
```
MONGO_URI=mongodb://admin:12345@localhost:27017/sentinel_db
```

**Mantener múltiples archivos de configuración:**
- `application-dev.properties` para entorno local.
- `application-prod.properties` para entorno de producción.

**Uso de `.gitignore`**: asegurarse de que `.env` y configuraciones locales no se versionen.

### 4. Estructura del Proyecto

```
sentinel-pi/
├── backend/
│   ├── src/main/java/... (código fuente Spring Boot)
│   ├── pom.xml
│   └── Dockerfile
│
├── frontend/
│   ├── src/app/... (código fuente Angular)
│   ├── package.json
│   └── Dockerfile
│
├── docker-compose.yml
├── .env (variables de entorno, no versionar)
└── README.md
```

### 5. Ejecución Local

#### Backend

```bash
cd backend
mvn clean install
mvn spring-boot:run
```

#### Frontend

```bash
cd frontend
yarn install
yarn start
```

#### Con Docker

```bash
docker-compose up --build
```

### 6. Pruebas con Postman

Se incluye una colección de Postman con las principales rutas de la API.

1. Importar el archivo `SentinelPI.postman_collection.json`.

2. Configurar la variable de entorno `{{baseUrl}}` en Postman:
   - Local: `http://localhost:8080/api`
   - Producción: `https://<dominio>/api`

### 7. Despliegue

**Construir las imágenes Docker:**
```bash
docker build -t sentinel-pi-backend ./backend
docker build -t sentinel-pi-frontend ./frontend
```

**Levantar con Docker Compose:**
```bash
docker-compose up -d
```

**Validar servicios en ejecución:**
- Backend: `http://localhost:8080/api`
- Frontend: `http://localhost:4200`

---

## Plan de Prueba – Proyecto Sentinel PI

### Objetivo:
Validar que Sentinel PI funcione correctamente en todos sus módulos: backend, frontend y APIs, asegurando integridad de datos, flujo de usuario correcto y respuesta ante errores.

### Alcance:

- **Backend**: endpoints, lógica de negocio, seguridad y base de datos.
- **Frontend**: interfaz, navegación, formularios y visualización de datos.
- **Integración**: comunicación frontend-backend, autenticación, manejo de errores.

### Criterios de Entrada:

- Código backend y frontend completo y desplegable en entorno de prueba.
- Base de datos inicializada con datos de prueba.
- Acceso a herramientas de testing (Postman, navegador, consola).

### Criterios de Salida:

- Todas las funcionalidades críticas probadas y sin fallas bloqueantes.
- Registro de incidencias y bugs para corrección.

### Recursos:

- **Tester**: 1-2 personas.
- **Software**: Postman, navegador web, consola backend, base de datos (MongoDB/MySQL).

### Riesgos:

- Cambios frecuentes en APIs o base de datos.
- Dependencias externas (servicios de terceros) que fallen.

---

## Casos de Prueba – Sentinel PI

| ID    | Área        | Funcionalidad                 | Caso de Prueba                                         | Datos de Prueba                | Resultado Esperado                                                       |
| ----- | ----------- | ----------------------------- | ------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------------------ |
| CP-01 | Backend     | CRUD Usuarios                 | Crear, leer, actualizar y eliminar usuarios vía API    | JSON de usuario válido         | Operaciones exitosas, respuestas 200/201/204 según caso                  |
| CP-02 | Backend     | Seguridad JWT                 | Probar login y acceso a endpoints protegidos           | Usuario válido/Inválido        | JWT emitido correctamente, acceso denegado sin token                     |
| CP-03 | Backend     | Manejo de errores             | Enviar request con datos inválidos                     | JSON incompleto o mal formado  | Respuesta 400 con mensaje de error                                       |
| CP-04 | Frontend    | Login                         | Ingresar credenciales válidas e inválidas              | Usuario válido/Inválido        | Redirección al dashboard o mensaje de error                              |
| CP-05 | Frontend    | Visualización de datos        | Abrir dashboard y listar servicios/usuarios            | Datos en DB de prueba          | Todos los datos se muestran correctamente y en orden                     |
| CP-06 | Frontend    | Formulario de servicio        | Crear un nuevo servicio desde UI                       | Formulario completo            | Servicio agregado y listado correctamente                                |
| CP-07 | Integración | Comunicación frontend-backend | Realizar CRUD completo desde UI                        | Usuario y servicio de prueba   | Acciones UI reflejan cambios reales en backend                           |
| CP-08 | Integración | Flujo completo                | Crear usuario → login → crear servicio → cerrar sesión | Datos de prueba                | Flujo funcional sin errores, todos los endpoints funcionan correctamente |
| CP-09 | Rendimiento | API                           | Hacer 100 requests simultáneos                         | JSON de prueba                 | Respuesta bajo 2 segundos promedio, sin errores                          |
| CP-10 | Seguridad   | SQL/NoSQL Injection           | Intentar inyectar código en endpoints                  | Payload malicioso              | Backend maneja la inyección y devuelve error seguro                      |
| CP-11 | Frontend    | UI responsiva                 | Abrir aplicación en escritorio, tablet y móvil         | Navegadores y tamaños variados | UI se adapta y mantiene funcionalidad                                    |

---

## Plan de Integración de Código y Versionamiento

### Estructura de Ramas

#### Ramas principales
- **main**: Contiene el código en producción. Todo aquí debe estar probado y estable.
- **develop**: Contiene el código en estado de integración, listo para pruebas antes de producción.

#### Ramas auxiliares

| Tipo de rama | Origen  | Fusión hacia   | Uso principal                                 |
| ------------ | ------- | -------------- | --------------------------------------------- |
| feature/*    | develop | develop        | Para nuevas funcionalidades.                  |
| bugfix/*     | develop | develop        | Corrección de errores encontrados en pruebas. |
| release/*    | develop | main + develop | Preparar una nueva versión para producción.   |
| hotfix/*     | main    | main + develop | Corrección urgente de errores en producción.  |

### Flujo de trabajo

#### Nueva funcionalidad

```bash
git checkout develop
git checkout -b feature/nombre-funcionalidad

# trabajar y commitear
git checkout develop
git merge feature/nombre-funcionalidad
git branch -d feature/nombre-funcionalidad
```

#### Nueva versión

```bash
git checkout develop
git checkout -b release/1.0.0

# ajustes finales
git checkout main
git merge release/1.0.0
git tag -a v1.0.0 -m "Release 1.0.0"
git checkout develop
git merge release/1.0.0
git branch -d release/1.0.0
```

#### Corrección urgente en producción

```bash
git checkout main
git checkout -b hotfix/fix-nombre-error

# aplicar fix
git checkout main
git merge hotfix/fix-nombre-error
git tag -a v1.0.1 -m "Hotfix 1.0.1"
git checkout develop
git merge hotfix/fix-nombre-error
git branch -d hotfix/fix-nombre-error
```

### Buenas prácticas de commits

- **Commits claros y concisos**. Evitar "arreglo", "cambio", etc.
- **Usar prefijos** para identificar el tipo de cambio:
  - `feat:` para nuevas funcionalidades
  - `fix:` para correcciones de bugs
  - `docs:` para cambios en documentación
  - `refactor:` para cambios de código que no afectan la funcionalidad
  - `test:` para agregar o modificar pruebas
  - `chore:` para tareas menores (build, configs, etc.)

#### Ejemplos de buenos mensajes de commit

```bash
feat: agrega autenticación con JWT
fix: corrige error al validar email duplicado
docs: actualiza sección de instalación
refactor: separa lógica de validación en servicio aparte
```

### Notas finales

- Siempre trabajar en ramas, nunca directo en `main` o `develop`.
- Hacer `pull` antes de empezar a trabajar.
- Borrar ramas locales cuando ya no se usen.
- Usar tags para marcar versiones en producción.

---

## Plan de Despliegue – Sentinel PI

### Objetivo
Establecer un proceso automatizado y confiable para el despliegue de Sentinel PI en diferentes entornos, garantizando la consistencia, trazabilidad y rollback en caso de fallos.

### Entornos de Despliegue

#### 1. Desarrollo (Development)
- **Propósito**: Pruebas locales y desarrollo activo
- **Rama**: `feature/*`, `develop`
- **Infraestructura**: Docker Compose local
- **Base de datos**: MongoDB local o contenedor
- **Despliegue**: Manual, automático en cambios de develop

#### 2. Pruebas (Testing/Staging)
- **Propósito**: Validación de funcionalidades y pruebas de integración
- **Rama**: `release/*`
- **Infraestructura**: Servidor de pruebas o contenedores en cloud
- **Base de datos**: MongoDB dedicada para testing
- **Despliegue**: Automático al crear rama release

#### 3. Producción (Production)
- **Propósito**: Sistema en vivo para usuarios finales
- **Rama**: `main`
- **Infraestructura**: Cloud (Azure/AWS) o servidores dedicados
- **Base de datos**: MongoDB en cluster con respaldo
- **Despliegue**: Automático al hacer merge a main con aprobación manual

### Estrategia de Despliegue

#### Pipeline de CI/CD

```yaml
# Ejemplo de flujo con GitHub Actions
Desarrollo → Testing → Producción
     ↓           ↓           ↓
   Docker    Automated   Blue-Green
   Compose    Testing    Deployment
```

#### Fases del despliegue

| Fase              | Acción                                    | Responsable            | Duración estimada |
| ----------------- | ----------------------------------------- | ---------------------- | ----------------- |
| 1. Build          | Compilación y creación de imágenes Docker | CI/CD Pipeline         | 5-10 min          |
| 2. Test           | Ejecución de pruebas automatizadas        | CI/CD Pipeline         | 3-5 min           |
| 3. Deploy Testing | Despliegue en entorno de pruebas          | CI/CD Pipeline         | 2-3 min           |
| 4. Validation     | Validación manual de funcionalidades      | QA Team                | 15-30 min         |
| 5. Deploy Prod    | Despliegue en producción                  | DevOps/Release Manager | 5-10 min          |
| 6. Health Check   | Verificación de servicios en producción   | CI/CD Pipeline         | 2-3 min           |

### Configuración por Entorno

#### Variables de entorno requeridas

```bash
# Desarrollo
SERVER_PORT=8080
MONGO_URI=mongodb://localhost:27017/sentinel_dev
JWT_SECRET=dev-secret-key
LOG_LEVEL=DEBUG

# Pruebas
SERVER_PORT=8080
MONGO_URI=mongodb://test-server:27017/sentinel_test
JWT_SECRET=test-secret-key
LOG_LEVEL=INFO

# Producción
SERVER_PORT=8080
MONGO_URI=mongodb://prod-cluster:27017/sentinel_prod
JWT_SECRET=${PROD_JWT_SECRET}
LOG_LEVEL=WARN
```

### Proceso de Rollback

#### Estrategia Blue-Green
1. **Preparación**: Mantener versión anterior (Green) mientras se despliega nueva (Blue)
2. **Switchover**: Cambiar tráfico de Green a Blue una vez validado
3. **Rollback**: En caso de fallo, regresar tráfico a Green inmediatamente

#### Comandos de rollback

```bash
# Rollback automático con Docker
docker-compose down
docker-compose up -d --scale backend=2
docker tag sentinel-pi-backend:previous sentinel-pi-backend:latest
docker-compose restart backend

# Rollback de base de datos (si aplica)
mongorestore --drop --db sentinel_prod /backup/previous-version/
```

