# 🛒 E-commerce API Testing using Postman

## 📌 Project Overview

This project demonstrates REST API testing for an E-commerce application using Postman. It covers authentication, CRUD operations, environment variables, automated test scripts, and collection execution.

## 🚀 Features

- User Authentication (Login API)
- Token-based Authorization
- Get User Profile
- Get All Products
- Get Single Product
- Add New Product
- Update Product
- Delete Product
- Environment Variables
- Automated Test Scripts
- Collection Runner Execution

## 🛠️ Tools Used

- Postman
- DummyJSON REST API
- JavaScript (Postman Test Scripts)

## 📂 APIs Tested

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/auth/login` | User Login |
| GET | `/auth/me` | Get User Profile |
| GET | `/products` | Get All Products |
| GET | `/products/{{product_id}}` | Get Single Product |
| POST | `/products/add` | Add New Product |
| PUT | `/products/{{product_id}}` | Update Product |
| DELETE | `/products/{{product_id}}` | Delete Product |

## 🔑 Environment Variables

- `base_url`
- `token`
- `product_id`
- `new_product`
- `deleted_product`

## ✅ Test Scripts

The following validations are implemented:

- Status Code Validation
- Response Validation
- Dynamic Variable Storage
- Environment Variable Update

Example:

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

let jsonData = pm.response.json();
pm.environment.set("product_id", jsonData.id);
```

## ▶️ How to Run

1. Clone this repository.
2. Open Postman.
3. Import:
   - `Ecom_API_Project.postman_collection.json`
   - `MyENV1.postman_environment.json`
4. Select **MyENV1** Environment.
5. Run the collection using **Collection Runner**.

## 📷 Screenshots

- Login API
login_API.png 

- Get Products
get_products.png

- Add Product
adding_product-2.png

- Update Product
update_product.png

- Delete Product
delete_product.png

- Collection Runner Results
env_runner.png

## 📁 Repository Structure

```
Ecom-API-Testing-Postman/
│
├── Ecom_API_Project.postman_collection.json
├── MyENV1.postman_environment.json
├── README.md
└── screenshots/
```

## 📚 Learning Outcomes

- REST API Testing
- CRUD Operations
- Authentication using Bearer Token
- Environment Variables
- Dynamic Data Handling
- Automated Test Scripts
- Collection Runner
- API Validation

## 👨‍💻 Author

**Kumar Suraj**

GitHub: https://github.com/kumar-983

LinkedIn: https://www.linkedin.com/in/kumar-suraj-204a5b269