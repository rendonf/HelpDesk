# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso tecnico:

Este recurso contará con los siguientes campos:

* [id]:  (primary key, int) Es un autoincrementable
* [codigo]: (string) T + entero incrementable correspondiente
* [nombre]: (string) Nombre completo del usuario
* [clave]: (string) Contraseña de ingreso
* [documento]: (int) Documento de identidad del tecnico
* [correo]: (string) Correo de contacto del tecnico
* [telefono]: (int) Teléfono de contacto del tecnico
* [rol]: (foreign, int) Llave foránea al recurso "Rol"

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

Los campos `:nombre:`, `:clave:`, `:documento:`, `:correo:`, `:telefono:` y `:rol:` son obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c1c932000067000b03e2

```json
Tecnico
{
    "id": 1,
    "codigo": "T015",
    "nombre": "Eduar Alexander Marin",
    "clave": "01clave01",
    "documento": 111233853,
    "correo":"eduar@correo.com",
    "telefono": 2314536543,
    "rol": 3
}
```

## Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`.  

Los campos `:nombre:`, `:clave:`, `:correo:`, `:telefono:` y `:rol:` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c3023200002c000b03e6

```json
Tecnico
{
    "id": 1,
    "codigo": "T015",
    "nombre": "Eduar Alexander Marin",
    "clave": "otracosa3",
    "documento": 111233853,
    "correo":"alex@correo.com",
    "telefono": 1111112233,
    "rol": 3
}
```

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c37d32000086000b03e7

```json
Tecnico
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc6c37d32000086000b03e7

```json
Tecnico
{
    "id": 1
}
```