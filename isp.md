# Principio de Segregacion de Interfaces (ISP)

El Principio de Segregación de Interfaces (ISP) forma parte de los principios SOLID y establece que una clase no debería verse obligada a implementar interfaces que no utiliza. En otras palabras, es mejor tener varias interfaces específicas y pequeñas que una única interfaz genérica y grande. Este principio promueve la cohesión, evita la dependencia innecesaria y mejora la mantenibilidad del código. 
Puede ser fundamental para optimizar el sistema de gestión de turnos al abordar problemas relacionados con la sobrecarga de responsabilidades en las interfaces y la dificultad de escalabilidad.

## Motivacion

El problema surge cuando sistema de gestión de turnos utiliza una única interfaz general llamada, por ejemplo: GestionDeTurnos, con métodos que abarcan tareas diversas como: reservar turnos, cancelar citas, generar reportes estadísticos, enviar notificaciones, registrar pacientes nuevos.
El problema surge cuando distintas partes del sistema o diferentes usuarios (administradores, médicos y pacientes) necesitan implementar esta interfaz. Algunos de estos roles solo requieren unas pocas funcionalidades, pero terminan siendo forzados a implementar métodos innecesarios que no usan, violando el principio ISP. 
El ISP propone dividir la interfaz general en interfaces más pequeñas y específicas, adaptadas a las necesidades de los distintos actores del sistema como por ejemplo: división de interfaces, asignación de interfaces, esto permite una mejor cohesion/escalabilidad/mantenibilidad.

### Ejemplo

Un ejemplo podría ser el sistema de pago en una tienda. Se puede ir a comprar un café en una cafetería. El establecimiento ofrece varias formas de pago: efectivo, tarjeta de crédito, pago móvil, entre otras. Sin embargo, cada método de pago tiene su propia interfaz específica. Por ejemplo: terminal de tarjetas: solo procesa tarjetas de crédito y débito. Aplicaciones móviles: solo aceptan pagos digitales como billeteras virtuales. Caja registradora: Acepta efectivo.
Cada opción de pago tiene una interfaz separada que solo ofrece las funcionalidades necesarias para ese tipo de transacción, evitando que un sistema tenga métodos innecesarios para ciertos clientes. Así como en el principio de segregación de interfaces, cada usuario usa solo lo que necesita sin verse obligado a manejar métodos irrelevantes.

![Principio de Segregación de Interfaces (ISP)](https://github.com/user-attachments/assets/e8ec4fe7-8e01-432a-8940-a9175e59bcaa)


[Estructura de clases](https://drive.google.com/file/d/18iVn_fwCLfVJvihi94y3ZTvcb7meb1V7/view?usp=sharing)
