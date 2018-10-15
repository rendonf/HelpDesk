# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso rol:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [descripcion]: (string) Descripcion o nombre de los tipos o roles que tendrán los usuarios registrados.


Ejemplo en mocky.io:http://www.mocky.io/v2/5bc3f98830000064007586f9


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  |

## Método POST
#### Create

Crea una instancia del recurso `:resource:`. La entrada `:descripcion:` es un campo obligatorio.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3f98830000064007586f9

```json
Rol
{
    "id": 1,
    "descripcion": "Responsable"
}
```

## Método DELETE
####Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`

Ejemplo en mocky.io:

```json

```