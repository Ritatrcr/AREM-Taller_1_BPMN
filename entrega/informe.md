# Procesos de agendamiento de las reservas  
**Elite Airsoft – Funza, Cundinamarca**

## 1. Introducción
El presente informe tiene como objetivo describir y analizar el proceso de agendamiento de reservas de la empresa **Elite Airsoft**, modelado mediante la notación **BPMN**. A partir de este análisis, se explicará el proceso actual y se identificarán las diferencias frente a un caso base teórico.

Elite Airsoft es una empresa dedicada a la organización de partidas de airsoft, ubicada en el municipio de Funza. Uno de los principales motivos para la selección de esta empresa es el fácil acceso a la información del negocio, dado que se mantiene una relación directa con los propietarios, lo que permitió comprender con mayor precisión la forma real en que se ejecutan los procesos actualmente.

## 2. Contexto de la empresa y selección del proceso
Elite Airsoft es una empresa relativamente nueva, por lo cual muchos de sus procesos aún se realizan de manera manual o semi-manual, especialmente en la gestión de reservas. Actualmente, el agendamiento de partidas se lleva a cabo principalmente a través de **WhatsApp**, con intervención directa del personal.

Se identificó una oportunidad de mejora clara en este proceso:

- Es un proceso crítico para la operación del negocio.  
- Se repite constantemente.  
- Presenta riesgos de errores humanos, demoras y pérdida de información.  
- Tiene alto potencial de automatización futura.

Por estas razones, se decidió centrar este trabajo inicialmente en el proceso de reservas, dejando otros procesos de la empresa para fases posteriores.

## 3. Descripción del proceso actual
El modelo BPMN desarrollado y representado en el archivo XML corresponde a la situación actual del proceso de agendamiento.

### a) Actores del proceso
El proceso está dividido en dos carriles principales: **Cliente** y **Asistente**.

- **Cliente:** persona interesada en reservar una partida de airsoft.  
- **Asistente:** encargado de gestionar la reserva, validar disponibilidad, pagos y confirmar o cancelar la cita.

**Figura No. 1.** Actores en el proceso.

### b) Flujo del proceso
El proceso inicia cuando el cliente decide crear una reserva, iniciando una conversación por medio de WhatsApp.

1. El cliente inicia el contacto y solicita información sobre la partida.  
2. El asistente solicita los datos necesarios para la reserva, tales como **fecha, hora y número de jugadores**.  
3. Con la información suministrada, el asistente verifica la disponibilidad para la fecha y hora solicitadas.  
   - En caso de no contar con disponibilidad, se solicita al cliente un cambio de fecha u hora.  
   - Si existe disponibilidad, la fecha y hora se congelan temporalmente por un periodo de **dos horas**.  
4. El asistente procede con el método de pago y solicita el comprobante.  
5. Durante el lapso de las dos horas establecidas, el cliente debe confirmar su reserva.  
   - Si el cliente decide confirmar la cita, deberá enviar el comprobante de pago.  
   - En caso de que el cliente no confirme la reserva dentro del tiempo establecido o decida no continuar con el proceso, la cita será cancelada.  
6. El asistente procede a validar el pago recibido:  
   - Si el pago no es válido o no se recibe dentro del tiempo establecido, la reserva se cancela y la fecha y hora son descongeladas.  
   - Si el pago es validado correctamente, notifica la confirmación al cliente, registra la fecha y hora de la reserva y el proceso finaliza con la cita confirmada.

Este flujo refleja la forma en que la empresa opera actualmente, con una alta dependencia del factor humano y de la comunicación manual.

**Figura No. 2.** Proceso inicial de las reservas.  
**Figura No. 3.** Proceso final de las reservas.

## 4. Diferencias con el caso base
Al comparar el proceso de agendamiento de reservas de Elite Airsoft con un caso base (generalmente soportado por plataformas digitales automatizadas para la gestión de reservas), se identifican las siguientes diferencias clave:

- El proceso no se ejecuta a través de un sistema de reservas, sino mediante mensajería instantánea, lo que limita la automatización y el control del flujo.  
- No existe un sistema automático para la validación de disponibilidad; esta actividad depende completamente del asistente, quien realiza la verificación de manera manual.  
- La confirmación y cancelación de las reservas se llevan a cabo de forma manual, sin notificaciones automáticas.  
- El control del tiempo de congelación de la reserva no es automatizado; requiere seguimiento constante por parte del asistente.  
- El registro de la información de la reserva se realiza manualmente, lo que aumenta la probabilidad de errores y retrabajo.

Estas diferencias evidencian que el proceso actual presenta un menor nivel de madurez digital en comparación con el caso base.

## 5. Justificación del modelo BPMN
El modelo BPMN tiene como propósito principal representar de manera fiel el proceso real de agendamiento de reservas en Elite Airsoft, sin introducir mejoras o supuestos que no correspondan a la situación actual de la empresa.

Para ello, el modelo:

- Documenta el flujo del proceso tal como se ejecuta actualmente.  
- Identifica de forma clara los puntos de decisión críticos, especialmente los relacionados con la disponibilidad y la validación del pago.  
- Muestra las interacciones entre el cliente y el asistente, evidenciando la alta dependencia del factor humano en la operación.

Asimismo, este modelo sirve como base para una futura propuesta orientada a la automatización y optimización del proceso.

Adicionalmente, el uso de BPMN:

- Facilita la comprensión del proceso por parte de los dueños y colaboradores de la empresa.  
- Permite identificar cuellos de botella y tareas repetitivas.  
- Sienta las bases para la futura implementación de herramientas tecnológicas.

