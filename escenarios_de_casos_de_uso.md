# Escenario de caso de uso 

## 1) Registro Inicial

### Descripción General

El usuario puede registrarse en sistema con el fin de solicitar turnos medicos, eso lo puede llevar a cabo tanto él como una recepcionista por medio de unos simples paso.

### Flujo de eventos

1. **Solicitud de turno**  
   - El paciente solicita un turno por primera vez

2. **El recepcionista/usuario ingresa al sistema**  
   - Al intentar solicitar un turno el sistema presenta un requisito.  

3. **Solicitud y verificacion**  
   - El sistema verifica que el nuevo usuario no cuente con datos ya ingresados en la plataforma.

4. **Validacion de datos**  
   - El paciente debe completar y validar datos personales y medicos. 

5. **Eleccion de turno**  
   - En caso de ya estar registrado el usuario puede seleccionar el turno deseado segun requerimientos.
  
6. **Notificacion de registro**  
   - Ya ingresado en sistema el sistema le envia una notificacion de registro.
  
### Precondiciones

 - El usuario no debe estar registrado en el sistema.
 - El usuario debe haber brindar datos validos de registro.

### Poscondiciones 

 - El usuario genera un perfil de paciente.
 - El usuario contara con una plataforma rapida a la mano

[Caso de Uso 1 - Registro Inicial](https://docs.google.com/spreadsheets/d/1iDibAocPatfpSnckenbusRCkZAPGzphCoc3sMy9lmjA/edit?usp=sharing)


## 2) Gestion de turnos

### Descripción General

El usuario/recepcionista puede generar un turno medico de manera repida, eficaz y comoda.

### Flujo de eventos

1. **Ingreso a sistema**  
   - El usuario ingresa al sistema.

2. **El usuario ingresa sus datos de paciente**  
   - El usuario ingresa la sistema con sus datos personales, ya registrado.

3. **Solicitud de turno**  
   - El sistema puede elegir el medico deseado segun especialidad/fecha/horario.

4. **Inconveniente de solicitud**  
   - Llegado a tener algun problema el usuario, puede generar sus solicitud por medio de un recepcionista. 

5. **Confirmacion de datos**  
   - El usuario de confirmar sus datos para efectuar la reserva.
  
6. **Datos de reserva**  
   - El sistema le envia una confirmacion del turno por mail.
  
### Precondiciones

 - El usuario debe estar registrado en el sistema.
 - El usuario no debe tener mas de un turno en un mismo dia y horario

### Poscondiciones 

 - El usuario confirma turno segun necesidades especificas
 - Se registra la fecha y hora de la reserva en el sistema.
 - El usuario tendra una reserva formal via mail.

[Caso de Uso 2 - Gestion de Turnos](https://docs.google.com/spreadsheets/d/1YqXoRkZ8ns9GaxsD1G4IxjYA0E8N67veo2R2syTCskc/edit?usp=sharing)

## 3) Notificaciones

### Descripción General

El sistema enviara informacion y avisos por asignaciones/cancelaciones al usuario/medico, debido a que de esta manera se llevara un prevenira ausencias medicas o de pacientes.

### Flujo de eventos

1. **Verificacion de reserva**  
   - El usuario debera contar con una reserva efectuada anteriomente.

2. **Avisos previos**  
   - El usuario contara con un aviso de confirmacion en forma de notificacion.

3. **Modificacion/cancelacion de turno**  
   - El sistema alertara al usuario en caso de que se efecute una modificacion o cancelacion de turno.

4. **Confirmacion de turno**  
   - El sistema avisara al usuario dias previos al usuario para que este al tanto de su solicitud.

5. **Reconfirmacion**  
   - El sistema reconfirmara al usuario por la plataforma mail, para que el mismo este al tanto del turno elegido.
  
### Precondiciones

 - El usuario debe contar con un turno elegido.

### Poscondiciones 

 - El usuario quedara alertado ante cualquier cambio con respecto al turno seleccionado.

[Caso de Uso 3 - Notificaciones](https://docs.google.com/spreadsheets/d/1HQ6j5cDjQse3wKrqOjckHI9Vclj_MEZl8BB-2inHmQA/edit?usp=sharing)

## 4) Historial de turnos

### Descripción General

El usuario o cualquier personal medico podra visualizar el historial de turnos hasta el dia de la fecha, esto permitira llevar un mejor control tanto desde el ambito profesional (medico especialista) como para el paciente.

### Flujo de eventos

1. **Ingreso**  
   - El usuario/medico/recepcionista deben ingresar a sistema.

2. **Logueo de usuario**  
   - El usuario debera loguearse en sistema con sus datos personales.

3. **Logueo administrativo**  
   - Tanto el sector administrativo/medico debe ingresar en sistema con usuarios de personal disignado.

4. **Visualizacion de historial**  
   - Los usuarios con acceso al sistema podran visualizar el hisotirail de turnos, por una parte los pacientes verificaran su historial personal y por otro el personal medico el paciente requerido.
  
### Precondiciones

 - El usuario debe contar con turnos asignados previamente.
 - El personal adminisitrativo debe contar con usuarios administrativos.

### Poscondiciones 

 - El usuario podra visualizar algun resultado medico/receta brindado anteriomente.
 - EL personal medico podra llevar un mejor control de los pacientes tratados o a tratar.

[Caso de Uso 4 - Hostorial de turnos](https://docs.google.com/spreadsheets/d/1XCcC-tH_H2AmWhlmQI8Zb9EEPM45lzWu5yNALwGzNnE/edit?usp=sharing)

## 5) Calendario de turnos

### Descripción General

Por medio de un calendario de turnos, el personal medico podra llevar un mejor control con respecto a los turnos brindados/solicitados por parte de los usuarios.

### Flujo de eventos

1. **Asignacion de turnos**  
   - El personal administrativo otorga turnos a pacientes segun las solcitudes que se presenten dia a dia.

2. **Planificacion**  
   - El personal verificara los dias siguientes para continuar brindando turnos en los dias disponibles.

3. **Control de turnos**  
   - El personal adminsitrativo/medico tendra un control segun las solicitudes efectuadas por los usuario por medio del sistema.

4. **Modificacion de turnos**  
   - El personal modificara los turnos que no puedan concetrase en caso de contar con mucha demanda o poco personal medico, en base al dia mas solicitado.
  
5. **Notificacion de aviso**
   - El sistema/persona medico enviara una notificacion al usuario en caso de llevar a cabo una cancelacion/modificacion/confirmacion de turno.
  
### Precondiciones

 - Contar con pacientes con turnos confirmados y vigentes.

### Poscondiciones 

 - Un mejor control administrativo con respecto a los turnos otorgados.

[Caso de Uso 5 - Calendario de turnos](https://docs.google.com/spreadsheets/d/1Vd2VLOPPkbVEgE8nfFKkTMAk1Eg9RLoz9nYtfIaQEZQ/edit?usp=sharing)



   


