# REST API Server

REST API service built with **Java 17** and **Spring Boot 3.4**.

## Repository

**GitHub:** [SacchettaDev/REST-API-Server](https://github.com/SacchettaDev/REST-API-Server)

## Requirements

- **JDK 17+**
- **Maven 3.9+** (or Eclipse with M2E)

### Eclipse

**File → Import → Maven → Existing Maven Projects** → select the project directory → **Finish**. Run with **Run As → Spring Boot App** (Spring Tools) or **Run As → Java Application** on `RestApiServerApplication`.

## Running locally

```bash
mvn spring-boot:run
```

### Health check

```bash
curl http://localhost:8080/api/health
```

Expected JSON response: `{"status":"UP","service":"rest-api-server"}`.

## Tests

```bash
mvn test
```

## License

See repository settings or add a `LICENSE` file when applicable.
