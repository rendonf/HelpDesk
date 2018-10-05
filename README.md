# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Este es el documento de diseño de la API para gestionar terceros de la solución. Esta API cuenta con 7 recursos:

* [Ticket](ticket.md): `helpDesk/documentation/ticket` 
* [GestionTicket](gestionTicket.md): `helpDesk/documentation/gestionTicket`
* [Prioridad](prioridad.md): `helpDesk/documentation/prioridad`
* [Estado](estado.md): `helpDesk/documentation/estado`
* [Usuario](usuario.md): `helpDesk/documentation/usuario`
* [Cliente](cliente.md): `helpDesk/documentation/cliente`
* [Rol](rol.md): `helpDesk/documentation/rol`


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
