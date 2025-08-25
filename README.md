# Movie Management API

## Overview

A simple RESTful API for managing movies, built with Spring Boot.  
Supports full CRUD operations on movies with validation, error handling, and auto-generated OpenAPI (Swagger) documentation.

---

## Tech Stack

- **Java 17**  
- **Spring Boot 3.1**  
- **Spring Web MVC** - REST API  
- **Spring Data JPA** - Database interaction  
- **H2 Database** - In-memory DB for development/testing  
- **Jakarta Bean Validation** - Input validation  
- **Maven** - Build and dependency management  

---

## How to Run the Project

### Prerequisites

- Java JDK 17 or higher  
- Maven installed

### Steps

1. Clone or download the repository.  
2. Navigate to the project root directory.  
3. Build and download dependencies:  
    -- mvn clean install
4. Run the project:
   -- mvn spring-boot:run


## How to Run the test

### test this apis on postman 

Here is the list of APIs for the Movie Management API:

| HTTP Method | Endpoint          | Description             |
|-------------|-------------------|-------------------------|
| GET         | /movies           | List all movies         |
| GET         | /movies/{id}      | Get a movie by ID       |
| POST        | /movies           | Create a new movie      |
| PUT         | /movies/{id}      | Update an existing movie|
| DELETE      | /movies/{id}      | Delete a movie by ID    |
