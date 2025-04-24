# Principio de Inversion de Dependencias (DIP)

El Principio de Inversión de Dependencias (DIP, por sus siglas en inglés) es uno de los principios fundamentales del diseño de software dentro de SOLID. Establece que: los módulos de alto nivel no deben depender de los módulos de bajo nivel, ambos deben depender de abstracciones. Las abstracciones no deben depender de los detalles, los detalles deben depender de las abstracciones.
En términos más simples, en lugar de que una clase concreta dependa directamente de otra clase concreta, ambas deben depender de una interfaz o abstracción. Esto permite mayor flexibilidad, facilita la extensibilidad del código y reduce el acoplamiento entre los componentes.

## Motivacion

En el sistema de turnos medicos, uno de los mayores problemas era que los módulos de alto nivel (como la lógica principal del sistema, que gestiona la programación de citas y la asignación de médicos) dependían directamente de implementaciones de bajo nivel (como bases de datos específicas o sistemas de notificación como el correo electrónico). Este enfoque hacía que cualquier cambio en estos componentes de bajo nivel tuviera un gran impacto en toda la aplicación.
Para resolver este problema, se implementó el principio de inversión de dependencias (DIP), reorganizando la arquitectura para que la lógica central pasara a depender de abstracciones como interfaces para servicios de notificación, acceso a datos, entre otros; en lugar de depender directamente de soluciones particulares. Por ejemplo, en vez de vincular el sistema de turnos a un servicio de correo específico, se definió una interfaz genérica llamada “Servicio de Notificaciónes”, la cual se complementa con el sistema sin necesidad de saber lo que conlleva por detras. Esto facilitó la posibilidad de modificar o sustituir el sistema de notificación sin impactar el resto de la aplicación. De esta manera, el código principal quedó desacoplado de los detalles técnicos, volviendo la solución más adaptable, sencilla de probar y más fácil de mantener con el paso del tiempo.

### Ejemplo 

Un ejemplo puede ser necesitar cargar un teléfono, pero cada país tiene un tipo diferente de enchufe. En lugar de que cada dispositivo dependa directamente de un tipo específico de toma de corriente, los aeropuertos y hoteles suelen tener adaptadores universales o puertos USB que permiten conectar distintos tipos de dispositivos sin importar su origen. De esta forma podemos visualizar como ingresa el Principio de Inversión de Dependencias.
Este diseño hace que el sistema sea flexible y fácil de actualizar sin afectar a los dispositivos. En programación, este mismo principio permite que los módulos dependan de abstracciones en lugar de implementaciones concretas, facilitando la escalabilidad y el mantenimiento del código.


![Principio de Inversión de Dependencias (DIP)](https://github.com/user-attachments/assets/2d3c840a-9621-4a89-a58e-e3df72f2bc2c)

[Estructura de Clase](https://drive.google.com/file/d/1tpfL3IL2obrOL2iZVlhVRyaQgbvS_e3j/view?usp=sharing)
