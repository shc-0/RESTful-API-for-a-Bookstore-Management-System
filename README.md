# FarmwiseAI's Backend Developer Assignment Documentation

## Introduction

This documentation provides an overview of the backend development assignment for FarmwiseAI. The assignment is structured into several modules, each contributing to the development of a backend system. The modules include System Modules, Code Base Modules, DBMS Model, and APIs.

## System Modules

### Swagger
- Provides a tool for API documentation.
- Authentication and authorization are essential components for secure API access.
- Logger for capturing system logs.
- Endpoints define the available routes for communication.
- API rate limiter helps control the rate of incoming requests.

### Socket Information
- Retrieves information about the host system, such as hostname, IPv4 address, and IPv6 address.
- Displays LAN Website URL using the IPv6 address.

## Code Base Modules

### Flask
- Web framework for building the backend application.

### SQLAlchemy
- SQL toolkit and Object-Relational Mapping (ORM) for database operations.

### Marshmallow
- Library for object serialization/deserialization.

### HTTPBasicAuth
- Provides basic HTTP authentication support.

### Configuration
- Configures the Flask application with necessary settings, including the database URI.

## DBMS Model

### User Model
- Represents a user with attributes like id, username, email, password hash, and role.
- Provides methods for hashing and verifying passwords.

### Book Model
- Represents a book with attributes like id, title, author, ISBN, price, and quantity.

### BookSchema
- Defines the serialization schema for Book model.

## APIs

### /book (POST)
- Adds a new book to the database.
- Requires authentication.

### /book (GET)
- Retrieves all books from the database.
- Requires authentication.

### /book/<isbn> (GET)
- Retrieves a specific book by ISBN.
- Requires authentication.

### /book/<isbn> (PUT)
- Updates information for a specific book by ISBN.
- Requires authentication.

### /book/<isbn> (DELETE)
- Deletes a specific book by ISBN.
- Requires authentication.

### Authentication
- Uses basic HTTP authentication.
- Validates users based on provided credentials.

### Error Handling
- Custom error handler for handling 404 (Not Found) errors.

## Usage

- Run the provided Flask application to start the server.
- Access the API endpoints using appropriate HTTP methods.
- Ensure proper authentication for secured routes.

## Conclusion

This backend development assignment demonstrates the implementation of a RESTful API using Flask, SQLAlchemy, and other related libraries. It provides a foundation for building a secure and scalable backend system for managing books.
