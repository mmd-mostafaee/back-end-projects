# Project 4: Real Estate Listings API

## Goal
Build an API for managing real estate property listings.

## Tools
- Django
- Django REST Framework (DRF)
- PostgreSQL

## Features

### Property Model
- Fields: `title`, `description`, `price`, `address`, `city`, `created_at`, `updated_at`, `agent`
- Relations: One-to-many with an `Agent` model (a real estate agent can manage multiple properties)

### Agent Model
- Fields: `name`, `email`, `phone`

### API Endpoints
- **GET /properties/** – List all properties
- **GET /properties/{id}/** – Retrieve a specific property by ID
- **POST /properties/** – Add a new property
- **PUT /properties/{id}/** – Update an existing property
- **DELETE /properties/{id}/** – Delete a property

### Advanced Features
- **Search and Filtering:** Allow users to search properties by city, price range, or agent.
- **Ordering:** Provide ordering options for properties (e.g., by price or date).

### DRF Features
- Use nested serializers to return agent information with property listings.
- Implement complex queries using Django ORM for search functionality.

## Learning Objectives
- Learn to use nested serializers to manage relationships between models.
- Implement advanced querying for search and filter functionality.

### Bonus:
- Add JWT-based user authentication so that only registered agents can add or modify property listings.
- Implement rate limiting and throttling for API requests to prevent abuse.

---

## Testing

### Unit Tests
- Test the models and relationships between `Property` and `Agent`.
- Test serializers, ensuring they handle nested relationships properly.

### API Tests
- Test search and filtering endpoints (e.g., `/properties?city=London`).
- Test rate limiting and throttling to ensure the API handles high traffic.
