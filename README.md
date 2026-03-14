# 🛍️ Shopping Mall Management System


### 📌 Project Description

The Shopping Mall Management System is a Java-based backend application designed to manage and maintain shopping mall details using a relational database.
This system supports CRUD operations (Create, Read, Update, Delete) and allows efficient handling of mall-related data through REST APIs.

The application uses Java for backend logic, MySQL for data storage, and Postman for testing and interacting with the APIs.
---

This project focuses on:
- Backend development using Spring Boot  
- REST API implementation  
- Database operations using JPA / Hibernate  

---

## 🚀 Features

- ✅ RESTful APIs using Spring Boot  
- ✅ Create, Read, Update, Delete (CRUD) operations  
- ✅ MySQL database integration  
- ✅ Spring Data JPA & Hibernate ORM  
- ✅ Layered architecture (Controller, Service, Repository)  
- ✅ Tested using Postman  
- ✅ Easy to extend and scale  

---

## 🧰 Technologies Used

| Category | Technology |
|----------|------------|
| Language | Java |
| Framework | Spring Boot |
| Database | MySQL |
| ORM | Spring Data JPA / Hibernate |
| Build Tool | Maven |
| Tools | Postman |
| Server | Embedded Tomcat |

---
### Project Structure
```css
Shopping-Mall-Management-System
│
├── src/main/java
│   ├── controller
│   ├── service
│   ├── repository
│   └── model
│
├── src/main/resources
│   └── application.properties
│
└── pom.xml

```

## 📌 Prerequisites

Before running this project, make sure you have:

- Java JDK 8 or higher  
- Maven installed  
- MySQL Server running  
- Postman (for API testing)  
- IDE (Eclipse / Spring Tool Suite)

  ## 🛠️ Setup & Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/SharathKasthala/Shopping-Mall-Management-System.git
cd Shopping-Mall-Management-System
```
### 2️⃣ Create MySQL Database

Login to MySQL and create the database:
```sql
CREATE DATABASE mall_db;
```
###3️⃣ Configure Database in application.properties

Edit the file src/main/resources/application.properties:

```bash
server.port=8080
spring.jpa.hibernate.ddl-auto=update
spring.datasource.url=jdbc:mysql://localhost:3306/customerdb
spring.datasource.username=root
spring.datasource.password=root
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.show-sql=true
```
###4️⃣ Run the Application

Using Maven:
```
mvn spring-boot:run
```

Or run the main class directly from your IDE:
```
ShoppingMallManagementSystemApplication.java
```

The server will start on:
```
http://localhost:8080
```

###🧪 Testing with Postman

Open Postman

Select request method (GET / POST / PUT / DELETE)

Enter the API URL (example: http://localhost:8080/malls)

Send and receive data in JSON format
```
Sample Request Body (POST)
{
  "name": "City Center Mall",
  "location": "Hyderabad",
  "manager": "John Doe"
}
```
💾 Database Table Example
```sql
CREATE TABLE mall (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    location VARCHAR(150),
    manager VARCHAR(100)
);
```
---
📈 Future Enhancements

- Implement authentication using Spring Security & JWT

- Migrate to Microservices architecture

- Integrate frontend using React / Angular

- Add pagination, sorting, and filtering

- Dockerize the application

- Deploy to cloud platforms (AWS / Azure / GCP)



###📝 Author       
 DendiHarshikReddy 
 📧 Email:harshikdendi2003@gmail.com    
 🔗 GitHub: https://github.com/HarshikReddyDendi
 

⭐ If you find this project helpful, consider giving it a star!


---
