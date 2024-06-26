# Loverary

Welcome to Loverary! This project is part of our Intro to Software Engineering and OOP with Java course. It aims to provide a simple and effective way to manage a library's book inventory, track borrowed books, and handle user accounts. 

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Setup and Installation](#setup-and-installation)
5. [Usage](#usage)
6. [License](#license)
7. [Contact](#contact)

## Project Overview

Loverary is designed to help library admins and staff members to manage book inventories and track the borrowing and returning of books. Users can browse available books, borrow books, and return them once they're done. The system also handles user registration and authentication.

## Features

- **Admin, Member and Staff Registration and Authentication**: Each can create accounts and log in to the system.
- **Book Inventory Management**: Library Admin can add, edit, and remove books from the inventory.
- **Book Borrowing and Returning**: Users can borrow available books and return them after use.
- **Search and Filter**: Users can search for books by title, author, genre, or ISBN.
- **User Dashboard**: Users can view their borrowed books and due dates.

## Technologies Used

- **Java**: The core programming language used for the system.
- **Java Swing**: Used for building the graphical user interface.
- **PostgreSQL**: A popular and efficient database to store user and book information.
- **Jira**: For effective project management.
- **Visual Paradigm**: For depicting models and high/low level architectural designs.
- **Maven**: For package management.

## Setup and Installation

To set up the project on your local machine, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Think-Co/loverary.git
    ```

2. **Open the project in IntelliJ IDEA**:
    - Open IntelliJ IDEA.
    - Select `File > Open` and choose the project directory.

3. **Setup the database**:
    - Ensure postgreSQL is installed on your machine.
    - Run the provided SQL script to set up the database schema (e.g., `setup.sql`).

4. **Build and run the project**:
    - Open the terminal in IntelliJ IDEA.
    - Build the project using Maven:
      ```bash
      mvn clean install
      ```

## Usage

1. **Register or Log in**:
   - Open the application.
   - Register a new account or log in with existing credentials.

2. **Browse and Search Books**:
   - Use the search bar to find books by title, author, genre, or ISBN.
   - Browse the list of available books.

3. **Borrow and Return Books**:
   - Select a book to borrow.
   - View borrowed books in your dashboard.
   - Return books when you're done.

4. **Manage Inventory** (for staff):
   - Add new books to the inventory.
   - Edit or remove existing books.

## License

This project is licensed under the MIT License. 

## Contact

If you have any questions or suggestions, feel free to reach out to us:

- **Email**: thinkCo@gmail.com

Happy Managing!
