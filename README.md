**Project Description**

The Library Management System is a web application designed to efficiently and easily manage a library. The system provides an interactive interface for managing books, users, and borrowing and returning operations. It was developed using Java and Spring Boot, and uses a PostgreSQL database to store data. The system allows users to add, update, delete, and view books and users, as well as record borrowing and returning transactions.

**Tools and Technologies Used:**

Java: The primary programming language used to develop the application logic.
Spring Boot: A framework that helps in rapidly developing web applications.
PostgreSQL: The database used to store data.
Maven/Gradle: Project management tools that help in building, testing, and deploying the project.
JUnit: A framework for unit testing in Java to ensure code quality.
Git/GitHub: Tools for managing and sharing the source code versions.
Key Features

**Book Management:**

Add a new book.
Update book details.
Delete books.
View a list of all books.

**User Management:**

Add a new user.
Update user details.
Delete users.
View a list of all users.

**Borrowing Management:**

Record a book borrowing for a user.
Record the return of a book.
View a list of all borrowing and returning transactions.

**Project Structure**

**Main Components:**

LibraryManagementSystemApplication: The main entry point of the application.
LibraryController: The controller that handles HTTP requests and directs them to the appropriate services.
LibraryService: The service containing the core business logic.
Book, User, Borrowing: Data models representing the tables in the database.
BookRepository, UserRepository, BorrowingRepository: Data repositories for interacting with the database.

**Testing:**

Unit tests using JUnit to verify the correctness of the application logic.
Configuration:

The application.properties file for database configuration and Hibernate settings.
Usage Instructions

**Database Setup:**

Create a PostgreSQL database named library_management.
Ensure to update the database connection settings in the application.properties file.
Running the Application:

Run the Spring Boot application using the command mvn spring-boot:run or using an IDE like IntelliJ IDEA or Eclipse.
Interacting with the System:

Use tools like Postman to send HTTP requests to various endpoints for managing books, users, and borrowings.
Endpoints

**Books:**

GET /library/books: View all books.
POST /library/books: Add a new book.
PUT /library/books/{id}: Update a book.
DELETE /library/books/{id}: Delete a book.

**Users:**

GET /library/users: View all users.
POST /library/users: Add a new user.
PUT /library/users/{id}: Update a user.
DELETE /library/users/{id}: Delete a user.

**Borrowings:**

POST /library/borrow: Record a book borrowing.
PUT /library/return/{id}: Record a book return.
GET /library/borrowings: View all borrowings.
