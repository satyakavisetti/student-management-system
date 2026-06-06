# Student Information and Result Management System

A web-based Student Information and Result Management System developed using PHP, MySQL, HTML, and CSS. This project allows users to securely manage student records, calculate results automatically, and view student result memos.

## Project Objective

The main objective of this project is to develop a web-based system that helps manage student information, store academic records, and generate results automatically.

## Features

* Secure Login System
* Add Student Details
* Store Student Records in MySQL Database
* Automatic Total Calculation
* Automatic Grade Calculation
* PASS / FAIL Result Generation
* Student Result Search by Roll Number
* Attractive Result Memo Display
* College Logo Integration
* Logout Functionality

## Requirements

Before running the project, install:

- XAMPP
- PHP
- MySQL
- Web Browser
- Code Editor (VS Code)

##  Technologies Used

### Frontend

* HTML
* CSS

### Backend

* PHP

### Database

* MySQL

### Server

* XAMPP Apache Server

### Database Management Tool

* phpMyAdmin

---

##  Project Structure

student_system/

├── login.html

├── login.php

├── logout.php

├── index.html

├── add_student.php

├── result.php

├── logo.png

└── README.md

---

## 🗄 Database Setup

### Create Database

```sql
CREATE DATABASE student_db;
```

### Use Database

```sql
USE student_db;
```

### Create Students Table

```sql
CREATE TABLE students (
roll VARCHAR(20) PRIMARY KEY,
name VARCHAR(50),
course1 VARCHAR(50),
marks1 INT,
course2 VARCHAR(50),
marks2 INT,
course3 VARCHAR(50),
marks3 INT,
total INT,
result VARCHAR(10),
grade VARCHAR(5)
);
```

### Create Users Table

```sql
CREATE TABLE users (
id INT AUTO_INCREMENT PRIMARY KEY,
username VARCHAR(50),
password VARCHAR(50)
);
```

### Insert Login User

```sql
INSERT INTO users(username,password)
VALUES('admin','admin123');
```

---

## 🚀 How to Run the Project

### Step 1

Install XAMPP.

### Step 2

Start:

* Apache
* MySQL

### Step 3

Copy the project folder into:

```text
C:\xampp\htdocs\
```

### Step 4

Open phpMyAdmin:

```text
http://localhost/phpmyadmin
```

### Step 5

Create the database and tables using the SQL commands provided above.

### Step 6

Run the application:

```text
http://localhost/student_system/login.html
```

---

## 🔐 Login Credentials

Username:

```text
admin
```

Password:

```text
admin123
```

---

## 📊 Result Calculation Logic

### PASS Condition

A student is declared PASS if all subject marks are greater than or equal to 35.

### FAIL Condition

A student is declared FAIL if any subject mark is below 35.

### Grade Calculation

| Percentage | Grade |
| ---------- | ----- |
| 90+        | A+    |
| 75-89      | A     |
| 60-74      | B     |
| 50-59      | C     |
| 35-49      | D     |
| Below 35   | F     |

---

##  Project Workflow

1. User logs into the system.
2. User enters student details and marks.
3. System calculates total, percentage, grade, and result.
4. Data is stored in MySQL database.
5. User can search results using roll number.
6. Result memo is displayed with complete details.

---

##  Sample Modules

* Login Page
* Add Student Page
* Result Search Page
* Student Result Memo Page

