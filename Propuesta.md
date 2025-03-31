# Propuesta TP DSW

## Grupo
### Integrantes
* 51036 - Santos Juan Pablo
* 51871 - Toloza Laureano
* 52726 - Garrido Alejo
* 52133 - Alfieri Agustin

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
Gestión de turnos de un consultorio médico
### Descripción
La solución web permitirá la gestión integral de profesionales en diversas áreas médicas, incluyendo la carga de datos y la asignación de prácticas correspondientes. Los usuarios podrán solicitar turnos, recibir notificaciones y recordatorios automáticos. Además, se implementará la gestión de descuentos por obras sociales en distintas prácticas, junto con un sistema de administración de pagos eficiente y seguro.

### Modelo
![imagen del modelo]()  TODO: Definir con el grupo

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo de Practica<br>2. CRUD Tipo de Profesional<br>3. CRUD Obra social|
|CRUD dependiente|1. CRUD Medico {depende de} CRUD Tipo de Profesional<br>2. CRUD Cliente {depende de} CRUD Obra social|
|Listado<br>+<br>detalle| 1. Listado de Profesionales disponibles filtrando por Tipo de practica, Tipo de Profesional => detalle CRUD Habitacion<br> 2. Listado de reservas filtrado por rango de fecha, muestra nro de habitación, fecha inicio y fin estadía, estado y nombre del cliente => detalle muestra datos completos de la reserva y del cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
