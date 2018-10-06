# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso cliente:

Este recurso contará con los siguientes campos:

* [id]: código autoincrementable
* [nombre]: almacenará el nombre completo del cliente o empresa que puede generar tickets
* [correo]: correo de contacto con el cliente
* [documento]: documento de identidad del cliente o NIT de la empresa
* [teléfono]: teléfono de contacto del cliente

Ejemplo en mocky.io: http://www.mocky.io/v2/5bb8bdc23000006900f93c1c


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                       | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                                   | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                        | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                                   | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                                | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
