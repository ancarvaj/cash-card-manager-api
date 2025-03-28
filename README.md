# Cash Card Manager API 

API REST para gestión de tarjetas prepago (Cash Cards), desarrollada con Spring Boot. Proyecto inspirado en el curso ["Building a REST API with Spring Boot"] de Spring Academy, con mejoras propias.

## Características

- **Gestión de Cash Cards**: CRUD completo con validaciones
- **Seguridad JWT**: Autenticación con roles (USER/ADMIN)
- **Documentación OpenAPI**: Interactiva via Swagger UI
- **Pruebas robustas**: Unitarias + de integración con Testcontainers
- **Dockerizado**: Ready para despliegue en producción

## Tecnologías

- **Backend**: Java 17, Spring Boot 3.3.10
- **Base de datos**: 
  - PostgreSQL (Producción) 
  - H2 (Testing)
- **Documentación**: OpenAPI + Swagger UI
- **Seguridad**: JWT + Spring Security
- **DevOps**:
  - Docker + Docker Compose
  - Jenkins (CI/CD)
  - SonarQube (Análisis de código)
- **Testing**: JUnit, Testcontainers

## Instalación

### Requisitos
- Java 17+
- Docker

```bash
docker-compose up -d  # Levanta PostgreSQL + aplicación en http://localhost:8080
```
## Documentación API
Accede a la UI interactiva:
http://localhost:8080/swagger-ui.html

## Testing

### Ejecutar tests
```bash
./mvnw test
```
## CI/CD

## CI/CD Pipeline
Flujo automatizado con Jenkins:
- Build y pruebas unitarias
- Análisis estático con SonarQube
- Build de imagen Docker
- Push a Docker Hub (versiones tagged)
