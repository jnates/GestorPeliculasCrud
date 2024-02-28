# GestorPeliculasCrud

## Descripción
GestorPeliculasCrud es una aplicación web desarrollada en Spring Boot que proporciona operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para gestionar películas.

## Funcionalidades
- Crear nuevas películas con información como nombre, género, y fecha de estreno.
- Leer información detallada de una película específica.
- Actualizar la información de una película existente.
- Eliminar una película de la base de datos.

## Tecnologías Utilizadas
- Java
- Spring Boot
- Thymeleaf
- Hibernate
- H2 Database (base de datos en memoria)

## Configuración y Uso
1. Clona este repositorio en tu máquina local.
2. Abre el proyecto en tu IDE favorito (como IntelliJ IDEA, Eclipse, etc.).
3. Asegúrate de tener instalado Java y Maven en tu sistema.
4. Configura las dependencias y las propiedades de la aplicación según sea necesario.
5. Ejecuta la aplicación desde tu IDE o utilizando el comando `mvn spring-boot:run` en la terminal.
6. Abre un navegador web y accede a `http://localhost:8080` para utilizar la aplicación.

## Endpoints

### Crear una nueva película
- **URL:** `/peliculas`
- **Método:** `POST`
- **Parámetros de la solicitud:**
  - `nombre`: Nombre de la película (cadena de texto).
  - `generoId`: ID del género de la película (entero).
  - `fechaEstreno`: Fecha de estreno de la película (formato: YYYY-MM-DD).
- **Descripción:** Crea una nueva película con la información proporcionada.
- **Ejemplo de solicitud:**
  ```http
  POST /peliculas HTTP/1.1
  Host: localhost:8080
  Content-Type: application/json

  {
    "nombre": "Pelicula de ejemplo",
    "generoId": 1,
    "fechaEstreno": "2024-02-28"
  }


## Contribución
¡Las contribuciones son bienvenidas! Si encuentras algún problema o tienes alguna sugerencia de mejora, por favor abre un issue o envía un pull request.

## Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para obtener más detalles.

