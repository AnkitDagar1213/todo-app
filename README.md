# Todo Application

This is a Todo application built with Java and the Spring framework.

## Data Flow

The application follows a typical Spring architecture with the following components:

Controller - Receives HTTP requests and sends responses.

Service - Contains the business logic and processes data.

Repository - Persists data to a database.

Database Design - Defines the structure and relationships of the data in the database.

### Controller

The TodoController class receives HTTP requests and sends responses. It uses the following functions:

addTodo - Adds a new Todo object to the database.

findTodoById - Finds a Todo object by its ID in the database.

findAllTodos - Retrieves all Todo objects from the database.

updateTodo - Updates an existing Todo object in the database.

deleteTodo - Deletes a Todo object from the database by its ID.

### Service

The TodoService class contains the business logic and processes data. It uses the following functions:

findAll - Retrieves all Todo objects from the database.

findById - Finds a Todo object by its ID in the database.

addTodo - Adds a new Todo object to the database.

deleteTodo - Deletes a Todo object from the database by its ID.

updateTodo - Updates an existing Todo object in the database.

### Repository

The TodoRepository interface defines the methods for interacting with the database. It uses the following functions:

findAll - Retrieves all Todo objects from the database.

findById - Finds a Todo object by its ID in the database.

save - Adds a new Todo object to the database or updates an existing one.

deleteById - Deletes a Todo object from the database by its ID.

## Database Design

The Todo table in the database has the following columns:

id (int) - The unique identifier for each Todo object.

title (varchar) - The title of the Todo.

status (boolean) - The status of the Todo (true for completed, false for incomplete).

## Data Structure

The application uses a List data structure to hold Todo objects in memory. The data is persisted to a MySQL database using the Spring Data JPA framework.

## Project Summary

This Todo application provides a simple API for managing Todo objects. Users can create, read, update, and delete Todo objects using HTTP requests. The application uses Java and the Spring framework to provide a scalable and maintainable architecture.
