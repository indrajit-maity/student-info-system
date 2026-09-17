# 🎓 Student Information System

A full-stack **Student Information System** designed to manage student records, departments, courses, and academic information through a structured web application.

## 👨‍💻 Author

**Indrajit Maity**

---

## 🚀 Features

- Student registration and management
- Add, update, view, and delete student records
- Department management
- Course management
- Student enrollment management
- RESTful API integration
- Database-driven student information
- Input validation
- Exception handling
- Responsive user interface

---

## 🛠️ Tech Stack

### Backend

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- REST API

### Database

- MySQL

### Frontend

- React.js
- HTML5
- CSS3
- JavaScript

### Tools

- Git
- GitHub
- Postman
- IntelliJ IDEA
- VS Code

---

## 🏗️ Project Architecture

```text
                    Student Information System
                              │
                              ▼
                         React Frontend
                              │
                              │ HTTP / REST API
                              ▼
                       Spring Boot Backend
                              │
                ┌─────────────┼─────────────┐
                │             │             │
                ▼             ▼             ▼
           Controller      Service      Repository
                              │             │
                              └──────┬──────┘
                                     ▼
                              JPA / Hibernate
                                     │
                                     ▼
                                  MySQL


Student-Information-System/
│
├── backend/
│   │
│   ├── src/
│   │   └── main/
│   │       │
│   │       ├── java/
│   │       │   └── com/
│   │       │       └── ...
│   │       │           ├── controller/
│   │       │           ├── service/
│   │       │           ├── repository/
│   │       │           ├── entity/
│   │       │           ├── dto/
│   │       │           └── exception/
│   │       │
│   │       └── resources/
│   │           └── application.properties
│   │
│   └── pom.xml
│
├── frontend/
│   │
│   ├── src/
│   ├── public/
│   └── package.json
│
└── README.md


Create Student
      │
      ▼
View Student
      │
      ▼
Update Student
      │
      ▼
Delete Student


                    Department
                        │
                        │
                        ▼
                     Student
                        │
                        │
                        ▼
                    Enrollment
                        │
                        │
                        ▼
                      Course