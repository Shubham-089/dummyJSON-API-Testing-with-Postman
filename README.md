# DummyJSON Postman Collection

## 📸 Project Image  
![Screenshot 2025-06-08 200319](https://github.com/user-attachments/assets/52ccf8d4-24f7-480b-9010-c387db1d4635)


This Postman collection provides a set of pre-configured requests for interacting with the [DummyJSON API](https://dummyjson.com). DummyJSON is a fake REST API for prototyping and testing frontend or backend applications.

## Base URL
https://dummyjson.com/

---

## 📦 Products Endpoints

### 1. **Get all products**
- **Method**: `GET`
- **URL**: `/products`
- **Description**: Fetches a list of all available products.

### 2. **Get a single product**
- **Method**: `GET`
- **URL**: `/products/1`
- **Description**: Fetches the product details with ID = 1.

### 3. **Search product**
- **Method**: `GET`
- **URL**: `/products/search?q=phone`
- **Description**: Searches for products containing the keyword "phone".

### 4. **Limit and Skip products**
- **Method**: `GET`
- **URL**: `/products?limit=10&skip=10&select=title,price`
- **Description**: Fetches 10 products, skips the first 10, and returns only the title and price.

### 5. **Sort products**
- **Method**: `GET`
- **URL**: `/products?sortBy=title&order=asc`
- **Description**: Sorts the products by title in ascending order.

---

## 📁 Categories

### 6. **Get all product categories**
- **Method**: `GET`
- **URL**: `/products/categories`
- **Description**: Returns a list of all product categories.

### 7. **Get category list**
- **Method**: `GET`
- **URL**: `/products/category-list`
- **Description**: Fetches a categorized product list (if supported by API).

### 8. **Get products by category**
- **Method**: `GET`
- **URL**: `/products/category/smartphones`
- **Description**: Fetches all products under the "smartphones" category.

---

## 🛠️ Product Management

### 9. **Add a product**
- **Method**: `POST`
- **URL**: `/products/add`
- **Description**: Adds a new product (Request body should contain product details in JSON).

### 10. **Update a product**
- **Method**: `PUT`
- **URL**: `/products/1`
- **Description**: Updates the product with ID = 1.

### 11. **Delete a product**
- **Method**: `DELETE`
- **URL**: `/products/1`
- **Description**: Deletes the product with ID = 1.

---

## 🔐 Authentication

### 12. **Login**
- **Method**: `POST`
- **URL**: `/auth/login`
- **Description**: Authenticates a user and returns a token.
- **Sample Body**:
```json
{
  "username": "emilys",
  "password": "emilyspass",
  "expiresInMins": 30
}


