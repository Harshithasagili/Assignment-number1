# Assignment-number1
This is CS253 Assignment number1

# Vehicle Rental Management System

## Introduction
The Vehicle Rental Management System is engineered to streamline the operations involved in renting vehicles, leveraging C++ for the logic and MongoDB for storing data. This system is designed to cater to the needs of customers, employees, and managers within a rental service, offering functionalities for the renting process, vehicle management, and user account handling.

## Requirements
- A running MongoDB server instance (either locally hosted or on the cloud).
- The MongoDB C++ Driver, properly installed within your C++ development setup.
- A compiler compatible with C++17 standards.

## Configuration and Deployment

### Database Preparation:
1. Confirm the availability of MongoDB on your system or opt for MongoDB Atlas for cloud-based services.
2. Initiate a carRentalDB database with customers, employees, and cars collections in MongoDB.

### Development Environment Setup:
1. Ensure the presence of a C++17 compliant compiler in your environment.
2. Adhere to the MongoDB C++ Driver setup instructions for installation.

### System Configuration:
1. Modify the MongoDB connection URI in the program's main function to align with your MongoDB deployment details.

   
# Car Rental System

## Overview
This is a Car Rental System application implemented in C++ that integrates with MongoDB for managing car rentals. It features functionalities for users in different roles such as customers, employees, and managers, to interact with the system according to their permissions.

## Features
- *User Authentication*: Supports secure login for customers, employees, and managers using IDs and passwords.
- *Car Management*: Enables the management of cars within the system, including adding, updating, viewing, and deleting car records.
- *User Interactions*: Allows customers to rent and return cars, and view their profiles including rental history and dues. Employees can rent cars under specific conditions, and managers have comprehensive control over all system operations.
- *Database Integration*: Utilizes MongoDB to store and retrieve all data related to cars, users, and transactions, showcasing how to perform CRUD operations in a C++ application.

## Key Components
- *User*: An abstract class that defines the common interface for all user types in the system. It includes methods for car rental activities and user information display.
- *Customer & Employee*: Derived classes from User, providing specific implementations for renting and returning cars. They include additional attributes and methods tailored to their respective roles.
- *Car*: Represents a car in the rental system with attributes such as ID, model, condition, and rental status.
- *Manager*: Inherits from User and includes administrative functions to manage the database records for cars, customers, and employees.
- *Database*: Manages database connections and operations with MongoDB, performing actions like adding, updating, and deleting records, as well as user verification.

## MongoDB Integration
The application demonstrates how to use the MongoDB C++ Driver to connect to a MongoDB database, create BSON documents for storage, and execute queries for various database operations.

## Compilation and Running
The system requires MongoDB C++ Driver installed and a MongoDB server running. Compile the code with a C++ compiler supporting C++11 or higher. Make sure to link against the MongoDB C++ Driver libraries.

## Conclusion
This Car Rental System is an example of a comprehensive application combining modern C++ with database operations, suitable for educational purposes or as a basis for more complex systems.
