# User Service

## Description
Handles user registration, login, authentication, and role management (USER/ADMIN).

## Technologies
- Java 17
- Spring Boot
- Spring Security (JWT)
- Spring Data JPA
- PostgreSQL
- Spring Boot Starter Mail (for verification emails)
- Maven

## Features
- Register new users
- Login with JWT token
- Role-based access control (ADMIN/USER)
- Email notifications for registration and login alerts

## Endpoints
- `POST /auth/register` → Register user
- `POST /auth/login` → Login and get JWT token

## Database Schema
- **users**
    - id: UUID
    - username: String
    - password: String (hashed)
    - role: String
    - email: String
