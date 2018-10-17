# HelpDesk
Trabajo final - Ingeniería de software II UCEVA

Descripción del recurso empresas:

Este recurso contará con los siguientes campos:

* [id]: (primary key, int) NIT de la empresa
* [nombre] (string)  Nombre de la empresa

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

 El campo de `:nombre:` es obligatorio.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc7382432000059310b072f

```json
Empresas
{
    "id": 1,
	"nombre": "Ingenio Margarita"
}
```

## Método PUT
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

## Método GET
#### Index

Lista toda las instancias del recurso `:resource:`. No se modifica ningún campo.

#### Show

Retorna la instancia identificada por `:id:` del recurso `:resource:`. No se modifica ningún campo.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73856320000d0290b0730

```json
Empresas
{
    "id": 1
}
```

## Método DELETE
#### Destroy

Elimina la instancia identificada por `:id:` del recurso `:resource:`.

Ejemplo en mocky.io: http://www.mocky.io/v2/5bc73856320000d0290b0730

```json
Empresas
{
    "id": 1
}
```