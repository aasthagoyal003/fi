📦 Inventory Management System (IMS) – Backend
This project is a backend application designed to manage product inventory. It allows users to register, log in, and perform inventory operations like adding products, updating quantities, and viewing items. The backend ensures only authenticated users can access and modify inventory data.

🔍 What This Project Does
The system supports:

User registration and login using secure tokens (JWT)

Adding new products to the inventory database

Updating the quantity of existing products

Viewing products with support for pagination (viewing data in chunks)

API documentation using Swagger (interactive interface)

Postman support for easily testing the API

🧠 Concepts and Tools Used
This project combines multiple technologies and ideas:

1. Node.js
A JavaScript runtime used to build server-side applications.

2. Express.js
A web framework that helps define API endpoints and handle HTTP requests easily.

3. MongoDB
A NoSQL database used to store users and product details.

4. Mongoose
An Object Data Modeling (ODM) library that connects the app to MongoDB and helps define the structure of data.

5. JWT (JSON Web Tokens)
A method of securely transmitting user authentication data. Once a user logs in, they receive a token which must be provided for accessing protected routes.

6. dotenv
Used to manage secret information (like database passwords and secret keys) through environment variables.

7. Swagger
Generates interactive API documentation so developers can easily test and understand the API.

🧩 How the Project is Structured
Controllers: Contain functions that handle the logic for each route (e.g., register a user, add a product).

Routes: Define the URLs available to users and which controller to use.

Models: Define the structure of the data stored in the database (users, products).

Middlewares: Handle tasks like checking if a user is authenticated before accessing certain routes.

Config: Contains the code to connect to the MongoDB database.

Swagger: Handles the setup of interactive API documentation.

🔐 User Authentication
Users must first register with a username and password. Upon login, the server provides a JWT token, which must be included in future requests to prove the user is authorized.

📦 Product Management
Once logged in, users can:

Add new products (name, quantity, etc.)

Update product quantities

View all products with options to filter pages (pagination)

🧪 How to Test the API
This project includes a Postman collection, which is a file that can be imported into Postman to test all the features step-by-step. Postman is a tool for sending HTTP requests without needing a frontend.

📘 API Documentation with Swagger
Swagger provides an interactive interface to test the API from the browser. After running the server, developers can visit a URL (usually /api-docs) to see all available endpoints, fill in data, and try out the features.

📝 Summary
This Inventory Management System backend provides a foundational example of how to:

Build an API with Express

Secure routes with JWT

Interact with a MongoDB database

Write organized and maintainable backend code