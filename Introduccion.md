# Anexo - Introduccion al Diseño Orientado a Objetos

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
1. El paciente ingresa en sistema.
2. En caso de no contar con un usuario debe registrarse.	
3. El paciente completa un formulario de registro.
4. El paciente debe validar datos personales.
5. Se envia mail de usuario al paciente.
6. El paciente debe validad la cuenta creada por medio de un mail.
* **Precondiciones:** El usuario no debe estar registrado previamente.
* **Postcondiciones:** El usuario queda registrado en la plataforma.
  

### Gestion de turnos

* **Actor:** Usuario.
* **Descripcion:** El usuario elige un turno segun la especialidad requerida.
* **Flujo principal:**
1. El paciente debe iniciar sesion en el sistema.
2. Debe ingresar en la opcion "Solicitar turno".
3. Debe elegir fecha.
4. Debe elegir especialidad.
5. Debe elegir horario.
6. Se envia confirmacion de turno por mail al paciente.
* **Precondiciones:** El usuario debe estar registrado.
* **Postcondiciones:** Turno deseado confirmado.


### Notificaciones 

* **Actor:** Plataforma/Aplicacion.
* **Descripcion:** La plataforma envia informacion y avisos por asignaciones/cancelaciones.
* **Flujo principal:** 
1. El sistema visuliza el calendario mensual de turnos.
2. El paciente ingresa al sistema.
3. El sistema efectua un control de turnos.
4. Verifica que los proximos duas no figuren saturados.
5. En caso de estar saturado, se cancela/modifica turno.
6. Se da aviso al paciente por mail.
7. En caso estar disponible el turno.
8. Se da aviso al cliente por mail para reconfirmacion de turno.
* **Precondiciones:** El usuario debe tener un turno confirmado.
* **Postcondiciones:** El usuario quedara avisado sobre las confirmacion o posibles cambios.


### Historial de turnos

* **Actor:** Usuario/Plataforma.
* **Descripcion:** El usuario podra ver turnos/consultas efectuadas anteriormente.
* **Flujo principal:** 
1. El paciente debe dirigirse al ingreso de usuario.
2. Debe ingresar con su usuario y contraseña.
3. Debe dirigirse a la opcion sistema de turnos.
4. El usuario debe dirigirse a la opcino historial de turnos.
5. Aplicando filtros de busqueda segun el turno requerido.
6. Podra visualizar el turno buscado, siempre y cuando haya usado el sistema por lo menos una vez.
* **Precondiciones:** El usuario debera haber tomado un pedido previamente.
* **Postcondiciones:** El mismo podra llevar un control sobre consultas previas y detalles de las mismas.

### Calendario de turnos 

* **Actor:** Medicos/profesionales y personal administrativo.
* **Descripcion:** El personal de centro podra llevar un control diario/mensual sobre los turnos asignados.
* **Flujo principal:**
1. El personal administrativo debe ingresar al sistema con credenciales administrativas.
2. El persona debe ingresar al calendario mensual de turnos
3. En caso de no contar con turnos disponibles en determinado dia.
4. Efectuaran la cancelacion/modificacion de turno.
5. Daran aviso al cliente por mail.
6. En caso de contar con un turno disponible.
7. Se enviara reconfirmacion de turno al cliente por mail.
* **Precondiciones:** Debe haber actividad y uso de la plataforma.
* **Postcondiciones:** Mejor control sobre turnos y recoordinacion de los mismos en caso de contar con mayor demanda.

![Boceto inicial del diseño de clases](https://github.com/user-attachments/assets/b19f4f15-0f0a-4f58-94ac-e52230139b0d)

