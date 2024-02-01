### Coding Task: Taxi Booking and Billing System

#### Objective:
Develop a Taxi Booking and Billing System using Spring Boot, which allows users to book taxis, calculate fares, and handle billing.

#### Requirements:

1. **Entities:**
   - `User` entity with fields: `id`, `name`, `email`, `password`, `accountBalance`.
   - `Taxi` entity with fields: `id`, `driverName`, `licenseNumber`, `currentLocation`.
   - `Booking` entity with fields: `id`, `userId`, `taxiId`, `pickupLocation`, `dropoffLocation`, `fare`, `bookingTime`, `status`.

2. **User Account Management:**
   - Create endpoints for user registration, login, and updating account balance.
   - Implement JWT-based authentication for secure access.

3. **Taxi Booking:**
   - Implement endpoints to:
     - Book a taxi, providing `pickupLocation` and `dropoffLocation`.
     - View booking details.
     - Cancel a booking.
   - Implement logic to assign the nearest available taxi to a booking.

4. **Fare Calculation and Billing:**
   - Calculate the fare based on distance and a fixed rate per kilometer.
   - After the ride is complete, deduct the fare from the user's account balance.
   - Handle scenarios where the user's account balance is insufficient.

5. **Exception Handling and Validation:**
   - Implement robust exception handling for various scenarios like invalid booking requests, payment failures, etc.
   - Use Spring's validation annotations for validating user inputs.

6. **Unit Testing:**
   - Write comprehensive unit tests for the system.
   - Use Mockito for mocking dependencies and JUnit for testing.

7. **API Documentation:**
   - Document the API using Swagger or similar tools.

#### Additional Points:

- Follow RESTful principles and best practices for API development.
- Ensure proper transaction management for booking and payment operations.
- Implement appropriate logging and error reporting.

#### Deliverables:

- Source code for the Spring Boot application with all the described features.
- Unit tests demonstrating the functionality and robustness of the application.
- API documentation.
- A README file explaining how to set up and run the application, along with any necessary configuration details.

This task requires the developer to deal with a variety of challenges, including real-time data processing, secure authentication, transaction management, and integration with external services (like payment gateways). It's an excellent way to assess a developer's skills in building complex and functional applications using Spring Boot.
