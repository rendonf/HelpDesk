# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso prioridad:

Este recurso contará con los siguientes campos:

* [id]: código autoincrementable
* [descripción]: nombre de la prioridad en la base de datos

Las prioridades de los tickets serán las siguientes: 

-Baja
-Media
-Alta

Arry de prioridades en mocky.io: http://www.mocky.io/v2/5bb7e8703000002a00f93b46

Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |
