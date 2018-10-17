# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso cliente:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) Código autoincrementable
* [codigo] (string)  C + entero incrementable correspondiente
* [nombre]: (string) Almacenará el nombre completo del cliente o empresa que puede generar tickets
* [clave]: (String) Contraseña del cliente
* [correo]: (string) Correo de contacto con el cliente
* [NIT]: (foreign, int) NIT de la empresa
* [telefono]: (int) Teléfono de contacto del cliente

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

El campo `:codigo:` es un identificador de los roles que se genera en el Fronend . Las entradas de `:nombre:`, `:clave:`, `:correo:` y `:telefono:` son campos obligatorios, el campo `:NIT:` se ingresa por default dependiendo del espacio de ayuda.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc67f0b32000060000b034b

```json
Cliente
{
    "id": 1,
	"codigo": "C0001",
	"nombre": "Jeeremías Aragón",
	"clave": "miclave01",
	"correo": "jere@correo.com",
	"NIT": 5278295,
	"telefono": 3998887766
}
```

## Método PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo las entradas de `:nombre:`, `:clave:, ``:correo:` y `:telefono:` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc67ffb32000084000b034d

```json
Cliente
{
    "id": 1,
    "codigo": "C0001",
    "nombre": "Jeeremías Aragón",
    "clave": "otraclave2",
    "correo": "jere@correo.com",
    "NIT": 5278295,
    "telefono": 555555555
}
```

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.


#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc680473200004e000b034e

```json
Cliente
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc680473200004e000b034e

```json
Cliente
{
    "id": 1
}
```