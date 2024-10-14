# Project 5: API Performance Optimization and Testing

## Goal
Build a fully optimized and well-tested API.

## Tools
- Django
- Django REST Framework (DRF)
- PostgreSQL
- Django Cache Framework
- DRF Testing Framework

## Features

### Project Optimization
- Enable caching for high-traffic endpoints (e.g., property listings) using Django’s caching framework.
- Optimize database queries with `select_related` and `prefetch_related` to minimize database hits on large datasets.

### Testing
- Write unit tests for all serializers, views, and models.
- Write integration tests to ensure API endpoints return the correct data.

### DRF Features
- Implement API throttling for specific endpoints (e.g., login attempts or property searches).
- Use custom middleware to measure request times and log performance metrics.

## Learning Objectives
- Learn to write unit and integration tests for Django and DRF.
- Implement caching and performance optimizations for large datasets.
- Understand throttling and how to secure APIs against abuse.

### Bonus:
- Add monitoring and logging to track performance metrics and issues.
- Explore load testing tools to simulate high traffic and measure API response times.

---

## Testing

### Unit Tests
- Write tests for each model, serializer, and view to ensure correctness and data integrity.

### API Tests
- Write tests for optimized endpoints to ensure they are working efficiently (e.g., testing cache hits).
- Write tests for throttling to ensure limits are enforced correctly.
