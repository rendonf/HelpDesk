# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso usuario:

Este recurso contará con los siguientes campos:

* [id]: código autoincrementable
* [nombre]: nombre completo del usuario
* [id_rol]: llave foránea al recurso "Rol"


Ejemplo en mocky.io: http://www.mocky.io/v2/5bbbaedd3200007a0027e9e9


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
