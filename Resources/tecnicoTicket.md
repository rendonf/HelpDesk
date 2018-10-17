# HelpDesk
Trabajo final - Ingenier�a de software II UCEVA

Descripci�n del recurso tecnico ticket:

Este recurso contar� con los siguientes campos:

* [id]:  (primary key, int) Es un autoincrementable
* [tecnico]: (foreign key, int) Asignaci�n del tecnico resposanble de un ticket
* [ticket]: (foreign key, int) Asignaci�n del ticket a un tecnico

Estos recursos contar�n con 5 operaciones:

| Operaci�n             | Endpoint                                                            | Descripci�n                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  


## M�todo POST
#### Create

Crea una instacia del recurso `:resource:`. 

Los campos `:tecnico:` y `:ticket:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c63532000076000b03f3

```json
TecnicoTicket
{
    "id": 1,
    "tecnico": 4,
    "ticket": 737
}
```

## M�todo PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`.  

El campo `:responsable:` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c69f32000071000b03f4

```json
TecnicoTicket
{
    "id": 1,
    "tecnico": 2,
    "ticket": 737
}
```

## M�todo GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ning�n campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ning�n campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c6d83200005a000b03f6

```json
TecnicoTicket
{
    "id": 1
}
```

## M�todo DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c6d83200005a000b03f6

```json
TecnicoTicket
{
    "id": 1
}
```