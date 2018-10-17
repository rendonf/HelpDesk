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

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6847232000082000b034f

```json
Prioridades
{
    "prioridad": [
        {"id": 1, "descripcion": "Baja"},
        {"id": 2, "descripcion": "Media"},
        {"id": 3, "descripcion": "Alta"}
    ]
}
```