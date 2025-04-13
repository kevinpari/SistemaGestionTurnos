# Introduccion al Diseño Orientado a Objetos

## 1. ¿Que es la programacion orientada a objetos?

La **Programacion orientada a objetos** es un enfoque de programacion que organiza y estructura el software en torno a "objetos", los cuales son instancias de clases. Las clases son como plantillas que definen las propiedades (atributos) y comportamientos (metodos) de los objetos.

Este enfoque es importante porque ofrece ventajas como la reutilizacion de programas, escalabilidad de aplicaciones, facilidad en compresion y mantenimiento de un codigo.


## 2. Cuatro fundamentos de POO

#### Estos son los 4 principios permiten que los objetos interactúen entre sí. 

### Abstracion

* Consiste en definir clases simplificando la realidad. 
Por ejemplo: Una "Radio", como usuario solo utilizas el "encendido" y "apagado".

### Encapsulamiento

* Consiste en ocultar o encapsular los datos y los detalles de implementación dentro de una clase.
Por ejemplo: Una "Cuenta Bancaria" no permite acceso directo al dinero fisico, solo mediante transacciones u operaciones.

### Herencia

* Permite la definición de múltiples clases usando las propiedades de otras clases.
Por ejemplo: Un "Automovil deportivo", presenta la clase de automovil pero puede presentar distintas caracteristicas segun marca/modelo/puertas.

### Polimorfismo

* Permite que una misma acción tenga diferentes comportamientos según el objeto.
Por ejemplo: Un "Animal" debido a que comparten la emision de algun sonido, pero siendo de difereten clase (perro/gato).


## 3. Requisitos Iniciales del Sistema

* Registro inicial para llevar un control personalizado de cada paciente.
* Gestionar turnos segun especialidad requerida.
* Notificar a los usuarios sobre la asignacion/cancelacion de turnos.
* Visualizacion de historial de turnos.
* Calendario y control de turnos para profesionales medicos. 

## 4. Casos de uso

### Registro inicial

* **Actor:** Usuario.
* **Descripción:** Permite al registrarse en la plataforma.
* **Flujo principal:**
1. El usuario ingresa a la plataforma.
2. Ingresa sus datos en sistema para registro.
3. Validacion y corroboracion de datos.
4. Confirmacion de cuenta por medio de un mail.
* **Precondiciones:** El usuario no debe estar registrado previamente.
* **Postcondiciones:** El usuario queda registrado en la plataforma.


### Gestion de turnos

* **Actor:** Usuario.
* **Descripcion:** El usuario elige un turno segun la especialidad requerida.
* **Flujo principal:**
1. El usuario selecciona una especialidad.
2. Elige dia y horario (siempre y cuando este disponible).
3. Confirmacion de turno y posterior de envio del mismo por mail.
* **Precondiciones:** El usuario debe estar registrado.
* **Postcondiciones:** Turno deseado confirmado.


### Notificaciones 

* **Actor:** Plataforma/Aplicacion.
* **Descripcion:** La plataforma envia informacion y avisos por asignaciones/cancelaciones.
* **Flujo principal:** 
1. El sistema verifica la agenda de turnos.
2. Dias previos al turno se enviara un aviso al usuario en forma de recordatorio.
3. En caso de cancelacion, tambien se dara aviso al usuario.
* **Precondiciones:** El usuario debe tener un turno confirmado.
* **Postcondiciones:** El usuario quedara avisado sobre las confirmacion o posibles cambios.


### Historial de turnos

* **Actor:** Usuario/Plataforma.
* **Descripcion:** El usuario podra ver turnos/consultas efectuadas anteriormente.
* **Flujo principal:** 
1. El usuario debe estar su cuenta personal.
2. Debe ingresar en historial de turnos.
3. Podra elegir un turno/consulta efectuada anteriormente segun filtros de meses/especialidad.
* **Precondiciones:** El usuario debera haber tomado un pedido previamente.
* **Postcondiciones:** El mismo podra llevar un control sobre consultas previas y detalles de las mismas.

### Calendario de turnos 

* **Actor:** Medicos/profesionales y personal administrativo.
* **Descripcion:** El personal de centro podra llevar un control diario/mensual sobre los turnos asignados.
* **Flujo principal:**
1. Varios usuario deberan haber solicitados  turnos previamente.
2. Visualizacion mensual de turnos.
3. Recoordinacion de turnos manteniendo un orden diario segun dias/horarios/especialidades.
* **Precondiciones:** Debe haber actividad y uso de la plataforma.
* **Postcondiciones:** Mejor control sobre turnos y recoordinacion de los mismos en caso de contar con mayor demanda.

