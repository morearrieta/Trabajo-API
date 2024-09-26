# Trabajo-API- Persona
Este proyecto es una aplicación Spring Boot que gestiona personas con su domicilio y localidad utilizando una arquitectura basada en repositorios, servicios y controladores.
Permite gestionar informacion utilizando jpa para la interaccion con la base de datos h2.
Se utiliza:
-Java 17
-Spring Boot: Marco principal para crear la aplicacion.
-Spring Data JPA: Gsetion de Base de Datos.
-H2 Database: Base de datos en memoria para pruebas.
-Gradle: gestion de dependencias. 

Estructura

entities
Aquí es donde se definen las entidades de la base de datos. En este caso, la entidad Persona, Domicilio y Localidad representan tablas en la base de datos.

repositories
La interfaz PersonaRepository, LocalidadRepository, DomiilioRepository extienden a JpaRepository, proporcionando métodos CRUD para la entidad Persona, Localidad y Domicilio.

services
La capa de servicios contiene la lógica de negocio. PersonaService interactúa con PersonaRepository para obtener, guardar y manipular datos. Y lo mismo con DomicilioService y LocalidadService.

controllers
PersonaController, LocalidadController y DomicilioController expone la API REST y maneja las solicitudes HTTP.

