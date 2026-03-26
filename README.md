# REST API Server (Java)

REST API built with **Java 17** and **Spring Boot 3.4**. The project is meant to grow in **small steps** with **frequent commits** on GitHub.

## Requirements

- **JDK 17+**
- **Maven 3.9+** (or let Eclipse manage dependencies via M2E)

### Eclipse

**File → Import → Maven → Existing Maven Projects** → select the `Rest-Api-Server` folder → Finish. Then **Run As → Spring Boot App** (with Spring Tools installed) or **Run As → Java Application** on `RestApiServerApplication`.

## Run locally

```bash
mvn spring-boot:run
```

Try it:

```bash
curl http://localhost:8080/api/health
```

Expected response: `{"status":"UP","service":"rest-api-server"}`.

## Tests

```bash
mvn test
```

## Next steps (ideas for small commits)

1. `feat:` Dedicated response DTO for `/api/health` (instead of `Map`).
2. `feat:` Sample in-memory CRUD endpoint (e.g. `Item` resource).
3. `feat:` Validation with Bean Validation (`jakarta.validation`).
4. `feat:` Global error handling (`@ControllerAdvice`).
5. `chore:` `dev` / `prod` profiles in `application-*.properties`.
6. `feat:` Persistence (Spring Data JPA + H2 or PostgreSQL).

Each item can be **one commit** (or several — even better for history).

## License

To be defined (e.g. MIT).
