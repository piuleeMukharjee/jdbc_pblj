# Java JDBC Applications with MVC and CRUD Operations

## 📌 Overview

This project consists of three parts that demonstrate how to use **Java JDBC** for database connectivity and operations. It also includes an MVC-based Student Management Application.

---

## 📁 Project Structure

/JDBC-Project/
│
├── PartA_FetchEmployeeData.java # Connect to DB and fetch employee data
├── PartB_ProductCRUD.java # CRUD operations on Product table
│
├── /studentmvc/
│ ├── Student.java # Model class
│ ├── StudentDAO.java # Controller for DB operations
│ └── StudentApp.java # View: Menu-driven UI
│
└── README.md # Project documentation

yaml
Copy code

---

## 🧩 Part A: Connect to MySQL and Fetch Employee Data

### ✔️ Objective:
Connect to a MySQL database and display all records from an `Employee` table using **JDBC**.

### 🔧 Table: `Employee`
| Column   | Type     |
|----------|----------|
| EmpID    | INT      |
| Name     | VARCHAR  |
| Salary   | DOUBLE   |

### 🧪 Features:
- Establish JDBC connection
- Run `SELECT * FROM Employee`
- Display results in console

### 🚀 Run:
```bash
javac PartA_FetchEmployeeData.java
java PartA_FetchEmployeeData
🧩 Part B: CRUD Operations on Product Table Using JDBC
✔️ Objective:
Perform Create, Read, Update, Delete operations on a Product table using JDBC and transaction management.

🔧 Table: Product
Column	Type
ProductID	INT
ProductName	VARCHAR
Price	DOUBLE
Quantity	INT

🧪 Features:
Menu-driven interface

Insert, View, Update, Delete operations

Uses PreparedStatement

Transaction handling using setAutoCommit(false), commit(), and rollback()

🚀 Run:
bash
Copy code
javac PartB_ProductCRUD.java
java PartB_ProductCRUD
🧩 Part C: Student Management Application using MVC Architecture
✔️ Objective:
A Student Management System built using MVC (Model-View-Controller) pattern and JDBC.

🔧 Table: Student
Column	Type
StudentID	INT
Name	VARCHAR
Department	VARCHAR
Marks	DOUBLE

📦 MVC Components:
Model: Student.java
Defines the student attributes.

View: StudentApp.java
Provides a console menu for CRUD operations.

Controller: StudentDAO.java
Handles all JDBC logic.

🧪 Features:
Add a new student

View all students

Update student details

Delete student records

Clean separation of logic using MVC

🚀 Run:
bash
Copy code
cd studentmvc
javac Student.java StudentDAO.java StudentApp.java
java StudentApp
💡 Requirements
Java 8 or later

MySQL Server

MySQL JDBC Driver (Connector/J)

⚙️ JDBC Setup
Add MySQL Connector to Classpath

Download mysql-connector-java-x.x.xx.jar from MySQL Downloads.

Run with classpath (example):

bash
Copy code
javac -cp .;mysql-connector-java-8.0.33.jar YourFile.java
java -cp .;mysql-connector-java-8.0.33.jar YourFile
