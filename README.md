# Library-Management-System

Library Management System
Table of Contents
Introduction
Features
Technologies Used
Database Schema
Installation
Usage
Contributing
License
Contact
Introduction
The Library Management System is a simple project designed to manage library operations such as tracking book inventory, issuing books, and handling book returns. This system facilitates the management of library resources and ensures efficient tracking of book availability.

Features
Add Book: Add new books to the library inventory.
Issue Book: Issue books to library members.
Submit Book: Handle the return of issued books.
Delete Book: Remove books from the inventory.
Display Books: Display the list of all books available in the library.
Technologies Used
Backend: MySQL for database management
Programming Language: Python
Libraries: mysql-connector-python for connecting Python with MySQL
Database Schema
The database schema consists of the following tables:

Books: Stores information about books.

bname (VARCHAR): Name of the book
bcode (VARCHAR, Primary Key): Unique code for each book
total (INT): Total number of copies available
subject (VARCHAR): Subject or genre of the book
Issue: Tracks book loans.

name (VARCHAR): Name of the person issuing the book
regno (VARCHAR): Registration number of the person
bcode (VARCHAR, Foreign Key): Code of the issued book
idate (DATE): Issue date
Submit: Tracks book returns.

name (VARCHAR): Name of the person returning the book
regno (VARCHAR): Registration number of the person
bcode (VARCHAR, Foreign Key): Code of the returned book
sdate (DATE): Submission date
Installation
Prerequisites
MySQL Server
Python
mysql-connector-python library
Steps
Clone the repository:
git clone https://github.com/ashutoasst/library-management-system.git
cd library-management-system
Set up the database:

Create the database and tables in MySQL.
sql
CREATE DATABASE lmanage;
USE lmanage;

CREATE TABLE books (
    bname VARCHAR(255),
    bcode VARCHAR(255) PRIMARY KEY,
    total INT,
    subject VARCHAR(255)
);

CREATE TABLE issue (
    name VARCHAR(255),
    regno VARCHAR(255),
    bcode VARCHAR(255),
    idate DATE,
    FOREIGN KEY (bcode) REFERENCES books(bcode)
);

CREATE TABLE submit (
    name VARCHAR(255),
    regno VARCHAR(255),
    bcode VARCHAR(255),
    sdate DATE,
    FOREIGN KEY (bcode) REFERENCES books(bcode)
);
Install the required Python library:

pip install mysql-connector-python
Configure the database connection:

Update the database connection settings in the Python script (if necessary).
Run the application:

python app.py
Usage
Run the script:

python app.py
Enter the username:

A random password will be generated and displayed.
Enter the displayed password to access the main menu.

Main Menu:

1. Add book: Add new books to the library.
2. Issue book: Issue books to members.
3. Submit book: Return issued books.
4. Delete book: Remove books from the library.
5. Display book: Display all books in the library.
Contributing
Contributions are welcome! Please follow these steps to contribute:

Contact
For any questions or suggestions, feel free to contact me at:

Email: ashutoshtripathi5914@gmail.com

GitHub: [ashutoasst](https://github.com/ashutoasst/Library-Management-System/edit/main/README.md)
