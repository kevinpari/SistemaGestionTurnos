# Principio de Abierto/Cerrado (OCP)

El objetivo principal del Principio de Abierto/Cerrado es permitir que el software sea extensible para nuevas funcionalidades sin necesidad de modificar su código ya existente. En el sistema utilizado para administrar los turnos médicos, la parte encargada de enviar notificaciones estaba construida de forma inflexible. Toda la lógica relacionada con el envío de mails, mensajes de texto o llamadas telefónicas se encontraba en una única unidad. Cada vez que era necesario incorporar un nuevo medio de notificación (como WhatsApp o notificaciones telefonicas), se debía modificar directamente ese código, lo que provocaba errores, afectaba funcionalidades previas y dificultaba el mantenimiento general del sistema.

El Principio Abierto-Cerrado (OCP) plantea que el sistema debe estar abierto para ampliacion, pero cerradas para modificación. Para solucionar este problema, se propone diseñar una interfaz de que pueda enviar notificaciones, como envío de mensajes, correos electrónicos y llamadas, sin modificar el código original. De esta manera, si en el futuro se agrega un nuevo canal de contacto, solo será necesario implementar una nueva clase sin afectar el funcionamiento de las existentes.

## Motivacion

En el sistema de gestión de turnos médicos, uno de los problemas más comunes aparecía cuando se necesitaba incorporar nuevas funcionalidades, como diferentes tipos de notificaciones dirigidas a pacientes y medicos. Inicialmente, solo se utilizaba el correo electrónico, pero con el tiempo al actualizarse los medios de contacto se fue agregando el SMS como otra alternativa de contacto. El inconveniente era que cada vez que se agregaba una nueva forma de notificación, había que modificar el codigo de funcionamiento ya existente y esto puede ocasionar fallas en las funciones ya vigentes, ademas de que el sistema se vuelve mas inestable ante mas cambios. El principio de abierto/cerrado (OCP) propone que los sistemas deben diseñarse de forma en la que puedan ampliarse sin necesidad de alterar el código original que ya está en funcionamiento. Es decir, permitir incorporar nuevas características/funciones sin modificar lo vigente.

### Ejemplo

Tenemos como ejemplo una máquina de café automática en una oficina, inicialmente, la máquina tiene tres botones: café negro, café con leche, chocolate caliente y cada boton prepara una bebida especifica. Si se agrega una nueva bebida (cappuccino), tenés que abrir la máquina, modificar su programación interna, cambiar circuitos, etc. Esto es riesgoso, costoso y puede romper otras funciones.
Una máquina de café diseñada con el principio OCP tendría ademas de las funciones ya vigentes lo siguiente: un sistema modular, donde cada bebida es un módulo intercambiable, en la se puede  agregar una nueva bebida, solo agregándo un nuevo cartucho/módulo o software, sin tocar el código/máquina base. De esta manera solo se agregaria las nuevas funciones sin tocar lo que ya funciona.


![Principio de Abierto_Cerrado (OCP)](https://github.com/user-attachments/assets/d84a1995-d205-49d2-ad7b-6f45043ee663)

[Estructura de clases](https://drive.google.com/file/d/1xiZ2DPH3rEGgFowO40Eje5HCoM9fIAv6/view?usp=sharing)


