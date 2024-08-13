# Estructura del Proyecto



## .env.template
Plantilla para el archivo de configuración de variables de entorno.



## controllers/

### controllers/auth.js
To generate an h2 heading in markdown, you can use the following syntax:



This will create a second-level heading in your markdown document.
Este archivo contiene los controladores relacionados con la autenticación de usuarios. Las funciones principales son:

- `crearUsuario`: Crea un nuevo usuario en la base de datos.
- `loginUsuario`: Autentica a un usuario existente y genera un token JWT.
- `revalidarToken`: Revalida el token JWT de un usuario autenticado.

### controllers/events.js
Este archivo contiene los controladores relacionados con la gestión de eventos. Las funciones principales son:

- `getEventos`: Obtiene todos los eventos de la base de datos.
- `crearEvento`: Crea un nuevo evento en la base de datos.
- `actualizarEvento`: Actualiza un evento existente en la base de datos.
- `eliminarEvento`: Elimina un evento de la base de datos.

## database/
Contiene la configuración de la base de datos.

- **config.js**: Archivo de configuración para la conexión a la base de datos.

## helpers/isDate.js
Este archivo contiene una función para validar si una fecha es válida utilizando la librería moment.

### Funciones principales:

- `isDate(value):` Verifica si el valor proporcionado es una fecha válida. Retorna true si la fecha es válida, de lo contrario, retorna false.
- `helpers/jwt.js:` Este archivo contiene funciones para la generación y verificación de JSON Web Tokens (JWT) utilizando la librería jsonwebtoken.

### Funciones principales:
- `generarJWT(uid, name):` Genera un token JWT con el uid y name proporcionados. Retorna una promesa que resuelve con el token generado o rechaza con un error si no se pudo generar el token.

## middlewares/
Contiene middlewares que son utilizados para validar y procesar las solicitudes.

- **validar-campos.js**: Middleware para validar los campos de las solicitudes.
- **validar-jwt.js**: Middleware para validar el JSON Web Token (JWT).

## models/
Contiene los modelos de datos que representan las entidades en la base de datos.

- **Evento.js**: Modelo para los eventos.
- **Usuario.js**: Modelo para los usuarios.

## public/
Contiene archivos estáticos que son servidos al cliente.

- **.DS_Store**: Archivo de sistema (puede ser ignorado).
- **assets/**: Carpeta que contiene los archivos de recursos como CSS y JavaScript.
  - **index-6i0AJy9o.css**: Archivo CSS para el estilo de la aplicación.
  - **index-BtGEsYMc.js**: Archivo JavaScript para la funcionalidad de la aplicación.
- **index.html**: Archivo HTML principal que se sirve al cliente.

## routes/
Contiene las definiciones de las rutas de la API.

- **auth.js**: Define las rutas para la autenticación de usuarios (`/api/auth`).
- **events.js**: Define las rutas para la gestión de eventos (`/api/events`).

## index.js
Archivo principal del servidor. Configura y arranca el servidor de Express, define las rutas y la conexión a la base de datos.

## package.json
Archivo de configuración de npm que contiene las dependencias y scripts del proyecto.