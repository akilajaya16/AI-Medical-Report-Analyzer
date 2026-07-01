# Database Connectivity (DB Connection)

## Overview

The AI-Based Medical Report Analyzer uses **MySQL** as its relational database. Spring Boot connects to the database using Spring Data JPA, enabling secure storage and retrieval of user information, medical reports, and AI analysis results.

---

## Database Configuration

Configure the database connection in the **application.properties** file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/medical_report_db
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
```

---

## Database Tables

* Users
* Medical_Reports
* Analysis_Results
* Parameters
* Result_Values

---

## Database Connection Flow

1. User submits a request.
2. Spring Boot Controller receives the request.
3. Service Layer processes business logic.
4. Repository communicates with MySQL.
5. Database returns the requested data.
6. Response is sent back to the frontend.

---

## Benefits

* Secure Database Access
* Fast Data Retrieval
* Automatic Table Mapping using JPA
* Reduced SQL Complexity
* Scalable Database Design

---

## Expected Outcome

The application establishes a secure and reliable connection with the MySQL database, ensuring efficient storage, retrieval, and management of medical reports and AI-generated analysis results.
