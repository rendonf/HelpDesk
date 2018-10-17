# HelpDesk
Trabajo final - Ingenier�a de software II UCEVA

Descripci�n del recurso moduloEmpresa:

Este recurso contar� con los siguientes campos:

* [id]: (primary key, int) C�digo autoincrementable
* [empresa] (foreign key, int)  C�digo que refiere al recurso *empresa*
* [modulos]: (foreign key, int) JSON que refiere al campo `:id:` del recurso *modulo* de los m�dulos activos

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

 Los campos `:empresa:` y `:modulos:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73e80320000053b0b075b

```json
moduloEmpresa
{
    "id": 1,
    "empresa": 21643,
    "modulos": [
       			 {"id": 4},
       			 {"id": 7},
       			 {"id": 2},
       			 {"id": 12}
	]
}
```

## M�todo PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo el campo `:nombre` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc753a4320000532d0b07e8

```json
moduloEmpresa
{
    "id": 1,
    "empresa": 21643,
    "modulos": [
        {"id": 4},
        {"id": 7},
        {"id": 2},
        {"id": 12},
        {"id": 8},
        {"id": 10}
    ]
}
```

## M�todo GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ning�n campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ning�n campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc75423320000dd2d0b07eb

```json
moduloEmpresa
{
    "id": 1
}
```

## M�todo DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc75423320000dd2d0b07eb

```json
moduloEmpresa
{
    "id": 1
}
```