# Console-Based Library Management System

## Project Description
This is a simple, console-based Library Management System implemented in Java. It allows users to manage books, register users, and handle the borrowing and returning of books. All data is stored in memory using Java Collections and will be lost upon program exit. It serves as a practical demonstration of object-oriented programming, data structures, and basic console application development in Java.

## Features
- Add new books with details (title, author, ISBN, publication year, genre).
- Register new users with a unique ID and name.
- Borrow books by specifying a user ID and book ISBN.
- Return books by specifying the book ISBN.
- Display a list of all books in the library (available and borrowed).
- Display only currently available books.
- Display a list of all registered users.
- View all books currently borrowed by a specific user.
- Search for books by title, author, or ISBN.
- Search for users by ID or name.
- Basic input validation to ensure data integrity (e.g., non-empty fields, valid ISBN/year formats, uniqueness checks).
- Error handling for invalid operations (e.g., borrowing an unavailable book, returning an un-borrowed book, user/book not found).

## How to Compile and Run

### Prerequisites
- Java Development Kit (JDK) installed (JDK 11 or higher is recommended).

### Steps
1.  **Save the files:** Save all the `.java` files into the corresponding directory structure (`src/com/example/lms/model`, `src/com/example/lms/service`, `src/com/example/lms/util`, `src/com/example/lms`).
2.  **Navigate to the `src` directory:** Open your terminal or command prompt and navigate to the `src` directory of your project.
    ```bash
    cd path/to/your/LMS/src
    ```
3.  **Compile the Java files:** Compile all the Java source files.
    ```bash
    javac com/example/lms/model/*.java com/example/lms/service/*.java com/example/lms/util/*.java com/example/lms/*.java
    ```
    Alternatively, if you are in the `src` directory:
    ```bash
    javac com/example/lms/**/*.java
    ```
4.  **Run the application:** After successful compilation, run the `Main` class.
    ```bash
    java com.example.lms.Main
    ```

## Usage
Upon running the application, a menu will be displayed in the console. Enter the number corresponding to the action you wish to perform and follow the on-screen prompts.

## Assumptions
- All data is stored in memory and will not persist after the program exits.
- ISBN is considered a unique identifier for books.
- User ID is considered a unique identifier for users.
- A simple, fixed loan period is assumed for tracking, but not explicitly enforced as "overdue" in this version.
