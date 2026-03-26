# REST API Server (Java)

API REST em **Java 17** com **Spring Boot 3.4**. Projeto pensado para evoluir em **passos pequenos** e com **muitos commits** no GitHub.

## Requisitos

- JDK **17+**
- **Maven** 3.9+ (ou deixar o Eclipse gerir dependências via M2E)

### Eclipse

**File → Import → Maven → Existing Maven Projects** → pasta `Rest-Api-Server` → Finish. Depois **Run As → Spring Boot App** (com Spring Tools instalado) ou **Run As → Java Application** em `RestApiServerApplication`.

## Correr localmente

```bash
mvn spring-boot:run
```

Testar:

```bash
curl http://localhost:8080/api/health
```

Resposta esperada: `{"status":"UP","service":"rest-api-server"}`.

## Testes

```bash
mvn test
```

## Próximos passos (ideias para commits pequenos)

1. `feat:` DTO de resposta dedicado para `/api/health` (em vez de `Map`).
2. `feat:` Endpoint de exemplo CRUD (ex.: recurso `Item` em memória).
3. `feat:` Validação com Bean Validation (`jakarta.validation`).
4. `feat:` Tratamento global de erros (`@ControllerAdvice`).
5. `chore:` Perfil `dev` / `prod` em `application-*.properties`.
6. `feat:` Persistência (Spring Data JPA + H2 ou PostgreSQL).

Cada item pode ser **1 commit** (ou vários, ainda melhor para o histórico).

## Licença

Definir quando quiseres (ex.: MIT).
