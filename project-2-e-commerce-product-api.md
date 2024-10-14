# Project 2: E-Commerce Product API

## Goal
Build an API for managing products in an e-commerce store.

## Tools
- Django
- Django REST Framework (DRF)
- PostgreSQL

## Features

### Product Model
- Fields: `name`, `description`, `price`, `category`, `created_at`, `updated_at`

### Category Model
- Fields: `name`
- Relations: One-to-many relationship with `Product` (a category can have multiple products)

### API Endpoints
- **GET /products/** – List all products
- **GET /products/{id}/** – Retrieve a specific product by ID
- **POST /products/** – Create a new product
- **PUT /products/{id}/** – Update a product
- **DELETE /products/{id}/** – Delete a product
- **GET /categories/** – List all categories

### Advanced Features
- **Filtering:** Implement filtering by category or price range (e.g., `/products?category=1&price_min=100&price_max=500`)
- **Ordering:** Allow products to be ordered by price or name.

### DRF Features
- Use `ViewSet` and routers to simplify the endpoint configuration.
- Use `SerializerMethodField` to return computed fields (e.g., product discounts, if applicable).

## Learning Objectives
- Master using `ViewSets` and routers for clean, concise API architecture.
- Implement filtering, ordering, and pagination in DRF.

### Bonus:
- Add user authentication and permissions, allowing only authorized users to create or modify products.

---

## Testing

### Unit Tests
- Test the `Product` and `Category` models to ensure relationships and constraints are correct.
- Test the serializers to ensure proper validation and data representation.

### API Tests
- Test all API endpoints (e.g., `GET /products/`, `POST /products/`).
- Test filtering and ordering functionality, ensuring correct results for different parameters.
- Test permissions (e.g., unauthenticated users cannot create products).
