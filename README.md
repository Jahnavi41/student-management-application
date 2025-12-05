# Student Management Application

A simple Spring Boot application that provides CRUD operations for managing student records.  
It uses Spring Web, Spring Data JPA, Hibernate, Lombok, and Swagger for API documentation.

---

## 🔧 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/Jahnavi41/StudentManagementApplication.git
cd StudentManagementApplication
```

### 2. Configure Database
Update `application.properties` with your database credentials.

Example (PostgreSQL):
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/student_db
spring.datasource.username=postgres
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 3. Build and Run the Application
```bash
mvn spring-boot:run
```

Application starts at:
```
http://localhost:8080
```

---

## 📚 API Documentation (Swagger)

Full API details, request/response formats, and schema documentation are available at:

```
http://localhost:8080/swagger-ui/index.html
```

Raw OpenAPI spec:
```
http://localhost:8080/v3/api-docs
```

---

## 📌 API Endpoints

Base URL:
```
/api/students
```

### Student Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/students` | Create a new student |
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get a student by ID |
| PUT | `/api/students/{id}` | Update a student by ID |
| DELETE | `/api/students/{id}` | Delete a student by ID |

---

## ▶️ How to Use

1. Start the application.  
2. Open Swagger UI.  
3. Use the endpoints to create, fetch, update, and delete student records.  
4. Swagger handles all examples and payload structures.

---

## ✔ Requirements

- Java 17+  
- Maven  
- PostgreSQL/MySQL (or any JPA-supported database)
