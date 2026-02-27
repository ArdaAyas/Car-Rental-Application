# Car Rental Application API

A robust RESTful application built with Spring Boot for rental car management. API can be used as the backend for both mobile and web applications. 

Developed as a final project for CSC393 course, Developing Backend Applications with Spring Framework.

## Definition

### Technologies Used
* Spring Boot 3.x
* Spring Data JPA / Hibernate
* MySQL (Can be swapped for any database implementation)
* OpenAPI (Swagger)
* JUnit 5

### Key Features
-  Search: Find avaliable cars by categories,dates,transmission and location
-  Reservations: Create rental reservations, add extra equipment, cancel and delete reservations
-  Car Management: Track currently rented cars, bring cars back, manage car inventory
-  UML Diagram: Can be found at `umldiagram.png` 
-  Car Status Tracking: All cars have status types for easy tracking.(Confirmed,Completed,Cancelled,Pending)
   
## Architecture
1. 3-Layer Architecture: Separation of `Controller`, `Service` and `Repository` layers.
2. DTO Pattern: Client doesn't use @Entity classes, instead all data is handled with Data Transfer Objects (DTOs) at the controller layer.
3. Specific SQL queries are used for each feature to access data from the database.

## Configuration
* Database is created in `MySQL` by default. 
* Create a `car_rental_db` database in MySQL.
* Change the `URL`, `username` and `password` at `application.properties`.
* Swagger API documentation can be found at `http://localhost:8081/swagger-ui/index.html`


## References
This project was made in collaboration with Bora Kısalar https://github.com/borakisalar
