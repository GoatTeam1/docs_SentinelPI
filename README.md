
---
# Sentinel Pi
### Sentinel PI
<p align="justify"> El aumento de los ciberataques a nivel mundial ha generado la necesidad urgente de contar con mecanismos de detección temprana que permitan mitigar riesgos y reforzar la seguridad en redes y sistemas críticos. En este contexto surge Sentinel Pi, un proyecto innovador diseñado como un honeypot inteligente basado en Raspberry Pi, cuyo propósito principal es actuar como una herramienta de bajo costo, accesible y adaptable para la detección temprana de amenazas informáticas. Este sistema busca no solo identificar y registrar intentos de intrusión, sino también ofrecer un entorno de análisis que permita comprender mejor los patrones de ataque y, a partir de ello, fortalecer la ciberdefensa de instituciones y organizaciones que requieran un monitoreo constante.

La arquitectura de Sentinel Pi está pensada de manera modular y escalable. En su núcleo, la Raspberry Pi funciona como un honeypot capaz de simular servicios comunes como SSH, FTP o Telnet, con el objetivo de atraer a potenciales atacantes y recopilar información sobre los intentos de acceso no autorizados. Todos los registros generados son procesados mediante una API centralizada desarrollada en Spring Boot, que asegura un flujo estructurado de datos hacia una base de datos confiable. Este enfoque permite manejar información sensible de manera segura y ordenada, garantizando la integridad de los registros y la consistencia de los eventos capturados.

Una de las características diferenciadoras de Sentinel Pi es su enfoque en la visualización distribuida de datos. Además de la interfaz web, el sistema incluye una aplicación desarrollada en Kotlin para Smart TV, lo que permite a los equipos de seguridad consultar de forma inmediata las métricas más relevantes en entornos de trabajo colaborativo o salas de monitoreo. De esta manera, los datos obtenidos del honeypot no permanecen ocultos en registros técnicos, sino que son expuestos como herramientas estratégicas para la toma de decisiones.

El proyecto también contempla requisitos no funcionales clave como la escalabilidad mediante contenedores en Docker Compose, la comunicación segura usando HTTPS y JWT, la portabilidad hacia diferentes dispositivos y navegadores, y la tolerancia a fallos frente a desconexiones o interrupciones temporales. Estos atributos garantizan que Sentinel Pi no sea una solución rígida, sino un sistema adaptable a diversos contextos institucionales, desde universidades hasta pequeñas empresas o dependencias gubernamentales que buscan robustecer su postura de seguridad sin invertir en costosas infraestructuras.

Sentinel Pi se apoya en prácticas ágiles y herramientas de modelado como UML, DFD y Redes de Petri, que han permitido definir de manera clara los casos de uso, los componentes principales y la interacción entre módulos. Asimismo, la documentación asociada al proyecto sigue los lineamientos del estándar IEEE 830, asegurando que los requisitos, restricciones y escenarios futuros estén formalmente especificados y disponibles para la comunidad.
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
Sentinel Pi es un sistema honeypot inteligente implementado sobre Raspberry Pi, diseñado para detectar y registrar intentos de intrusión, analizar amenazas con Python, y visualizarlas mediante un panel web en React y una app para Smart TV con Kotlin.
</p>

---

### PLANTEAMIENTO DEL PROBLEMA

<p align="justify">
Sentinel Pi es un sistema honeypotimplementado sobre Raspberry Pi, diseñado para detectar y registrar intentos de intrusión, analizar amenazas con Python, y visualizarlas mediante un panel web en React y una app para Smart TV con Kotlin. Este proyecto combina bajo costo, portabilidad y escalabilidad para ofrecer una solución accesible en entornos de ciberseguridad.

La arquitectura del sistema se centra en la Raspberry Pi como dispositivo principal, simulando servicios vulnerables para atraer atacantes y recopilar datos de sus actividades. Estos registros son enviados a una API desarrollada en Spring Boot, que centraliza la información, la almacena en bases de datos seguras y permite el análisis posterior. El uso de contenedores Docker y un diseño modular asegura que el sistema pueda adaptarse fácilmente a distintas instituciones sin comprometer su funcionamiento.

El panel web en React proporciona visualización en tiempo real de intentos de acceso, estadísticas históricas y patrones de ataque, utilizando librerías de gráficos como Recharts. Por su parte, la aplicación en Smart TV, desarrollada en Kotlin, está orientada a salas de monitoreo, facilitando la supervisión colaborativa.

En conjunto, Sentinel Pi democratiza la ciberseguridad, brindando a universidades, empresas y gobiernos una herramienta práctica, flexible y confiable para fortalecer su defensa digital.

</p>

---

### PROPUESTA DE SOLUCION
<p align="justify">
En respuesta al creciente número de ciberataques que amenazan diariamente la integridad de empresas, instituciones y servicios públicos, se plantea el desarrollo de Sentinel Pi, una solución práctica, accesible y orientada a la detección temprana de posibles intrusiones mediante el uso de dispositivos Raspberry Pi configurados como honeypots personalizados. Este enfoque busca ofrecer una herramienta tangible para monitorear y analizar el comportamiento de posibles atacantes antes de que logren comprometer activos críticos, reforzando así la seguridad en infraestructuras tecnológicas con bajo costo de implementación.

El proyecto contempla la creación de una plataforma web en React y una aplicación para dispositivos inteligentes, incluyendo Smart TV con Kotlin, que permitirán la visualización en tiempo real de los intentos de intrusión captados por el honeypot. Estos entornos ofrecerán reportes interactivos y estadísticas generadas con Python y librerías de análisis de datos, facilitando la comprensión de patrones de ataque, su frecuencia y los vectores más comunes utilizados por los atacantes.

La configuración del honeypot será adaptable a las necesidades particulares de cada organización, con el objetivo de atraer atacantes en un entorno controlado y seguro que no ponga en riesgo la infraestructura operativa. Toda la información recolectada será enviada a una API centralizada en Spring Boot, que se encargará de procesar, almacenar y clasificar los registros en una base de datos MongoDB para garantizar escalabilidad y eficiencia.

Sentinel Pi considera aspectos de seguridad avanzados, como la comunicación cifrada mediante HTTPS y autenticación con JWT, además de una arquitectura modular desplegada con Docker Compose para facilitar la portabilidad y el escalamiento en distintos entornos institucionales.

En conjunto, esta propuesta representa una solución integral que combina detección temprana, análisis forense y visualización intuitiva, otorgando a las instituciones una gran herramienta para reforzar sus defensas cibernéticas y anticiparse a posibles amenazas.

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

| Nombre                        | Usuario             | Puesto |
|-------------------------------|---------------------|--------|
| Leslie Janet Aparicio Castro   | [leslie-aparicio](https://github.com/leslie-aparicio)        | Documentadora       |
| Carlos Armando Aranda Hernández            | [Carlicsus](https://github.com/Carlicsus)       |   Desarrollador Backend     |
| José Alejandro Briones Arroyo    | [MotaBytes](https://github.com/MotaBytes)             |  Desarrollador del Honeypot y DecSecOps      |
| Diego Hernández Mota           | [alexba2004](https://github.com/alexba2004)       |   Desarrollador Frontend     |
| Jazziel Rodríguez López    | [JazzoLopez](https://github.com/JazzoLopez)             |  Desarrollador Backend     |


  

---


### ORGANIGRAMA DEL EQUIPO
  <img src="img/Organigrama Sentinel Pi (2).png" width="80%" style="padding: 10px;" />



---

### DIAGRAMA DE GANTT

  <img src="img/img/gantt_sentinel.drawio.png" width="80%" style="padding: 10px;" />

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
