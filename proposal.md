# Propuesta TP DSW

## Grupo
### Integrantes
* Calvi Alfie, María Laura (Leg. 51465)
* 

### Repositorios
* [frontend app](https://github.com/lauracalvi5/tp-dsw-frontend-2025)
* [backend app](https://github.com/lauracalvi5/tp-dsw-backend-2025)


## Tema
### Descripción
* Una plataforma que facilita la búsqueda y reserva de estacionamientos en tiempo real. Permite a los usuarios encontrar espacios disponibles en garajes, aplicar filtros según sus necesidades y gestionar reservas de manera sencilla. Ideal para optimizar tiempo y reducir el estrés al estacionar.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Vehículo<br>2. CRUD Usuario<br>3. CRUD Tipo Estacionamiento<br>4. CRUD Cochera|
|CRUD dependiente|1. CRUD Vehículo {depende de} CRUD Tipo Vehículo<br>2. CRUD Estacionamiento {depende de} CRUD Tipo Estacionamiento|
|Listado<br>+<br>detalle| 1. Listado de estacionamientos filtrado por ubicacion y precio, muestra nombre y disponibilidad => detalle CRUD Estacionamiento<br> 2. Listado de reservas filtrado por fecha, muestra id reserva, fecha inicio y fin de reserva, estado (activa, cancelada y vencida) y patente del vehiculo => detalle muestra datos completos de la reserva y del vehiculo|
|CUU/Epic|1. Reservar una cochera en un estacionamiento <br>2. Registrar entrada de vehiculo|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Vehículo<br>2. CRUD Usuario<br>3. CRUD Tipo Estacionamiento<br>4. CRUD Cochera<br>5. CRUD Vehículo<br>6. CRUD Estacionamiento|
|CUU/Epic|1. Reservar una cochera en un estacionamiento <br>2. Registrar entrada de vehiculo<br>3.Administración de cocheras <br>4. Registrar salida de vehiculo y facturación de estadía|


### Alcance Adicional Voluntario


|Req|Detalle|
|:-|:-|
|Listados |1. Reserva del día filtrado por fecha, vehículo, cochera y estado <br>2. Historial de calificaciones filtrado por usuario muestra datos del usuario y de cada calificación, incluyendo fecha, estacionamiento calificado, ubicación, puntuación, comentario y tipo de vehículo.|
|CUU/Epic|1. Calificar estacionamiento<br>2. Cancelación de reserva|
|Otros|1. Envío de confirmacion de reserva por email|
