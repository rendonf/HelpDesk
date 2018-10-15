# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso cliente:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [nombre]: (string) Almacenará el nombre completo del cliente o empresa que puede generar tickets
* [correo]: (string) Correo de contacto con el cliente
* [NIT]: (int) NIT de la empresa
* [telefono]: (int) Teléfono de contacto del cliente

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3f13030000010007586ed


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

Crea una instacia del recurso `:resource:`.  Las entradas de `:nombre:`, `:correo:` y `:telefono:` son campos obligatorios, el campo `:NIT:` solo es requerido para las empresas.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc3f13030000010007586ed

```json
Cliente
{
    "id": 1,
    "nombre": "Jeeremías Aragón",
    "correo": "jere@correo.com",
    "NIT": 1234567987,
    "telefono": 3998887766
}
```

##Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo las entradas de `:nombre:`, `:correo:` y `:telefono:` se pueden modificar.

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
