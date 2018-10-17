# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso moduloEmpresa:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [empresa] (foreign key, int)  Código que refiere al recurso *empresa*
* [modulos]: (foreign key, int) JSON que refiere al campo `:id:` del recurso *modulo* de los módulos activos

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

## Método PUT
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

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc75423320000dd2d0b07eb

```json
moduloEmpresa
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc75423320000dd2d0b07eb

```json
moduloEmpresa
{
    "id": 1
}
```