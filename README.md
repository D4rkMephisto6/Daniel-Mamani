# PharmaSoft Backend

Spring Boot REST API for the PharmaMobil course project.

## Local setup

Requirements: Java 21 and Docker Desktop with its Linux engine running.

1. Copy `.env.example` to `.env` and replace all placeholder values. Do not commit `.env`.
2. Set `JWT_SECRET` to a Base64-encoded key containing at least 32 random bytes.
3. Start Oracle with `docker compose up -d`.
4. Start the API with `mvnw.cmd spring-boot:run` from PowerShell.

The development profile connects to Oracle at `localhost:1522/FREEPDB1` and serves the API at port `8080`. The Android emulator reaches the host API at `http://10.0.2.2:8080/api/v1/`.

Database and JWT credentials are read from the local environment. The repository intentionally contains only placeholders, not working secrets.
