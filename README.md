# 🛒 E-commerce API Testing using Postman

## 📌 Project Overview

This project demonstrates API testing of an e-commerce application using Postman. The APIs are based on the Fake Store API and cover core functionalities such as user authentication, product retrieval, and cart operations.

The objective of this project is to showcase API testing skills including request creation, validation, chaining, and handling both positive and negative scenarios.

---

## 🛠 Tools & Technologies

* Postman
* JavaScript (for test scripting)

---

## 📂 APIs Covered

* 🔐 Login API (Authentication)
* 📦 Get All Products
* 🔍 Get Single Product
* 🛒 Cart APIs (Get/Add/Update)

---

## ✅ Test Coverage

* Status code validation (200, 201, etc.)
* Response time validation
* JSON response validation
* Data verification in response body
* API chaining using variables
* Environment variable usage

---

## ❌ Negative Test Scenarios

* Invalid login credentials
* Missing required fields
* Invalid product ID
* Unauthorized access scenarios

---

## 🔗 Key Features

* ✔ API request chaining implemented
* ✔ Dynamic data handling using environment variables
* ✔ Test scripts written using JavaScript
* ✔ Organized Postman collection structure
* ✔ Coverage of both positive and negative scenarios

---

## 🧪 Sample Test Script

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains product title", function () {
    let jsonData = pm.response.json();
    pm.expect(jsonData[0]).to.have.property("title");
});
```

---

## 🛒 Business Flow Covered

* User authentication (Login)
* Product listing and retrieval
* Cart operations (view/add/update)

---

## ▶️ How to Run the Project

1. Import the Postman Collection
2. Import the Environment file
3. Select the environment in Postman
4. Run the collection using Collection Runner

---

## 📁 Project Structure

```
ecommerce-api-testing-postman/
 ┣ collections/
 ┃ ┗ collection.json
 ┣ environments/
 ┃ ┗ environment.json
 ┗ README.md
```

---

## 👩‍💻 Author

**Anantha Mariya Stella**
QA Lead | API Testing
