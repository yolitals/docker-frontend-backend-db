# Ejercicio

    - Crear una imagen de Docker para el backend, los assets de la aplicación se encuentran en ./backend
      - La aplicación esta en node y se ejecuta de la siguiente forma:
        ```sh
        $ node server.js
        ```
    - Crear una imagen de Docker para el frontend, los assets se encuentran en la carpeta ./frontend
      - La Aplicación esta en javascript y se ejecuta de la siguiente forma:
        ```sh
        $ npm start
        ```
    - Desplegar los 3 componentes de la aplicación:
      - Frontend
      - Backend
      - Base de datos
    - Condiciones:
      - La información de la base de datos debe persistir.
      - Las comunicaciones entre los contenedores se deben limitar a lo siguiente:
        - La base de datos unicamente podra ser accedida desde el backend.
        - El frontend unicamente podra acceder al backend. 
