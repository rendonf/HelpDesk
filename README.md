# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Este es el documento de diseño de la API para gestionar terceros de la solución. Esta API cuenta con 7 recursos:

* [Ticket](ticket.md): `HelpDesk/blob/documentation/Resourses/ticket` 
* [GestionTicket](gestionTicket.md): `HelpDesk/blob/documentation/Resourses/gestionTicket`
* [Prioridad](prioridad.md): `HelpDesk/blob/documentation/Resourses/prioridad`
* [Estado](estado.md): `HelpDesk/blob/documentation/Resourses/estado`
* [Usuario](usuario.md): `HelpDesk/blob/documentation/Resourses/usuario`
* [Cliente](cliente.md): `HelpDesk/blob/documentation/Resourses/cliente`
* [Rol](rol.md): `HelpDesk/blob/documentation/Resourses/rol`


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
