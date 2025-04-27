# Spring Security Demo

This project demonstrates the basics of securing a Spring Boot web application using Spring Security. It features:

- Basic user authentication
- Stateless session management (for APIs)
- H2 in-memory database integration
- H2 Console access for development

## Features

- REST endpoint: `/hello` (protected, requires authentication)
- H2 Console at `/h2-console` (open for development)
- Custom user and password set in `application.properties`
- CSRF protection disabled for API/demo convenience

## Requirements

- Java 17+
- Maven

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone <your-repo-url>
   cd spring_security_demo
   ```

2. **Run the application:**
   ```sh
   mvn spring-boot:run
   ```

3. **Access the endpoints:**

    - **REST API:**  
      Visit [http://localhost:8080/hello](http://localhost:8080/hello)  
      When prompted, use the username and password configured in `application.properties`.

    - **H2 Console:**  
      Visit [http://localhost:8080/h2-console](http://localhost:8080/h2-console)  
      Use the JDBC URL, username, and password from `application.properties`.
