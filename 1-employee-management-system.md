### Coding Task: Employee Management System

#### Objective:
Develop a simple Employee Management System using Spring Boot, which allows for adding, retrieving, and searching employees.

#### Requirements:

1. **Entities:**
   - `Employee` entity with fields: `id` (auto-generated), `name`, `email`, `department`.

2. **Controller:**
   - Create an `EmployeeController` with endpoints:
     - `POST /employees` - to add a new employee. Validate the request to ensure that `name` and `email` are not blank.
     - `GET /employees/{id}` - to retrieve an employee by id.
     - `GET /employees?department={department}` - to find employees by department.

3. **Service & Repository:**
   - Implement an `EmployeeService` and `EmployeeRepository`.
   - The repository should extend `JpaRepository` and include custom methods to find employees by department.
   - The service should handle the business logic and call repository methods.

4. **Request Validation:**
   - Use Spring's validation annotations to ensure that the employee `name` and `email` are not blank in the POST request.
   - Implement appropriate exception handling to return meaningful error messages.

5. **Unit Testing:**
   - Write unit tests for the controller and service layers.
   - Use Mockito to mock the repository in service tests.
   - Test validation constraints and exception handling in controller tests.

#### Additional Points:

- Follow good coding practices like meaningful variable names, proper indentation, and code comments.
- Ensure the application is properly configured and runs without errors.
- Implement logging where necessary.

#### Deliverables:

- Source code for the Spring Boot application.
- Unit tests covering the key functionalities.
- A brief README on how to run the application and tests.
