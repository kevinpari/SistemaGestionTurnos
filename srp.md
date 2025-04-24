# Principio de responsabilidad unica(SRP)

El Principio de Responsabilidad Única (SRP) es el primero de los principios SOLID de diseño orientado a objetos, y establece que "Una clase debe tener una sola razón para cambiar".Esto significa que cada clase debe cumplir una única función o responsabilidad dentro del sistema. Si una clase tiene más de una responsabilidad, entonces está mal diseñada según este principio.
En el Sistema de Gestion de Turnos, este principio se aplica debido a que se detectaron varios componentes que combinan mulptiples tareas dentro de una sola unidad. Es decir, una parte del sistema era responsable de gestionar turnos, validar disponibilidad medica, informar al paciente y registrar la informacion en una base de datos. El principio de responsabilidad única propone separar esas funciones en partes iguales, para que cada una se ocupe de una sola tarea, por ejemplo: una se encarga de generar turnos, otra de confirmar horario segun la disponibilidad, otra gestionar los avisos y otra de registrar la informacion.

## Motivacion

Uno de lo grandes inconvenientes que presentaba el sistema de **Recepcion** contaba con multiples tareas de manera simultanea, por ejemplo: agendar un turno, comprobar la disponibilidad del profesional, notificar al paciente y guardar toda esa información en la base de datos. Esto generaba que una alta dependencia hacia esta clase gerando diversos problemas, como la interpretacion de codigo, cualquier cambio afectaba a todo lo demás, los errores eran más difíciles de localizar y corregir.

### Ejemplo
Si en un restaurante hay una unica persona que hace todas las tareas como: tomar ordenes, cocinar la comida, cobrarle a los clientes, limpiar las mesas. En el caso de que haya mucho caudal de trabajo o algun error, es probable que esta persona en algun momento colapse debido que cuenta con demasiadas responsabilidades.
Al aplicar el principio SRP se efectuaria una mejora en las tareas debido a que habria un individuo en particular que estaria a cargo de esas tareas, por ejemplo: Camarero (toma pedidos y los lleva a la cocina), cocinero (prepara la comida), cajero (cobrar al cliente), personal de limpieza (limpiar las mesas). De esta manera se llevaria un sistema mas ordenado, flexible y eficiente, igual que el código que sigue el SRP.

## Estructura de Clases

![Principio de Responsabilidad Única (SRP)](https://github.com/user-attachments/assets/22e0c240-976d-4623-9b7b-ef4abffea115)

[Estructura de clases](https://drive.google.com/file/d/1ELG_gbLS8WPo2m7L6OYDAp7fkZxk0yZ8/view?usp=sharing)
