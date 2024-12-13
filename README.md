# School Management System

Welcome to the **School Management System** project! This application simplifies school operations with robust role management, attendance tracking, and more. Follow the instructions below to set up the project in your environment.

---

## Features

- User authentication with Admin, Teacher, Parent, and Student roles.
- Role and permission management for access control.
- Dynamic dashboards tailored to user roles.
- CRUD operations for teachers, students, classes, and subjects.
- Attendance tracking and performance monitoring.
- Responsive and user-friendly web interface.

---

## Prerequisites

Ensure the following are installed:

1. **XAMPP** (for Apache and MySQL).
2. **Composer** (PHP dependency manager).
3. **VS Code** (as your code editor).
4. **Browser** (to access the application).

---

## Installation Guide

### Step 1: Clone the Repository
Clone the repository using Git or download the ZIP file:
```bash
git clone https://github.com/your-username/school-management-system.git
```
Extract the ZIP file if downloaded manually.

### Step 2: Configure the Project
1. Open the project folder in **VS Code**.
2. Rename `.env.example` to `.env` and update it with the following:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=schoolaravel
   DB_USERNAME=root
   DB_PASSWORD=
   ```

### Step 3: Install Dependencies
Open the integrated terminal in VS Code and run:
```bash
composer install
```

### Step 4: Set Up the Database
1. Start XAMPP and ensure **Apache** and **MySQL** are running.
2. Open **phpMyAdmin** at:
   ```
   http://localhost/phpmyadmin/
   ```
3. Create a new database named `schoolaravel`:
   ```sql
   CREATE DATABASE schoolaravel;
   ```

### Step 5: Run Migrations and Seeders
Execute the following commands in the terminal:
```bash
php artisan migrate
php artisan db:seed
```
This will create the necessary database tables and seed them with default data.

### Step 6: Start the Application
Serve the application locally with:
```bash
php artisan serve
```
Access the application at:
```
http://127.0.0.1:8000/home
```

---

## Login Credentials

Use the following credentials for different roles:

### Admin
- **Email**: `admin@mail.com`
- **Password**: `12345678`

### Teacher
- **Email**: `teacher@mail.com`
- **Password**: `12345678`

### Student
- **Email**: `student@mail.com`
- **Password**: `12345678`

### Parent
- **Email**: `parent@mail.com`
- **Password**: `12345678`

---

## Usage Instructions

### Admin
- Manage users, classes, and roles.
- Track school-wide attendance and performance metrics.

### Teacher
- Manage assigned classes and attendance.
- Interact with students and parents.

### Student
- View assignments, schedules, and grades.
- Access attendance records.

### Parent
- Monitor children’s progress and attendance.
- View school announcements.

---

## License

This project is open-source and available under the [MIT License](LICENSE).
