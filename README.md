# Practica Integradora 4 - Curso Backend NodeJS Modulo 3

¿Cómo abordar la tercera práctica integradora?

Primero toca dar un vistazo a lo que se tiene.

* Sistema de usuarios con roles "student" y "teacher".
* Sistema de cursos
* Modelo de registro y login (realizado con passport + jwt)
* Todo el servidor se encuentra con una arquitectura más sólida en comparación con el modelo previo.
* Manejo de passport para poder mantener un middleware "current" que nos permita obtener la información del usuario guardado en la cookie.
* Servicio de mailing para enviar correo cada vez que el usuario se registra a algún curso

La implementación de la última práctica integradora es bastante simple, debido a que sólo es necesario marcar los últimos detalles y dudas.

* Documentación: Crear el swagger de documención para las Apis de Users (Estudiantes) y     Cursos. (Al menos 1 de estas apis).
* Logger: Agregar logging a todas las apis de estudiantes y cursos, donde se muestre el metodo llamado y la URL invocada. Además colocar un log del status recibido. 
* Testing: 
    - Crear el super test para el api de usuarios o de cursos.
    - Crear test unitarios para los Daos de estudiantes o cursos.

## Preparacion del ambiente

Se crea un archivo config.js en la carpeta config, éste alojará todas las variables de entorno. Además, se colocará dotenv para poder cargar el archivo .env

* Modificar el archivo de configuración para cargar mis propias variables de entorno según corresponda.
* Debe existir como mínimo la URL para conectarme a mi BD de MongoDB (local o en la nube) 
* Crear archivos de ambiente para desarrollo y producción donde, desarrollo le debe apuntar a la BD en local y prod a la BD de mongo atlas.


* NUEVOS IMPORTS:
- winston
- swagger-jsdoc
- swagger-ui-express
- chai: en modo development
- mocha: en modo development