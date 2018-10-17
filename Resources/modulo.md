# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso modulo:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [nombre] (string)  Nombre del módulo
* [descripcion]: (string) Descripción del módulo

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

 Los campos `:nombre:` y `:descripcion:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b1c320000053b0b073c

```json
Modulos
{
    "id": 1,
    "nombre": "Ventas",
    "descripcion": "El modulo de ventas administra las incidencias de cada trabajo y muestra estadísticas en tiempo real de los trabajos"
}
```

## Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo el campo `:nombre` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b65320000003b0b073f

```json
Modulos
{
    "id": 1,
    "nombre": "Ventas",
    "descripcion": "El modulo de ventas administra las incidencias de cada trabajo"
}
```

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b8f320000cd280b0740

```json
Modulos
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b8f320000cd280b0740

```json
Modulos
{
    "id": 1
}
```