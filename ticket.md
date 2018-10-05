# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso ticket:

Este recurso contará con los siguientes campos:

* [id]: código autoincrementable
* [asunto]: Título del ticket
* [descripción]: breve resumen de la incidencia que presenta el usuario
* [fechaGeneracion]: fecha en que se creó el ticket
* [idCliente]: cliente que genera el ticket
* [idPrioridad]: prioridad con que se atenderá la incidencia
* [idEstado]: estado del trámite
* [idResponsable]: usuario asignado para tramitar el ticket
* [fechaCambioEstado]: fecha en que la solicitud del cliente es atendida y por ende, cambia de estado


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
