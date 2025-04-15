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

   


