# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Este es el documento de diseño de la API para gestionar terceros de la solución. Esta API cuenta con 7 recursos:

* [Ticket](Resources/ticket.md): `HelpDesk/blob/documentation/Resources/ticket` 
* [GestionTicket](Resources/gestionTicket.md): `HelpDesk/blob/documentation/Resources/gestionTicket`
* [Prioridad](Resources/prioridad.md): `HelpDesk/blob/documentation/Resources/prioridad`
* [Estado](Resources/estado.md): `HelpDesk/blob/documentation/Resources/estado`
* [Usuario](Resources/usuario.md): `HelpDesk/blob/documentation/Resources/usuario`
* [Cliente](Resources/cliente.md): `HelpDesk/blob/documentation/Resources/cliente`
* [Rol](Resources/rol.md): `HelpDesk/blob/documentation/Resources/rol`


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
