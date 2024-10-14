# Project 3: User Management and JWT Authentication

## Goal
Build a user management system with JWT authentication for secure login and access control.

## Tools
- Django
- Django REST Framework (DRF)
- PostgreSQL
- Simple JWT

## Features

### User Registration
- **POST /register/** – Register a new user with username, email, and password.

### User Login
- **POST /login/** – Authenticate user and return a JWT token.

### User Profile
- **GET /profile/** – Retrieve the authenticated user’s profile.
- **PUT /profile/** – Update the authenticated user’s profile.

### API Endpoints (Protected)
- All user-related API endpoints are protected by JWT tokens.

### DRF Features
- Implement `JWTAuthentication` using `SimpleJWT`.
- Add custom permission classes to protect specific routes (e.g., only authenticated users can view profiles).

## Learning Objectives
- Understand how to implement token-based authentication in Django using JWT.
- Learn how to secure API endpoints with permission classes.

### Bonus:
- Add password reset functionality.
- Implement role-based permissions (e.g., admin users vs. regular users).

---

## Testing

### Unit Tests
- Test user registration logic to ensure correct handling of user data.
- Test JWT token generation and validation.

### API Tests
- Test authentication endpoints (e.g., `POST /login/`) to ensure proper token generation and validation.
- Test protected routes to ensure unauthorized access is restricted.
