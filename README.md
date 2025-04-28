# 📚 Student Management System (Spring MVC + JDBC + MySQL)

A simple and structured **Student Management Web Application** built using **Spring MVC (Java Configuration)**, **JDBC Template**, and **MySQL**.

This project provides a clean CRUD system to manage students with **unique emails**, **search functionality** by **name** or **grade**, and a **responsive Bootstrap 5** interface.

---

## ✨ Features
- List all students in a responsive table
- Add a new student (name, email, grade)
- Update existing student details
- Delete a student
- Search students dynamically by name or grade
- Email uniqueness enforced at the database level
- Full separation of layers: Controller ➔ Service ➔ Repository
- Modern and clean UI using **Bootstrap 5**

---

## 🛠️ Tech Stack
- **Java 17**
- **Spring MVC 6**
- **Spring JDBC Template**
- **MySQL 8**
- **Tomcat 11**
- **JSP (Jakarta EE 10)**
- **Maven 3.8+**
- **Bootstrap 5**

---

## ⚙️ Requirements
- Java JDK 17+
- Maven 3.8+
- MySQL Server 8+
- Apache Tomcat 10+ (tested on Tomcat 11)

---

## 🚀 How to Run
1. Clone the repository
2. Create the MySQL database and table (SQL script included)
3. Configure `db.properties` (or directly in `SpringConfig.java`) with your DB credentials
4. Build the project using Maven
5. Deploy the generated WAR file on your Apache Tomcat server

---

## 📜 Database Setup
Execute the following SQL commands to create your database and table:

```sql
CREATE DATABASE yourdb;
USE yourdb;

CREATE TABLE student (
 id INT AUTO_INCREMENT PRIMARY KEY,
 name VARCHAR(100) NOT NULL,
 email VARCHAR(100) NOT NULL UNIQUE,
 grade DOUBLE NOT NULL
);


