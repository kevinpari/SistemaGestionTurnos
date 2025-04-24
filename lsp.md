# Principio de Sustitución de Liskov (LSP)

Este principio está vinculado al uso de la herencia en diseño orientado a objetos, nos dice que una subclase debe comportarse como su clase padre sin romper reglas. Si una subclase no puede actuar exactamente como la clase base, no debería ser una subclase.
En el sistema de gestión de turnos médicos, se creó una clase base Usuario y varias subclases como Paciente, Médico y Administracion. Sin embargo, algunas subclases sobrescribían métodos heredados de forma que rompían la lógica general del sistema. Por ejemplo, si un método esperaba un objeto Usuario y se le pasaba un Administrador, podía fallar porque este no tenía implementado correctamente un comportamiento esperado, como agendar turnos.

## Motivacion

El problema en el sistema de gestion de turnos aparece cuando algunas de estas subclases modificaban métodos heredados de manera que rompían la lógica del sistema. Por ejemplo, en ciertos contextos se esperaba trabajar con un objeto del tipo Paciente, pero al utilizar un Administrador, el sistema fallaba porque esta subclase no implementaba adecuadamente funciones clave como la de reservar turnos. Esto iba en contra del principio, ya que todas las subclases de Paciente deberían poder emplearse de forma intercambiable sin que se altere el funcionamiento del sistema.
Para evitar que el sistema fallara o se volviera inestable, se implementaban excepciones manuales, lo que aumentaba la complejidad y el riesgo de cometer errores.
El principio de sustitución de Liskov establece que una subclase debe ser capaz de sustituir a su clase padre sin afectar el funcionamiento del sistema. En este caso, si un Administrador no puede realizar las mismas acciones que un Usuario (como solicitar turnos), se estaría violando este principio.
La solución consistió en redefinir de manera precisa qué acciones podía llevar a cabo cada tipo de usuario. De esta forma, cada uno se limitaba a sus propias funciones, lo que hizo el sistema más organizado, seguro y fácil de gestionar.

### Ejemplo

Si tomamos de ejemplo a los vehiculos, se debe suponer que estamos diseñando un sistema de vehículos en una empresa de transporte. Supongamos que tenemos una clase base vehículo, y de esa clase derivan otras más específicas, como coche y camión. El principio de Sustitución de Liskov (LSP) dice que si tienes un objeto de tipo Vehículo, deberías poder sustituirlo por un Camión o un Coche sin que el sistema rompa o se comporte incorrectamente.


![Principio de Sustitución de Liskov (LSP)](https://github.com/user-attachments/assets/ed256c49-ab10-4554-88fc-9599b43c8f6e)

[Estructura de clases](https://drive.google.com/file/d/1sQPSaQ-vaJoUqP3zjGgciabn1oldVDHf/view?usp=sharing)
