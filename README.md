# Passenger Service API 

Passenger service is a RestFul API using Java Spring Boot and JPA & Hibernate to build my embedded SQL database (H2)

## Installation

- Clone the project using the command:

```bash
git clone
```
## Project requirement 
- IntelliJ IDEA IDE
- Java 11 JDK 
- Maven
- Postman for testing purposes (Optional)

## Run
- Install all the project dependencies

- Type this command in the terminal:
```bash
mvn clean install
```
- Start the application by pressing run in IntelliJ IDEA or by typing this command in the terminal after you enter the project folder:
```bash
java -jar target/passengerdata-0.0.1-SNAPSHOT.jar
```
- The database has already initialized data so that you can test the application immediately. 
- _The database will be dropped and get created each time you run the application as it is **embedded SQL database (H2)**._

## API Documentation

This App allows you to preform CRUD operations for the passenger and search for passenger by ID


## Documents

| Files  | Type |
| ------------- |:-------------:|
| _id      | Unique id for the passenger (Long)     |
| firstName      | String     |
| lastName      | String     |
| passportId      | long     |
| email      | String     |

## Routes

 1. Route URL: ```http://localhost:8080/passengers``` on this route you can preform GET and POST request, so you can (GET) all passengers in the database , add new (POST) passengers and (DELETE) all passengers.
 
 ```
 [
    {
        "id": 1,
        "firstName": "Abdullah",
        "lastName": "Alrez",
        "passportID": 33231237,
        "email": "abdullah@gmail.com"
    },
  .
  .
  .
  .
]
```
 
 2. Route URL: ```http://localhost:8080/passengers/{id}``` on this route you preform GET,DELETE and PUT request (Retrieve), so you can delete, update and get the passengers by its id.
 
 