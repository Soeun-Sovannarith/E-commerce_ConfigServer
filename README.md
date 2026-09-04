# E-commerce Config Server

Standalone Java 22 / Spring Boot Config Server for the commerce microservices.
The server reads versioned application configuration from `config-repository/`
in this repository.

## Run

```bash
./gradlew bootRun
```

The server listens on port `8888`. Example endpoints:

- `http://localhost:8888/user-service/default`
- `http://localhost:8888/product-service/local`
- `http://localhost:8888/order-service/default`
- `http://localhost:8888/api-gateway/default`
- `http://localhost:8888/eureka-server/default`

Secrets are supplied using environment variables; they are not committed.
