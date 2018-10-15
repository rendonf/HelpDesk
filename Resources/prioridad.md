# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso prioridad:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [descripcion]: (string) Nombre de la prioridad en la base de datos

Las prioridades de los tickets serán las siguientes:

-  Baja
-  Media
-  Alta

Array de prioridades en mocky.io: http://www.mocky.io/v2/5bc3ed7430000069007586e4

Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                            |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  


## Método POST
#### Create

Crea una instancia del recurso `:resource:`. La entrada `:descripcion:` es un campo obligatorio.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3ed7430000069007586e4

```json
Prioridades
{
    "prioridad": [
        {"id": 1, "descripcion": "baja"},
        {"id": 2, "descripcion": "media"},
        {"id": 3, "descripcion": "alta"}
    ]
}
```

## Método DELETE
####Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`

Ejemplo en mocky.io:

```json

```