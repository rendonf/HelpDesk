# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso tecnico ticket:

Este recurso contará con los siguientes campos:

* [id]:  (primary key, int) Es un autoincrementable
* [tecnico]: (foreign key, int) Asignación del tecnico resposanble de un ticket
* [ticket]: (foreign key, int) Asignación del ticket a un tecnico

Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  


## Método POST
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

## Método PUT
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

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c6d83200005a000b03f6

```json
TecnicoTicket
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c6d83200005a000b03f6

```json
TecnicoTicket
{
    "id": 1
}
```