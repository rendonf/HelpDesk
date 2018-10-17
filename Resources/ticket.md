# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso ticket:

Este recurso contará con los siguientes campos:

* [id]:  (primary key, int) Código autoincrementable
* [asunto]: (string) Título del ticket 
* [modulo]: (foreign key, int) Indica el respectivo módulo donde se encuentra el problema, apunta al recurso *modulo*
* [descripcion]: (string) Breve resumen de la incidencia que presenta el usuario
* [fechaCreacion]: (date) Fecha en que se creó el ticket
* [cliente]: (foreign key, int) Cliente que genera el ticket 
* [prioridad]: (foreign key, int) Prioridad con que se atenderá la incidencia
* [estado]: (foreign key, int) Estado del trámite
* [fechaCambioEstado]: (date) Fecha en que la solicitud del cliente es atendida y por ende, cambia de estado

Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`


## Método POST
#### Create

Crea una instacia del recurso `:resource:`. 

Los campos de `:asunto:`, `:modulo:`, `:descripcion:` y `:cliente:` son obligatorios, el campo  `:fechaCreacion:` lo genera el sistema, el campo `:estado:` lo genera el sistema por default con la etiqueta en *Espera*  y el campo `:prioridad:` es asignado después de una previa revisión del ticket.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc757d8320000013b0b07ff

```json
Ticket
{
    "id":1,
    "asunto":"no puedo iniciar sesión",
    "modulo": null,
    "descripcion":"me robaron la contraseña y requiero cambiarla urgentemente",
    "fechaCreacion":"5/10/2018",
    "cliente":34,
    "prioridad":null,
    "estado":1,
    "fechaCambioEstado":"5/10/2018"
}
```

## Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo las entradas de `:prioridad:`, `:estado:`,  y `:fechaCambioEstado:` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6bc2e3200004e000b03cb

```json
Ticket
{
    "id":1,
    "asunto":"no puedo iniciar sesión",
    "modulo": null,
    "descripcion":"me robaron la contraseña y requiero cambiarla urgentemente",
    "fechaCreacion":"5/10/2018",
    "cliente":34,
    "prioridad":3,
    "estado":2,
    "fechaCambioEstado":"15/10/2018"
}
```

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6bd4c3200007c000b03ce

```json
Ticket
{
    "id":1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6bd4c3200007c000b03ce

```json
Ticket
{
    "id":1
}
```