# Principio de Abierto/Cerrado (OCP)

El objetivo principal del Principio de Abierto/Cerrado es permitir que el software sea extensible para nuevas funcionalidades sin necesidad de modificar su código ya existente. En el sistema utilizado para administrar los turnos médicos, la parte encargada de enviar notificaciones estaba construida de forma inflexible. Toda la lógica relacionada con el envío de mails, mensajes de texto o llamadas telefónicas se encontraba en una única unidad. Cada vez que era necesario incorporar un nuevo medio de notificación (como WhatsApp o notificaciones telefonicas), se debía modificar directamente ese código, lo que provocaba errores, afectaba funcionalidades previas y dificultaba el mantenimiento general del sistema.

El Principio Abierto-Cerrado (OCP) plantea que el sistema debe estar abierto para ampliacion, pero cerradas para modificación. Para solucionar este problema, se propone diseñar una interfaz de que pueda enviar notificaciones, como envío de mensajes, correos electrónicos y llamadas, sin modificar el código original. De esta manera, si en el futuro se agrega un nuevo canal de contacto, solo será necesario implementar una nueva clase sin afectar el funcionamiento de las existentes.

## Motivacion

En el sistema de gestión de turnos médicos, uno de los problemas más comunes aparecía cuando se necesitaba incorporar nuevas funcionalidades, como diferentes tipos de notificaciones dirigidas a pacientes y medicos. Inicialmente, solo se utilizaba el correo electrónico, pero con el tiempo al actualizarse los medios de contacto se fue agregando el SMS como otra alternativa de contacto. El inconveniente era que cada vez que se agregaba una nueva forma de notificación, había que modificar el codigo de funcionamiento ya existente y esto puede ocasionar fallas en las funciones ya vigentes, ademas de que el sistema se vuelve mas inestable ante mas cambios. El principio de abierto/cerrado (OCP) propone que los sistemas deben diseñarse de forma en la que puedan ampliarse sin necesidad de alterar el código original que ya está en funcionamiento. Es decir, permitir incorporar nuevas características/funciones sin modificar lo vigente.

## Ejemplo

