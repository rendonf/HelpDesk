# HelpDesk
Trabajo final - Ingenier�a de software II UCEVA

Descripci�n del recurso archivo:

Este recurso contar� con los siguientes campos:

* [id]:  (primary key, int) Es un autoincrementable
* [archivo]: (object) Asignaci�n del tecnico resposanble de un ticket
* [respuesta]: (foreign key, int) Respuesta a la que corresponde el archivo multimedia

Estos recursos contar�n con 4 operaciones:

| Operaci�n             | Endpoint                                                            | Descripci�n                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:` 


## M�todo POST
#### Create

Crea una instacia del recurso `:resource:`.

Los campos `:tecnico:` y `:ticket:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6d39232000067000b042f

```json
Archivos
{
    "id": 4,
    "archivo": null,
    "respuesta": 3
}
```

## M�todo GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ning�n campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ning�n campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6d3ba32000067000b0431

```json
Archivos
{
    "id": 4
}
```

## M�todo DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6d3ba32000067000b0431

```json
Archivos
{
    "id": 4
}
```