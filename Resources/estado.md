# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso estado:

Este recurso contará con los siguientes campos:

* [id]: código autoincrementable
* [descripción]: breve resumen del estado del ticket, el cual nos indica el procesamiento y estado en que se encuentra la incidencia reportada por un usuario


Ejemplo en mocky.io: http://www.mocky.io/v2/5bbbadea3200007e0027e9e7


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
