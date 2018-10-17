# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso estado:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [descripcion]: (string)  Nombre del estado en la base de datos

Los estados del tickets serán las siguientes:

-  *Espera* :  Aún no se ha asignado un responsable y dado una prioridad
-  *Proceso* :  Ya se asigno un reponsable y esta en proceso de solución del problema
-  *Resuelta* :  El problema ya ha sido resuelto.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc665ca32000078000b032e

```json
Estados
{
    "estado": [
        {"id": 1, "descripcion": "Espera"},
        {"id": 2, "descripcion": "Proceso"},
        {"id": 3, "descripcion": "Resuelta"}
    ]
}
```