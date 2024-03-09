# Spring Boot CRUD Operations with Student Entity

This project implements CRUD (Create, Read, Update, Delete) operations on a Student entity using Spring Boot and exposes these functionalities through REST APIs. 

## Prerequisites
- Java Development Kit (JDK) installed
- Maven installed
- Postman (optional, for testing APIs)
- cURL (optional, for command-line testing)

## REST API Endpoints

1. **Save Student**  
   - HTTP Method: POST
   - Endpoint: `http://localhost:8080/student`
   - Request Body Example: 
     ```json
     {
       "name": "rishabh",
       "email": "rishabh@gmail.com"
     }
     ```

2. **Get Student by Id**  
   - HTTP Method: GET
   - Endpoint: `http://localhost:8080/student/{id}`
   - Example: `http://localhost:8080/student/2`

3. **Get All Students**  
   - HTTP Method: GET
   - Endpoint: `http://localhost:8080/student`

4. **Update a Student**  
   - HTTP Method: PUT
   - Endpoint: `http://localhost:8080/student/{id}`
   - Request Body Example: 
     ```json
     {
       "id": 25,
       "name": "rishabh",
       "email": "rishabh@gmail.com"
     }
     ```

5. **Delete a Student**  
   - HTTP Method: DELETE
   - Endpoint: `http://localhost:8080/student/{id}`
   - Example: `http://localhost:8080/student/25`

## Command Prompt and cURL Syntax

1. **Save Student**
   ```bash
   curl -X POST -H "Content-Type: application/json" -d "{\"name\":\"rishabh\",\"email\":\"rishabh@gmail.com\"}" http://localhost:8080/student
   ```

2. **Get Student by Id**
   ```bash
   curl http://localhost:8080/student/{id}
   ```

3. **Get All Students**
   ```bash
   curl http://localhost:8080/student
   ```

4. **Update a Student**
   ```bash
   curl -X PUT -H "Content-Type: application/json" -d "{\"id\":23,\"name\":\"kajal\",\"email\":\"kajal@gmail.com\"}" http://localhost:8080/student/25 -v
   ```

5. **Delete a Student**
   ```bash
   curl -X DELETE http://localhost:8080/student/25
   ```

## Notes
- cURL is a versatile command-line tool for making HTTP requests.
- Postman is an alternative tool for testing REST APIs with a graphical user interface.

## Authors
- [Rishabh Pathak]

## License
This project is licensed under the [springbootcrud] License - see the [LICENSE.md](LICENSE.md) file for details.
