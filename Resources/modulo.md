# HelpDesk
Trabajo final - Ingenier�a de software II UCEVA

Descripci�n del recurso modulo:

Este recurso contar� con los siguientes campos:

* [id]: (primary key, int) C�digo autoincrementable
* [nombre] (string)  Nombre del m�dulo
* [descripcion]: (string) Descripci�n del m�dulo

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

 Los campos `:nombre:` y `:descripcion:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b1c320000053b0b073c

```json
Modulos
{
    "id": 1,
    "nombre": "Ventas",
    "descripcion": "El modulo de ventas administra las incidencias de cada trabajo y muestra estad�sticas en tiempo real de los trabajos"
}
```

## M�todo PUT
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

## M�todo GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ning�n campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ning�n campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b8f320000cd280b0740

```json
Modulos
{
    "id": 1
}
```

## M�todo DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73b8f320000cd280b0740

```json
Modulos
{
    "id": 1
}
```