# User Management System - Final Project
# User Management System

Welcome to my user management system project. This project is my user management system built for the NJIT final assignment.

...

## Overview
This project is a robust User Management System built with FastAPI and Docker.  
It provides secure user registration, login, and role-based access control to manage user profiles efficiently.

## Features
- User registration and login with JWT authentication  
- Role-based access control (Admin, Manager, User)  
- CRUD operations on user profiles (Create, Read, Update, Delete)  
- Email verification integration  
- Secure password handling with hashing and salting  
- API documented with OpenAPI  
- Dockerized deployment for easy setup and consistent environment  
- Automated database migrations using Alembic  

## Getting Started

### Prerequisites
- Python 3.12+  
- Docker and Docker Compose  
- Git  

### Installation

1. Clone the repository  
   ```bash
   git clone https://github.com/KellyNzale/user_management.git
   cd user_management
Build and start the Docker containers

bash
Copy
Edit
docker-compose up --build
Run database migrations

bash
Copy
Edit
docker exec -it user_management-fastapi-1 alembic upgrade head
Access the API documentation at http://localhost:8000/docs

Usage
Register a new user
Send a POST request to /register/ with JSON body including email, password, and profile details.

Login
Send a POST request to /login/ with username (email) and password to receive a JWT token.

Manage users
Use the /users/ endpoints to create, read, update, or delete users. Role-based access control applies.

Testing
API endpoints were tested using curl and Postman.

Additional unit and integration tests were implemented to cover key functionality.

Project Structure
app/ - FastAPI application source code

alembic/ - Database migration scripts

docker-compose.yml - Docker configuration

Dockerfile - FastAPI app container instructions

Contribution
This is an individual project, but feel free to open issues or suggest improvements.

License
MIT License

Author: Kelly Nzale
Date: August 2025

Copy
Edit
