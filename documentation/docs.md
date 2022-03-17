# Door-of-drums API

## Introduction

Welcome to the Door-of-drums API. You can use our API to access Door-of-drums API endpoints, which can get information on the songs that are used in the game, the user info and the records of the users.

## Authentication

Door-of-drums uses API keys to allow access to the API. For this you have to be register on the [game page](https://doors-of-drums.github.io/Pagina-web/).

Door-of-drums expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: key`

You must replace `key` with your personal API key.

## User

### Get user info

This endpoint retrieves all the info from all users.

#### HTTP Request

`GET https://doors-of-drums.github.io/Pagina-web/documentation/Usuario/user.json`

#### Result of this query

```json
{
  "1": {
    "nombre_usuario": "mastergamer",
    "pais": "México",
    "fecha_nacimiento": "2000-08-09T05:00:00.000Z",
    "contrasenia": "fastpass",
    "correo": "usuario1@gmail.com",
    "apellido_ma": "López",
    "apellido_pa": "Pérez",
    "genero": "mujer",
    "telefono": "5552518625",
    "Foto": "imagen1.jpg",
    "status" : "active"
  },
  "2": {
    "nombre_usuario": "justNeto",
    "pais": "México",
    "fecha_nacimiento": "2000-08-09T05:00:00.000Z",
    "contrasenia": "fastpass",
    "correo": "usuario1@gmail.com",
    "apellido_ma": "López",
    "apellido_pa": "Pérez",
    "genero": "hombre",
    "telefono": "5552518625",
    "Foto": "imagen2.jpg",
    "status" : "active"
  },
  "3": {
    "nombre_usuario": "sofi:)",
    "pais": "México",
    "fecha_nacimiento": "2000-08-09T05:00:00.000Z",
    "contrasenia": "fastpass",
    "correo": "usuario1@gmail.com",
    "apellido_ma": "López",
    "apellido_pa": "Pérez",
    "genero": "mujer",
    "telefono": "5552518625",
    "Foto": "imagen1.jpg",
    "status" : "active"
  }
}

```

## Records

### Get all records

This endpoint retrieves the records from all users.

#### HTTP Request

`GET https://doors-of-drums.github.io/Pagina-web/documentation/Historial/historial.json`


#### Result of this query

```json
{
  "historial": {
    "id_historial": 1,
    "id_usuario": 1,
    "puntos_por_partida": 10,
    "fecha_del_juego": "2022-03-16T00:36:10.194Z",
    "id_cancion": 1,
    "tiempo_jugado": 40
  }
}
```

## Song

### Get song info

This endpoint retrieves the informations of all the songs of the game.

#### HTTP Request

`GET https://doors-of-drums.github.io/Pagina-web/documentation/Cancion/cancion.json`

#### Result of this query

```json
{
  "1": {
    "nombre": "Martinillo",
    "duracion": "3:42",
    "genero": "pop",
    "ritmo": "alto",
    "dificultad": "alta"
  },

  "2": {
    "nombre": "Pin Pon es un muñeco",
    "duracion": "2:04",
    "genero": "infantil",
    "ritmo": "bajo",
    "dificultad": "baja"
  }, 

  "3": {
    "nombre": "Las ruedas del autobús",
    "duracion": "2:14",
    "genero": "infantil",
    "ritmo": "medio",
    "dificultad": "media"
  }
}
```
