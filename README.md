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
4. Run the project:
5. Application will start on port **8081** by default.  
6. Base API URL: `http://localhost:8081/movies`

---

## APIs List

| HTTP Method | Endpoint          | Description              |
|-------------|-------------------|--------------------------|
| GET         | /movies           | List all movies          |
| GET         | /movies/{id}      | Get a movie by ID        |
| POST        | /movies           | Create a new movie       |
| PUT         | /movies/{id}      | Update an existing movie |
| DELETE      | /movies/{id}      | Delete a movie by ID     |

---

## How to Test APIs in Postman

1. Open Postman.  
2. Create a new request for each endpoint:  

- **List all movies**  
  Method: `GET`  
  URL: `http://localhost:8081/movies`  

- **Create a new movie**  
  Method: `POST`  
  URL: `http://localhost:8081/movies`  
  Body (raw, JSON):  
  ```
  {
    "title": "Inception",
    "director": "Christopher Nolan",
    "releaseYear": 2010,
    "genre": "Sci-Fi",
    "rating": 9
  }
  ```  

- **Get movie by ID**  
  Method: `GET`  
  URL: `http://localhost:8081/movies/{id}` (replace `{id}`)  

- **Update movie by ID**  
  Method: `PUT`  
  URL: `http://localhost:8081/movies/{id}`  
  Body (raw, JSON):  
  ```
  {
    "title": "Inception Updated",
    "director": "Christopher Nolan",
    "releaseYear": 2010,
    "genre": "Sci-Fi Thriller",
    "rating": 10
  }
  ```  

- **Delete movie by ID**  
  Method: `DELETE`  
  URL: `http://localhost:8081/movies/{id}`  

3. Set the **Content-Type** header to `application/json` for POST and PUT requests.  

