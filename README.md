# Student Record System

A menu-driven C/C++ application for managing student records, including student details, grades, attendance, searching, filtering, validation, and persistent storage.

## Project Information

- **Project:** Student Record System
- **Team:** H-11
- **Technology:** C / C++
- **Project Phase:** Phase 1 – Requirements and Design

## Problem Statement

A record-keeping system for student details such as grades and attendance.

The system is designed to maintain student information in an organized manner and allow authorized users to add, view, search, update, and delete student records.

## Proposed Solution

The Student Record System is a menu-driven C/C++ application that provides:

- Student record management
- Grade management
- Attendance management
- Student search and filtering
- Input validation
- Persistent storage
- Authentication and role-based access
- Error handling
- Backup and recovery support

## User Roles

The system supports three types of users:

### Administrator
- Add student records
- View student records
- Search student records
- Update student information
- Delete student records
- Filter student records
- Exit the system

### Faculty
- View student records
- Search student records
- Record grades
- Update grades
- View grades
- Record attendance
- Update attendance
- View attendance
- Filter student records
- Exit the system

### Student
- View own profile
- View own grades
- View own attendance
- Exit the system

## Main Data Maintained

The system maintains:

- Student ID
- Student Name
- Contact Details
- Course / Department
- Semester
- Subject / Marks / Grades
- Attendance

## Key Features

### Authentication
Users log in using their credentials and are provided access according to their role.

### Student Management
Administrators can add, view, update, search, and delete student records.

### Grade Management
Faculty members can record, update, and view student grades.

### Attendance Management
Faculty members can record, update, and view student attendance.

### Search and Filtering
Student records can be searched using Student ID or name and filtered using course, department, or semester.

### Input Validation
The system validates required fields, Student IDs, marks, attendance values, and other user inputs before saving data.

### Persistent Storage
Student records are stored using a persistent storage mechanism such as text, CSV, binary files, or a permitted local database.

### Role-Based Access
Access to student information and operations is restricted according to the authenticated user's role.

## Architecture

The system follows a **Layered Architecture** consisting of:

1. Presentation Layer
2. Application Layer
3. Validation Layer
4. Data Layer

The architecture is divided into modular components such as:

- Authentication
- Student Management
- Academic Records
- Attendance
- Search and Reports
- Validation
- Backup
- Data Model
- Data Storage

## Project Documentation

The repository contains the following documentation:

- **Software Requirements Specification (SRS)**
- **Software Architecture & Design Specification**
- **Software Test Plan**
- **Test Case Related Update for Test Plan**

The SRS contains the functional, non-functional and technical requirements, security requirements, traceability information and use-case-related documentation. :contentReference[oaicite:1]{index=1}

The Architecture & Design Specification documents the layered architecture, component diagram, requirements traceability, security architecture, sequence diagrams, API design and error handling. :contentReference[oaicite:2]{index=2}

The Test Plan covers functional, non-functional and security testing, including authentication, student management, grades, attendance, search/filtering, validation, persistent storage and access control. :contentReference[oaicite:3]{index=3}

## Testing

Testing is organized into:

- Unit Testing (UT)
- Functional Testing (FT)
- System Testing (ST)
- Acceptance Testing (AT)
- Review-based verification (REV)

The test plan maps test cases to the requirements defined in the SRS. :contentReference[oaicite:4]{index=4}

Security validation includes:

- Authentication validation
- Role-based access control validation

## Security

The system implements security through:

- User authentication
- Role-based access control
- Input validation
- Restriction of unauthorized operations
- Data protection
- Backup and recovery support

## Requirements

The system requirements include:

- **25 Functional Requirements**
- **12 Non-Functional Requirements**
- **4 Technical Requirements**
- **2 Security Objectives**
- **2 Security Requirements**

## Project Structure

```text
Student-Record-System/
│
├── src/
│   ├── main.cpp
│   ├── auth.cpp
│   ├── student.cpp
│   ├── grades.cpp
│   ├── attendance.cpp
│   ├── search.cpp
│   ├── report.cpp
│   ├── validation.cpp
│   ├── storage.cpp
│   └── backup.cpp
│
├── include/
│   └── student.h
│
├── data/
│   └── students.dat / students.csv
│
├── docs/
│   ├── SRS.pdf
│   ├── Software Architecture & Design Specification.pdf
│   ├── Test Plan.pdf
│   └── Test Case Related Update for Test Plan.pdf
│
└── README.md
