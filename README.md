# Task7

# Java JDBC – Employee Database App

## Objective
This application demonstrates Java Database Connectivity (JDBC) for managing an employee database with basic CRUD operations.

## Features
- Add a new employee
- View all employees
- Update employee details
- Delete employee

## Setup Guide

1. **Database Setup**:
   - Run the following SQL to create the database and table:
     ```sql
     CREATE DATABASE employee_db;
     USE employee_db;

     CREATE TABLE employees (
         id INT AUTO_INCREMENT PRIMARY KEY,
         name VARCHAR(100),
         department VARCHAR(100),
         salary DOUBLE
     );
     ```

2. **Java Setup**:
   - Ensure MySQL is installed and running.
   - Use MySQL JDBC driver (`mysql-connector-java.jar`).
   - Update the DB credentials in the code if needed.

3. **Compile and Run**:
   ```bash
   javac EmployeeDBApp.java
   java -cp .:mysql-connector-java.jar EmployeeDBApp
   ```

## Code Explanation
- `Connection`: Establishes a connection to MySQL.
- `PreparedStatement`: Used to execute parameterized SQL queries.
- `ResultSet`: Fetches and displays employee data.
- Scanner is used for interactive command-line input.

Enjoy building with JDBC!
