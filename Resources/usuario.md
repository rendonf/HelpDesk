# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso usuario:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [nombre]: (string) Nombre completo del usuario
* [clave]: (string) Contraseña de ingreso
* [rol]: (foreign, int) Llave foránea al recurso "Rol"


Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3e4d730000064007586db


Estos recursos contarán con 5 operaciones:

| Operación             | Endpoint                                                            | Descripción                                                            |
| --------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| __Create__            | `POST helpDesk/develop/:resource:`                                  | Crea una instancia del recurso `:resource:`.                           |
| __Update__            | `PUT helpDesk/develop/:resource:/:id:`                              | Modifica la instancia identificada por `:id:` del recurso `:resource:` |
| __Index__             | `GET helpDesk/develop/:resource:`                                   | Lista toda las instancias del recurso `:resource:`                     |
| __Show__              | `GET helpDesk/develop/:resource:/:id:`                              | Retorna la instancia identificada por `:id:` del recurso `:resource:`  |
| __Destroy__           | `DELETE helpDesk/develop/:resource:/:id:`                           | Elimina la instancia identificada por `:id:` del recurso `:resource:`  


##Método POST
#### Create

Crea una instacia del recurso `:resource:`.  Las entradas `:nombre:`, `:clave:` y `:rol:` son campos obligatorios.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3e4d730000064007586db

```json
Usuario
{
    "id": 1,
    "nombre": "Eduar Alexander Marin",
    "clave": "01clave01",
    "rol": 1
}
```

##Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo las entradas de `:nombre:`, `:clave:` y `:rol:` se pueden modificar.

Ejemplo en mocky.io:

```json

```

##Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io:

```json

```

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: 

```json

```

##Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io:

```json

```