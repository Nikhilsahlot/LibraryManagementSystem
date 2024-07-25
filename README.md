# Library Management System

## Project Overview

The Library Management System is a web-based application developed using **Spring Boot** and **Thymeleaf** for managing book inventory. It uses an **H2 in-memory database** for development.

## Key Features

- **View Books**: Users can view a list of all books with details including book name, author, and price.
- **Search Books**: Users can search for books by name using a search box.
- **Add Books**: Users can add new books to the system via a form.
- **Delete Books**: Users can remove books from the system.

## Technologies Used

### Backend

- **Spring Boot**: Provides the framework for building the RESTful API and handling business logic.
- **Spring Data JPA**: Simplifies database operations with repository support for CRUD operations.
- **H2 Database**: An in-memory database used for storing book information and user interactions during development.

### Frontend

- **Thymeleaf**: A templating engine used to render dynamic HTML views and forms.
- **HTML/CSS**: For creating the user interface with proper styling.

## Architecture

1. **Model**: Defines the data structure with a `Book` entity representing book details, mapped to the H2 database.
2. **Repository**: `BookRepository` interface extends `JpaRepository`, providing built-in CRUD operations and custom queries.
3. **Service**: `BookService` contains business logic for managing book data, including operations like adding, deleting, and searching for books.
4. **Controller**: `BookController` handles HTTP requests, maps them to service methods, and returns the appropriate views to the user.

## Configuration

- **Database Configuration**: The application is configured to use an H2 in-memory database for development, with properties defined in `application.properties` or `application.yml`.

## Development Highlights

- Implemented form-based interactions for adding and deleting books.
- Incorporated search functionality with dynamic query methods.
- Utilized Thymeleaf for server-side rendering and HTML generation.

## Challenges and Solutions

- **Database Integration**: Configured H2 as the database for development, ensuring proper CRUD operations.
- **Error Handling**: Implemented error handling for scenarios such as unsupported HTTP methods and validation issues.

