# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso respuesta:

Este recurso contará con los siguientes campos:

* [id]:  (primary key, int) Es un autoincrementable
* [respuesta]: (string) Asignación del tecnico resposanble de un ticket
* [fechaRespuesta]: (date) Fecha en que se realiza la respuesta de un ticket
* [ticket]: (foreign key, int) Ticket al que corresponde la respuesta
* [usuario]: (foreign key, string) Usuario al que corresponde la respuesta (cliente o tecnico) el llamado se realiza con el `:codigo:`

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

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6cc1f3200007c000b0408

```json
Respuestas
{
    "id": 1,
    "respuesta": "El usuario al que desea ingresar se encuentra eliminado",
    "fechaRespuesta": "30/9/2018",
    "ticket": 32,
    "usuario": "T012"
}}
```

## Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`.

El campo `:respuesta:` se pueden modificar.

Ejemplo en mocky.io:http://www.mocky.io/v2/5bc6cd2d3200005a000b040a

```json
Respuestas
{
    "id": 1,
    "respuesta": "El usuario al que desea ingresar no existe",
    "fechaRespuesta": "30/9/2018",
    "ticket": 32,
    "usuario": "T012"
}
```

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6cdbc3200005a000b040f

```json
Respuestas
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6cdbc3200005a000b040f

```json
Respuestas
{
    "id": 1
}
```