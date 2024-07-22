# Library-Management-System

Library Management System
# Introduction
The Library Management System is a simple project designed to manage library operations such as tracking book inventory, issuing books, and handling book returns. This system facilitates the management of library resources and ensures efficient tracking of book availability.

# Features
This system offers several key features, including the ability to add new books to the library inventory, issue books to library members, handle the return of issued books, remove books from the inventory, and display the list of all books available in the library.

# Technologies Used
The project uses MySQL for database management and Python as the programming language. The mysql-connector-python library is used to connect Python with MySQL.

# Database Schema
The database schema consists of three main tables:

Books: This table stores information about books, including the book name (bname), book code (bcode), total number of copies available (total), and subject (subject).

Issue: This table tracks book loans, including the name of the person issuing the book (name), their registration number (regno), the code of the issued book (bcode), and the issue date (idate).

Submit: This table tracks book returns, including the name of the person returning the book (name), their registration number (regno), the code of the returned book (bcode), and the submission date (sdate).

# Installation
To set up the project, first ensure you have MySQL Server and Python installed. Then, clone the repository using git clone https://github.com/ashutoasst/library-management-system.git and navigate into the project directory with cd library-management-system.

Next, set up the database by creating the necessary tables in MySQL. You can use the provided SQL commands to create the books, issue, and submit tables. After setting up the database, install the required Python library with pip install mysql-connector-python. Update the database connection settings in the Python script if necessary, and then run the application using python app.py.

# Usage
To use the system, run the script python app.py. You will be prompted to enter a username, and a random password will be generated and displayed. Enter this password to access the main menu. The main menu offers options to add books, issue books, submit books, delete books, and display all books in the library.

# Contributing
Contributions to the project are welcome! To contribute, fork the repository, create a new branch, commit your changes, push to the branch, and open a pull request.

# License
This project is licensed under the MIT License. See the LICENSE file for more details.

# Contact
For any questions or suggestions, feel free to contact me at ashutoashtripathi563@gmail.com or on GitHub at ashutoasst .


