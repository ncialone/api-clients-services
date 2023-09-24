## Descripción del Proyecto

Este repositorio contiene un proyecto de API REST que permite la creación de clientes y servicios, con la capacidad de vincular determinados servicios a determinados clientes.

### Endpoints API

A continuación, se describen los endpoints disponibles en este proyecto:

### Clientes
#### Listar Todos los Clientes
Endpoint: `GET /clients`

Descripción: Este endpoint te permite obtener una lista de todos los clientes registrados en el sistema.

#### Crear un Nuevo Cliente
Endpoint: `POST /clients`

Descripción: Utiliza este endpoint para crear un nuevo cliente en la base de datos. Debes proporcionar los datos del cliente en el cuerpo de la solicitud.

#### Obtener Detalles de un Cliente
Endpoint: `GET /clients/{client}`

Descripción: Este endpoint te permite obtener los detalles de un cliente específico identificado por su ID.

#### Actualizar un Cliente
Endpoint: `PUT /clients/{client}`

Descripción: Utiliza este endpoint para actualizar la información de un cliente existente. Debes proporcionar los nuevos datos del cliente en el cuerpo de la solicitud.

#### Eliminar un Cliente
Endpoint: `DELETE /clients/{client}`

Descripción: Este endpoint te permite eliminar un cliente específico de la base de datos.

### Servicios
#### Listar Todos los Servicios
Endpoint: `GET /services`

Descripción: Este endpoint te proporciona una lista de todos los servicios disponibles en el sistema.

#### Crear un Nuevo Servicio
Endpoint: `POST /services`

Descripción: Utiliza este endpoint para crear un nuevo servicio. Debes proporcionar los detalles del servicio en el cuerpo de la solicitud.

#### Obtener Detalles de un Servicio
Endpoint: `GET /services/{service}`

Descripción: Este endpoint te permite obtener los detalles de un servicio específico identificado por su ID.

#### Actualizar un Servicio
Endpoint: `PUT /services/{service}`

Descripción: Utiliza este endpoint para actualizar la información de un servicio existente. Debes proporcionar los nuevos datos del servicio en el cuerpo de la solicitud.

#### Eliminar un Servicio
Endpoint: `DELETE /services/{service}`

Descripción: Este endpoint te permite eliminar un servicio específico de la base de datos.

### Vinculación de Clientes y Servicios
#### Vincular un Servicio a un Cliente
Endpoint: `POST /clients/service`

Descripción: Utiliza este endpoint para vincular un servicio específico a un cliente. Debes proporcionar los IDs del cliente y del servicio en el cuerpo de la solicitud.

#### Desvincular un Servicio de un Cliente
Endpoint: `POST /clients/service/detach`

Descripción: Este endpoint te permite desvincular un servicio previamente vinculado a un cliente. Debes proporcionar los IDs del cliente y del servicio en el cuerpo de la solicitud.

#### Obtener Clientes de un Servicio
Endpoint: `POST /services/clients`

Descripción: Utiliza este endpoint para obtener la lista de clientes que están vinculados a un servicio específico. Debes proporcionar el ID del servicio en el cuerpo de la solicitud.
