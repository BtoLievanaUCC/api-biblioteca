API Biblioteca
=========================================================================================================================
01 Descripción del proyecto

API Biblioteca es una aplicación desarrollada para gestionar la información de una biblioteca. El proyecto incluye componentes para trabajar con clientes, libros y préstamos, facilitando la administración de estos recursos mediante una API.

==========================================================================================================================
02 Tecnologías utilizadas

- **Java 21:** lenguaje de programación utilizado para desarrollar la aplicación.
- **Spring Boot:** framework utilizado para construir la API.
- **Spring Web MVC:** permite crear los controladores y gestionar las solicitudes HTTP.
- **Spring Data JPA:** facilita el acceso y la gestión de los datos mediante entidades y repositorios.
- **MySQL:** sistema de gestión de bases de datos utilizado por el proyecto.
- **MySQL Connector/J:** controlador que permite la conexión entre Java y MySQL.
- **Thymeleaf:** motor de plantillas utilizado para integrar vistas HTML.
- **Maven:** herramienta utilizada para gestionar las dependencias y la construcción del proyecto.

==========================================================================================================================
03 Instalación y ejecución

Requisitos previos

- Tener instalado Java JDK 21.
- Tener instalado MySQL.
- Tener acceso a una terminal para ejecutar los comandos del proyecto.

Pasos de instalación

1. Clonar o descargar el repositorio del proyecto.
2. Crear una base de datos en MySQL llamada `libreria`.
3. Configurar la conexión a la base de datos mediante las variables de entorno correspondientes.
4. Abrir una terminal en la carpeta raíz del proyecto, donde se encuentra el archivo `pom.xml`.
5. Ejecutar la aplicación con Maven Wrapper.

En Windows, ejecutar:

mvnw.cmd spring-boot:run

### Acceso a la aplicación

La aplicación se ejecuta en el puerto 1500 por defecto.

URL local:

`http://localhost:1500`

==========================================================================================================================
04 Listado de endpoints

### Clientes

- GET /api/clientes - Obtener todos los clientes.
- GET /api/clientes/{id} - Obtener un cliente por su ID.
- POST /api/clientes - Registrar un nuevo cliente.
- DELETE /api/clientes/{id} - Eliminar un cliente por su ID.

### Libros

- GET /api/libros - Obtener todos los libros.
- GET /api/libros/{isbn} - Obtener un libro por su ISBN.
- POST /api/libros - Registrar un nuevo libro.
- PUT /api/libros/{isbn} - Actualizar un libro existente.
- DELETE /api/libros/{isbn} - Eliminar un libro por su ISBN.

### Préstamos

- GET /api/prestamos - Obtener todos los préstamos.
- GET /api/prestamos/{id} - Obtener un préstamo por su ID.
- POST /api/prestamos - Registrar un nuevo préstamo.
- DELETE /api/prestamos/{id} - Eliminar un préstamo por su ID.

### Vistas web

- GET / - Mostrar la vista principal.
- GET /vista/libros - Mostrar la administración de libros.
- POST /vista/libros/guardar - Registrar un libro.
- POST /vista/libros/{isbn}/actualizar - Actualizar un libro.
- POST /vista/libros/{isbn}/eliminar - Eliminar un libro.
- GET /vista/clientes - Mostrar la administración de clientes.
- POST /vista/clientes/guardar - Registrar un cliente.
- GET /vista/clientes/editar/{id} - Cargar un cliente para editarlo.
- GET /vista/clientes/eliminar/{id} - Eliminar un cliente.
- GET /vista/prestamos - Mostrar la administración de préstamos.
- POST /vista/prestamos/guardar - Registrar un préstamo.
- GET /vista/prestamos/eliminar/{id} - Eliminar un préstamo.



