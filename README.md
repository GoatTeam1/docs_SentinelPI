
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
El incremento de los ataques informáticos ha generado un clima de inseguridad tecnológica en múltiples sectores. Las instituciones educativas, empresas y organizaciones públicas enfrentan amenazas constantes que comprometen no sólo sus datos, sino también su reputación. Un incidente de seguridad que derive en la pérdida de confianza puede provocar desde sanciones legales hasta la quiebra de una organización.
Este proyecto busca empoderar a las instituciones con una herramienta económica y efectiva de detección temprana de amenazas, brindando visibilidad sobre los intentos de ataque que reciben, lo cual permitirá implementar medidas preventivas antes de que se concrete una intrusión. Al usar un honeypot personalizado según el contexto de la organización, se mejora la pertinencia de los datos obtenidos y se fomenta una cultura proactiva en seguridad informática.

</p>

---

### PROPUESTA DE SOLUCION
<p align="justify">
En respuesta al creciente número de ciberataques que amenazan diariamente la integridad de empresas, instituciones y servicios, se plantea el desarrollo de una solución práctica, accesible y orientada a la detección temprana de posibles intrusiones mediante el uso de dispositivos Raspberry Pi configurados como honeypots personalizados. Esta propuesta busca ofrecer una herramienta tangible para monitorear y analizar el comportamiento de posibles atacantes antes de que logren comprometer activos críticos.

El proyecto contempla la creación de una plataforma web y una aplicación para dispositivos inteligentes que permitan la visualización en tiempo real de los ataques recibidos por el honeypot. Este será adaptado según las necesidades particulares de cada organización, simulando servicios y entornos reales para atraer posibles atacantes sin poner en riesgo la infraestructura operativa. La información recolectada será fundamental para identificar patrones de ataque, vulnerabilidades y métodos utilizados por los intrusos.

</p>

---

### OBJETIVO GENERAL

<p align="justify">Diseñar e implementar un sistema de seguridad pasiva basado en Raspberry Pi, que funcione como un honeypot para detectar y registrar intentos de intrusión en redes informáticas, proporcionando a las empresas e instituciones una interfaz web accesible para visualizar y analizar los intentos de ataque en tiempo real, con el fin de fortalecer sus medidas de ciberseguridad de manera proactiva.
</p>


---

### OBJETIVOS ESPECIFICOS

<p align="justify"><strong>Configurar el Raspberry Pi como un honeypot capaz de detectar y registrar intentos de intrusión.</p>

<p align="justify"><strong>Mapa interactivo</strong>Desarrollar una plataforma web que permita visualizar en tiempo real los intentos de acceso captados por el sistema.</p>

<p align="justify"><strong>Implementación de alertas</strong>Implementar un sistema centralizado que recopile, almacene y analice los datos generados por el dispositivo.</p>

<p align="justify"><strong>Implementación de reportes eficiente</strong>Facilitar a las instituciones el monitoreo y la comprensión de los ataques mediante gráficos, reportes y estadísticas.</p>

<p align="justify"><strong>Desarrollar una aplicación para dispositivos inteligentes que permita la consulta de los datos de seguridad capturados por el honeypot desde diferentes entornos.</p>

<p align="justify"><strong>Validar el sistema mediante pruebas en un entorno controlado simulando escenarios reales de ataque.</p>

<p align="justify"><strong>Asegurar que el sistema pueda escalar o adaptarse a distintas instituciones con necesidades específicas.</p>





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






