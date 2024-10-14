# Project 1: Simple Blog API

## Goal
Build a basic blog API that supports CRUD operations for blog posts and authors.

## Tools
- Django
- Django REST Framework (DRF)
- PostgreSQL

## Features

### Blog Post Model
- Fields: `title`, `content`, `created_at`, `author`
- Relations: One-to-many relationship with an `Author` model

### API Endpoints
- **GET /posts/** – Retrieve a list of all blog posts
- **GET /posts/{id}/** – Retrieve a specific blog post by its ID
- **POST /posts/** – Create a new blog post
- **PUT /posts/{id}/** – Update an existing post
- **DELETE /posts/{id}/** – Delete a post

### Author Model
- Fields: `name`, `email`

### DRF Features
- Use `ModelSerializer` to automatically create serializers for the `Post` and `Author` models.
- Use `APIView` for defining the basic CRUD logic for the blog post.

## Learning Objectives
- Understand basic Django model structure and relationships.
- Learn how to use serializers to convert querysets to JSON.
- Create and wire up API views with proper URL routing using DRF.

### Bonus:
- Implement pagination for the `GET /posts/` endpoint.
- Add simple filtering (e.g., by `author` or `created_at`).

---

## Testing

### Unit Tests
- Test the models to ensure proper relationships between `Post` and `Author`.
- Test the serializers to ensure correct data representation and validation.

### API Tests
- Test each API endpoint (e.g., `GET /posts/`, `POST /posts/`) to ensure proper functionality.
- Test edge cases such as invalid data submissions (e.g., missing fields in a POST request).
