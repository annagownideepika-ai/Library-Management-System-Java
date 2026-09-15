# Library Management System

A simple Library Management System developed using **Java, JDBC, and MySQL**.

## Description

The Library Management System is a console-based Java application used to manage books in a library. It provides basic operations such as adding, viewing, searching, issuing, returning, and deleting books.

## Features

* Add a new book
* View all books
* Search for a book
* Issue a book
* Return a book
* Delete a book
* Store book information in MySQL

## Technologies Used

* Java
* JDBC
* MySQL
* Maven
* IntelliJ IDEA / Eclipse / VS Code

## Database Setup

Create the database:

```sql
CREATE DATABASE library_db;

USE library_db;

CREATE TABLE books (
    id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(150) NOT NULL,
    author VARCHAR(100) NOT NULL,
    category VARCHAR(100),
    available BOOLEAN DEFAULT TRUE
);
```

## Configuration

Open `DatabaseConnection.java` and change the MySQL username and password:

```java
private static final String USER = "root";
private static final String PASSWORD = "your_password";
```

Replace `your_password` with your MySQL password.

## How to Run

1. Install Java.
2. Install MySQL.
3. Create the `library_db` database.
4. Create the `books` table using the SQL above.
5. Add the MySQL JDBC driver to the project.
6. Update the database username and password.
7. Run `Main.java`.
8. Select an option from the menu.

## Modules

### Add Book

Adds a new book with its title, author, and category.

### View Books

Displays all books and their availability status.

### Search Book

Searches for a book using its ID.

### Issue Book

Changes the book status from available to issued.

### Return Book

Changes the book status from issued to available.

### Delete Book

Deletes a book record from the database.

## CRUD Operations

* **Create** → Add Book
* **Read** → View/Search Book
* **Update** → Issue/Return Book
* **Delete** → Delete Book

## Project Purpose

This project demonstrates Java programming, JDBC connectivity, MySQL database operations, SQL queries, exception handling, and CRUD operations.

## Future Enhancements

* Add a graphical user interface
* Add student/member management
* Add librarian login
* Add issue and return dates
* Add fine calculation
* Add book search by title or author
* Add book categories

## License

This project is created for educational purposes.
