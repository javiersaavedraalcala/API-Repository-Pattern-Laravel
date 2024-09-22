# RESTful API CRUD Application in Laravel 11

This project involves creating a RESTful API for managing products, implemented using Laravel 11. This repository serves as a guide for anyone interested in learning how to build CRUD applications with Laravel while adhering to best practices.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage of Repository Pattern and Service Provider](#usage-of-repository-pattern-and-service-provider)
- [API Usage](#api-usage)
- [Contribution](#contribution)
- [License](#license)

## Features

- Full CRUD functionality for managing products.
- Request validation to ensure data integrity.
- Standardized API response handling.
- Implementation of the Repository design pattern for clean data access.
- Use of Service Providers for binding interfaces to their implementations.
- API resources for formatting responses.

## Requirements

- PHP 8.0 or higher
- Composer
- MySQL (or SQLite for testing)
- Laravel 11

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/javiersaavedraalcala/API-Repository-Pattern-Laravel.git
   cd your_repository

## Usage of Repository Pattern and Service Provider

This project employs the **Repository pattern**, which helps separate the logic for data access from the rest of the application. By doing so, it enhances maintainability and testability.

The **Service Provider** is used to bind the `ProductRepositoryInterface` to its implementation, `ProductRepository`. This allows the application to utilize dependency injection, making it easier to manage dependencies and switch implementations if necessary.

## API Usage

### API Routes

- `GET /api/products`: Retrieves a list of products.
- `POST /api/products`: Creates a new product.
- `GET /api/products/{id}`: Retrieves a specific product.
- `PUT /api/products/{id}`: Updates an existing product.
- `DELETE /api/products/{id}`: Deletes a product.

### Example Request

**Create a new product**:

```http
POST /api/products
Content-Type: application/json

{
    "name": "Example Product",
    "details": "Details about the example product"
}
```

## Contribution

Contributions are welcome! If you want to collaborate, please create a fork of the repository and open a pull request. Any suggestions or improvements are appreciated.

## License

This project is licensed under the MIT License.
