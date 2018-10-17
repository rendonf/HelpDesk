# HelpDesk
Trabajo final - Ingenier�a de software II UCEVA

Descripci�n del recurso empresas:

Este recurso contar� con los siguientes campos:

* [id]: (primary key, int) NIT de la empresa
* [nombre] (string)  Nombre de la empresa

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

 El campo de `:nombre:` es obligatorio.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc7382432000059310b072f

```json
Empresas
{
    "id": 1,
	"nombre": "Ingenio Margarita"
}
```

## M�todo PUT
#### Update

Modifica la instancia identificada por `:id:` del recurso `:resource:`. Solo el campo `:nombre` se pueden modificar.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc737f6320000cd280b072d

```json
Empresas
{
    "id": 1,
    "nombre": "Ingenio Maria"
}
```

## M�todo GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ning�n campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ning�n campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73856320000d0290b0730

```json
Empresas
{
    "id": 1
}
```

## M�todo DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73856320000d0290b0730

```json
Empresas
{
    "id": 1
}
```