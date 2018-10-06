# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Este es el documento de diseño de la API para gestionar terceros de la solución. Esta API cuenta con 7 recursos:

* [Ticket](ticket.md): `helpDesk/tree/documentation/Resourses/ticket` 
* [GestionTicket](gestionTicket.md): `helpDesk/documentation/Resourses/gestionTicket`
* [Prioridad](prioridad.md): `helpDesk/documentation/Resourses/prioridad`
* [Estado](estado.md): `helpDesk/documentation/Resourses/estado`
* [Usuario](usuario.md): `helpDesk/documentation/Resourses/usuario`
* [Cliente](cliente.md): `helpDesk/documentation/Resourses/cliente`
* [Rol](rol.md): `helpDesk/documentation/Resourses/rol`


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
