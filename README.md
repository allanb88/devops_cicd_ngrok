# Billing Application: Spring Boot and Angular

A learning project that brings together a Spring Boot billing API and an Angular frontend. The repository also contains Firebase configuration and container build files for the web application.

## Components

- `billing/`: Spring Boot invoice and billing API, with Maven profiles and Swagger UI.
- `angularWorkSpace/`: Angular workspace containing the billing user interface.
- Dockerfiles and Firebase configuration are included with the relevant application components.

## Requirements

- Java 17 or later and the Maven Wrapper for the API
- Node.js and npm for the Angular workspace
- Angular CLI 10.0.7 for the frontend tooling

## Start the API

```bash
cd billing
./mvnw spring-boot:run -Plocal
```

The API example documents Swagger UI at `http://localhost:7080/swagger-ui/index.html`; confirm the actual port in the application startup log.

## Start the frontend

```bash
cd angularWorkSpace
npm install
npx ng serve
```

Open <http://localhost:4200>. Configure the frontend's API endpoint to match the locally running billing service.

Review Firebase and environment configuration before deploying. Keep credentials and private keys out of source control.
