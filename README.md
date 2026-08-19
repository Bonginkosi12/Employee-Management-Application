# Employee-Management-Microservices
## project overview for Employee-Management Application
##### Project Status
This project is actively under development. More services and features will be added as development continues.

Employee Management Microservices is a backend application built using a microservices architecture. The system is divided into independent services responsible for different areas of employee management.
Each service has its own responsibility and database, while RabbitMQ is used for asynchronous communication between services.

## Employee Management Microservices
### Structure:
1. Employee Service - Manages employee information and employee-related operations.
   Repository: https://github.com/Bonginkosi12/Employee-Service.git

2. Salary Service - Manages employee salary information, allowing us to create salary records
   Repository: https://github.com/Bonginkosi12/Salary-service.git

3. Leave Service - Manages leave for employees, allowing employees to request for leave.
   Repository: https://github.com/Bonginkosi12/Leave-service.git

5. Performance Service - Manages employee performance and performance-related information.
   Repository: In progress

6. Attendance Service - Manages employee attendance records and attendance-related information.
   Repository: In progress

### Architecture:
Employee-Service(Producer)
        |
        |
EmployeeCreatedEvent(Message)
        |
        |
    RabbitMQ(RabbitMQ enables services to communicate through events without requiring direct synchronous communication between every service)
        |
        |
    Consumers
    Salary-Service\ leave-Service \ Performance-Service \ Attendance-Service
    

### Key Concepts Demonstrated
Microservices Architecture
RESTful API Development
CRUD Operations
Database-per-Service Architecture
Event-Driven Architecture
Asynchronous Messaging
RabbitMQ Producers and Consumers
Spring Data JPA
PostgreSQL Database Integration
Docker

### Technology stack
Backend:
- Java
- Spring Boot
- REST APIs
- Spring Data JPA
- Hibernate

Database:
- PostgreSQL

Messaging:
- RabbitMQ

Development & Testing:
- IntelliJ IDEA
- Postman

