API para control de vacunas
Descripción: 
    Esta API permite la conexión entre el videojuego 'Doors of drums' y el sistema web mediante métodos GET, 
    gracias a esta se podrá conocer [datos] aparter de su username (?). 

Parámetros y respuestas esperadas:

ENDPOINT:
https://doors-of-drums.github.io/Pagina-web/[archivos json]

Verbo: GET
Parámetro de entrada esperado: username (?)

Salida: JSON con los datos de la persona:
    [datos]

    CURP (CURP de la persona buscada)
    VACUNAS (lista de las vacunas que se tienen registradas para esa persona, 
    los detalles que incluye cada vacuna son: fecha_de_aplicacion, 
    nombre_vacuna)

Ejemplo: https://doors-of-drums.github.io/Pagina-web/[archivos json]
Devolvería el JSON:
    {
        "curp": "GOGL901201HDFNMS04",
        "vacunas": [
            {
                "fecha_aplicacion": "14/01/2022 13:34",
                "nombre_vacuna": "Pfizer"
            },
            {
                "fecha_aplicacion": "14/02/2022 17:34",
                "nombre_vacuna": "Pfizer refuerzo"
            }
        ]
    }


ENDPOINT:
Ver datos de la partida (?)
https://doors-of-drums.github.io/Pagina-web/[archivos json]

Verbo: GET
Parámetro de entrada esperado: username (?)

Salida: JSON con las estadísticas personales del jugador:
    [datos]
    
    CURP (CURP de la persona)
    fecha_de_aplicacion (La fecha de aplicación recibida)
    nombre_vacuna (El nombre de la vacuna recibida)

Ejemplo: https://doors-of-drums.github.io/Pagina-web/[archivos json]
Devolvería el JSON:
    {
        "curp": "GOGL901201HDFNMS04",
        "fecha_aplicacion": "14/01/2022 13:34",
        "nombre_vacuna": "Pfizer"
    }