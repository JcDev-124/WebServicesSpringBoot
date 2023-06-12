# Project Web Services with Spring Boot and JPA/Hibernate

This repository contains the source code and related resources for a Web Services project using the Spring Boot framework in Java and JPA/Hibernate for data persistence.

## Objectives

The objective of this project is to create a Web Services system using Spring Boot in Java, along with JPA/Hibernate technology for data persistence. The main objectives of the project are:

- Create a Spring Boot Java project for system development.
- Implement a complete domain model, including entities such as "User," "Order," "Product," and associations between them.
- Structure the logical layers of the application, such as resource, service, and repository, for organization and separation of responsibilities.
- Configure a test database using the H2 Database to facilitate development and testing.
- Populate the database with initial data for testing and simulations.
- Implement CRUD operations (Create, Retrieve, Update, Delete) for the entities of the system.
- Perform exception handling properly, ensuring appropriate responses and handling errors consistently.

## Project Configuration

### Dependencies

The project uses the following dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>

<dependency>
    <groupId>com.h2database</groupId>
    <artifactId>h2</artifactId>
    <scope>runtime</scope>
</dependency>

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

### Database

The test database configuration is done using the H2 Database. H2 is an in-memory database that allows temporary storage of data during development and testing.

### Logical Layers

The project should be organized into logical layers to ensure a clear separation of responsibilities:

- Resource Layer: Responsible for handling HTTP requests and providing appropriate responses. In this layer, RESTful controllers are implemented.
- Service Layer: Responsible for implementing the business logic of the application. Here, validations, calculations, and operations related to the domain are performed.
- Repository Layer: Responsible for performing data persistence and retrieval using JPA/Hibernate.

### Entities

The project should implement a complete domain model, including entities like "User," "Order," "Product," and others. The entities should be mapped using JPA/Hibernate annotations, such as `@Entity`, `@Table`, `@Id`, `@GeneratedValue`, `@ManyToOne`, `@ManyToMany`, `@OneToOne`, etc.

### CRUD Operations

The system should implement CRUD operations for the domain entities. The operations include:

- Create: Insert new records into the database.
- Retrieve: Retrieve records from the database based on search criteria.
- Update: Update existing records in the database.
- Delete: Delete records from the database.

### Exception Handling

The system should handle exceptions properly, ensuring appropriate responses to the client and consistent error handling. Custom exception classes, such as `ResourceNotFoundException` and `DatabaseException`, should be created, and an `ExceptionHandler` should be implemented to map the exceptions and provide appropriate responses in JSON format.

## Running the Project

To run the project, follow the steps below:

1. Clone this repository to your development environment.
2. Open the project in your preferred IDE.
3. Make sure you have Java 17 installed in your environment.
4. Compile and run the project using the tools available in your IDE or using the command line.
5. Use tools like Postman or Swagger to make HTTP requests and test the system's functionalities.

## Final Remarks

This project serves as a foundation for the development of web systems using Spring Boot and JPA/Hibernate. It covers various concepts and common practices in the development of

 RESTful APIs, such as layer structuring, entity mapping, exception handling, and more.

Feel free to explore and modify the project according to your needs and objectives. If you have any questions or need assistance, refer to the official documentation of Spring Boot and JPA/Hibernate or search for additional resources online.

Enjoy the learning process and have fun developing with Spring Boot and JPA/Hibernate!