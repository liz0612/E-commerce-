# E-commerce-
## Demo Video

Watch the demo video on Google Drive: [Demo Video Link](https://drive.google.com/file/d/1a5uP69ZPcCrZEfqUOVP2DSf1oiX7U2lO/view?usp=sharing)
## Description
This is the back-end API for an e-commerce application built using **Node.js**, **Express.js**, **Sequelize**, and **MySQL**. It allows for the management of categories, products, and tags, and supports **CRUD** operations (Create, Read, Update, Delete). The database is seeded with sample data for testing purposes.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Testing](#testing)
- [License](#license)

## Installation

### Clone the Repository
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/liz0612/E-commerce-
   	2.	Navigate to the project directory:
   cd E-commerce-
   3.	Install the required dependencies:
   npm install
   4.	Create a .env file in the root directory and add the following variables:
   DB_NAME=ecommerce_db
DB_USER=[your MySQL username]
DB_PW=[your MySQL password]
	5.	Note: Ensure that you have MySQL installed and running on your machine.

Usage

Start the Server

To start the server, run: npm run start
The server will start and listen on port 3003 (or whatever port you’ve configured in server.js).

Seed the Database

If you want to seed your database with sample data, run: npm run seeds 
This will insert sample categories, products, and tags into your database.

Syncing Sequelize Models

When starting the application, the Sequelize models will automatically sync with the MySQL database.

API Routes

Categories
	•	GET /api/categories - Retrieve all categories.
	•	POST /api/categories - Create a new category.
	•	PUT /api/categories/:id - Update a category by ID.
	•	DELETE /api/categories/:id - Delete a category by ID.

Products
	•	GET /api/products - Retrieve all products.
	•	POST /api/products - Create a new product.
	•	PUT /api/products/:id - Update a product by ID.
	•	DELETE /api/products/:id - Delete a product by ID.

Tags
	•	GET /api/tags - Retrieve all tags.
	•	POST /api/tags - Create a new tag.
	•	PUT /api/tags/:id - Update a tag by ID.
	•	DELETE /api/tags/:id - Delete a tag by ID.

Product-Tag Associations
	•	GET /api/product_tags - Retrieve all product-tag associations.

Testing

You can test the API using Postman or Insomnia. Here are some basic examples:
	1.	Get All Categories:
	•	Method: GET
	•	URL: http://localhost:3003/api/categories
	2.	Create a New Category:
	•	Method: POST
	•	URL: http://localhost:3003/api/categories
	•	Body (raw, JSON): {
  "category_name": "Electronics"
}
	3.	Update a Category:
	•	Method: PUT
	•	URL: http://localhost:3003/api/categories/:id
	•	Body (raw, JSON): {
  "category_name": "Home Appliances"
}
	4.	Delete a Category:
	•	Method: DELETE
	•	URL: http://localhost:3003/api/categories/:id

License

This project is licensed under the MIT License - see the LICENSE file for details.
