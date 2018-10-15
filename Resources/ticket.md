# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso ticket:

Este recurso contará con los siguientes campos:

* [id]:  (primary key, int) Código autoincrementable
* [asunto]: (string) Título del ticket 
* [descripcion]: (string) Breve resumen de la incidencia que presenta el usuario
* [fechaGeneracion]: (date) Fecha en que se creó el ticket
* [cliente]: (foreign key, int) Cliente que genera el ticket 
* [prioridad]: (foreign key, int) Prioridad con que se atenderá la incidencia
* [estado]: (foreign key, int) Estado del trámite
* [responsable]: (foreign key, int) Usuario asignado para tramitar el ticket
* [fechaCambioEstado]: (date) Fecha en que la solicitud del cliente es atendida y por ende, cambia de estado

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3dea73000004a007586d4

Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`


##Método POST
#### Create

Crea una instacia del recurso `:resource:`.  Las entradas de `:asunto:`, `:descripcion:`, `:fechaGeneracion:`, `:cliente:` y `:estado:` son campos obligatorios. Los campo de `:prioridad:`, `:responsable:` y `:fechaCambioEstado:`  son asignados después de una revisión previa.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3dea73000004a007586d4

```json
Ticket
{
    "id":1,
    "asunto":"no puedo iniciar sesión",
    "descripcion":"me robaron la contraseña y requiero cambiarla urgentemente",
    "fechaGeneracion":"5/10/2018",
    "cliente":1,
    "prioridad":1,
    "estado":2,
    "responsable":5,
    "fechaCambioEstado":"5/10/2018"
}
```

##Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo las entradas de `:prioridad:`, `:estado:`, `:responsable:` y `:fechaCambioEstado:` se pueden modificar.

Ejemplo en mocky.io:

```json

```

##Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io:

```json

```

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: 

```json

```

##Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io:

```json

```