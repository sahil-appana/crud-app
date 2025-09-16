# CRUD App (Spring Boot)

A simple **CRUD (Create, Read, Update, Delete)** application built with **Spring Boot**, **Spring Data JPA**, and **H2 Database**.

---

## 🚀 Features
- RESTful APIs for managing users
- In-memory H2 database (auto-configured)
- JPA + Hibernate for persistence
- Lombok for cleaner code

---

## 📂 Project Structure
```
crud-app/
 ├── src/main/java/com/example/crudapp/
 │   ├── CrudAppApplication.java        # Main class
 │   ├── controller/UserController.java # REST Controller
 │   ├── model/User.java                # Entity
 │   └── repository/UserRepository.java # Repository
 ├── src/main/resources/
 │   └── application.properties         # Config (H2 DB)
 ├── pom.xml                            # Maven dependencies
```

---

## ⚡ Run the Application

### Prerequisites
- Install **Java 17+**
- Install **Maven**

### Run
```bash
mvn spring-boot:run
```

The app will start at:  
👉 `http://localhost:8080`

---

## 📌 API Endpoints

| Method | Endpoint            | Description        |
|--------|---------------------|--------------------|
| GET    | `/api/users`        | Get all users      |
| GET    | `/api/users/{id}`   | Get user by ID     |
| POST   | `/api/users`        | Create new user    |
| PUT    | `/api/users/{id}`   | Update user by ID  |
| DELETE | `/api/users/{id}`   | Delete user by ID  |

---

## 🛠 Example Request
Create a new user:
```bash
curl -X POST http://localhost:8080/api/users \
     -H "Content-Type: application/json" \
     -d '{"name":"Satya","email":"satya@example.com"}'
```

---

## 🧑 Author
- **Appana Satya Sahil**


---

## 🧪 Postman Collection
You can import the file **`crud-app.postman_collection.json`** into Postman to test all APIs directly.
