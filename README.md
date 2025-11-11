# KT Gateway API

This project is a Spring Boot Kotlin application that acts as an API Gateway.

## Technologies Used

- **Language:** Kotlin 2.2.21
- **Framework:** Spring Boot 3.5.7
- **Build Tool:** Gradle 8.14.3
- **Java Version:** 21
- **Database:** Redis (for caching)
- **Containerization:** Docker

## How to Run

### Using Gradle

To run the application using Gradle, execute the following command in the root directory of the project:

```bash
./gradlew bootRun
```

The application will start on port 8080.

### Using Docker

This project includes a `docker-compose.yml` file to run the application in a containerized environment along with its dependencies.

1.  **Build the application image:**

    First, you need to build the Docker image for the application. You can do this using the Spring Boot plugin for Gradle:

    ```bash
    ./gradlew bootBuildImage --imageName=kaiqkt/kt-gateway-api:local
    ```

2.  **Start the services:**

    Once the image is built, you can start all the services defined in the `docker-compose.yml` file:

    ```bash
    docker-compose up
    ```

    This will start the API Gateway, Redis, PostgreSQL, and the Authentication API.

## API Documentation

API documentation can be found at... (To be added)
