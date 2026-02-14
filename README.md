# 📄 Informe Técnico del Taller

## 🔖 Taller BPMN - segunda sesión 

## 👥 Integrantes del equipo
- Rita Trindade da Cruz (ritatrcr)
- Brandon Merchan Sandoval (merchito12)
- Daniel Felipe Forero Sánchez (DanielForero14)


## 🧠 Descripción general del trabajo
El objetivo de este taller fue modelar un proceso de negocio real utilizando la notación BPMN, identificando claramente eventos, actividades, decisiones, actores y puntos críticos del flujo.
El trabajo se desarrolló en dos etapas: primero, el modelado de un caso base común Clínica Salud Viva trabajado en clase, y posteriormente la aplicación del mismo enfoque a un cliente real, Elite Airsoft, permitiendo comparar un proceso idealizado con uno que se ejecuta actualmente de forma manual o semi-manual.
Esta metodología permitió comprender cómo BPMN se adapta tanto a contextos con alto nivel de automatización como a procesos operativos más informales.
## 🔧 Proceso de desarrollo
El desarrollo del trabajo inició con el análisis del caso base de la Clínica Salud Viva, identificando el flujo principal de agendamiento de citas, los actores involucrados y las interacciones con sistemas de información. A partir de este análisis, se construyó un primer modelo BPMN en clase, el cual fue ajustado con base en la retroalimentación del docente.
Posteriormente, el equipo seleccionó el proceso real de agendamiento de reservas de Elite Airsoft, el cual es gestionado principalmente por WhatsApp. Se recopilaron los pasos reales del proceso, se definieron los carriles cliente y asistente, y se modelaron decisiones críticas como la disponibilidad, la congelación de fechas y la validación de pagos.
Como herramienta principal se utilizó draw.io, permitiendo iterar rápidamente sobre el modelo hasta representar fielmente el proceso actual sin introducir mejoras que no existieran en la realidad del negocio.


## 🧩 Análisis del modelo propuesto
### Estructura del modelo
El modelo BPMN se estructura mediante:
•	Un evento de inicio asociado a la intención del cliente de realizar una reserva.
•	Actividades secuenciales claramente definidas.
•	Gateways exclusivos (XOR) para la toma de decisiones.
•	Eventos de tiempo y mensajes para representar esperas y notificaciones.
•	Eventos de fin diferenciando entre cita confirmada y no confirmada.
### Representación de las necesidades del cliente
El modelo refleja de manera fiel las necesidades del cliente al mostrar:
•	La dependencia del contacto directo vía WhatsApp.
•	La intervención humana en la validación de disponibilidad y pagos.
•	La importancia del control del tiempo para evitar bloqueos innecesarios de fechas.
### Supuestos tomados
•	El proceso modelado representa el estado actual, no un proceso optimizado.
•	La validación de pagos y disponibilidad es manual.
•	No existe un sistema automatizado de reservas ni notificaciones automáticas


## 📈 Diagrama final entregado
![Modelo BPMN - Clínica Salud Viva](/images/Clínica.png)
![Modelo BPMN - Empresa](/images/Empresa.png)

## 📋 Tabla de actores

| Nombre del elemento       | Tipo    | Descripción                                   | Responsable        |
|---------------------------|---------|-----------------------------------------------|--------------------|
| Paciente / Cliente        | Actor   | Usuario que solicita una cita o reserva       | Cliente            |
| Asistente                 | Actor   | Persona encargada de gestionar reservas y pagos | Empresa            |
| Sistema de agendamiento   | Sistema | Plataforma digital (en el caso de la clinica)                | Clínica            |
| WhatsApp                  | Canal   | Medio de comunicación principal               | Cliente / Empresa  |
| Base de datos             | Sistema | Registro de citas o reservas                  | Empresa            |



## 🔍 Investigación complementaria
### Tema investigado:
Buenas prácticas en modelado de procesos con BPMN y su aplicación en procesos reales.

### Resumen:
La notación BPMN (Business Process Model and Notation) es un estándar ampliamente utilizado para representar procesos de negocio de forma clara y comprensible tanto para usuarios técnicos como no técnicos. Entre las buenas prácticas más relevantes se encuentra el uso adecuado de eventos, la correcta separación de responsabilidades mediante carriles y la limitación de la complejidad visual del modelo.
En el contexto del taller, estas buenas prácticas permitieron modelar procesos reales sin perder claridad, incluso cuando estos presentan múltiples decisiones manuales, como ocurre en el caso de Elite Airsoft. La investigación evidenció que BPMN no solo es útil para documentar procesos actuales, sino que también sirve como base para futuras mejoras y automatizaciones.


## 📚 Referencias
•  [1] Universidad de La Sabana. Material de clase – Arquitectura Empresarial. s.f.
https://unisabanaedu.sharepoint.com/sites/ArquitecturaEmpresarial/SitePages/Material-de-clase.as

•  [2] Object Management Group (OMG). Business Process Model and Notation (BPMN) Specification. s.f.
https://www.omg.org/spec/BPMN/

•  [3] Chakray Consulting. ¿Qué es BPMN y para qué sirve?. s.f.
https://chakray.com/es/que-es-el-bpmn-y-para-que-sirve/

•  [4] BbT0IN3y2V4. Introducción a BPMN – Modelado de procesos. YouTube, s.f.
https://www.youtube.com/watch?v=BbT0IN3y2V4

---

