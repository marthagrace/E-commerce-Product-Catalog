🛒 E-commerce Product Catalog - RESTful API
A Spring Boot-based RESTful API to manage an e-commerce product catalog. This project supports product listing, searching, filtering, and secure access using Spring Security.

📌 Problem Statement
E-commerce Product Catalog
Create a RESTful API to manage an e-commerce product catalog. The API should support product listing, filtering by category or price, and searching by product name.

🎯 Objectives
Develop a secure REST API for product management.
Implement CRUD operations for products using Spring Data JPA and MySQL.
Provide filtering and search functionality.
Secure the API using Spring Security.

🧾 Requirements
📦 Product Entity:
productId: Long
name: String
description: String
price: Double
category: String
stockQuantity: Integer

🌐 API Endpoints:
POST /products – Add a product
GET /products – Get all products
GET /products/{id} – Get product by ID
PUT /products/{id} – Update product
DELETE /products/{id} – Delete product
GET /products/search?name=xyz – Search by product name
GET /products/filter?category=Electronics&minPrice=100&maxPrice=1000 – Filter products

🔒 Security
Role-based access control using Spring Security
ADMIN can add/update/delete
USER can view/search/filter
Basic Authentication (username & password)

🧪 Tech Stack
Java 17
Spring Boot
Spring Data JPA
MySQL
Spring Security
Lombok
Maven

🗃️ Database Configuration
Update your application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

🧑‍💻 Users
Seeded users (example for testing):

Username	Password	Role
admin	admin123	ADMIN
user	user123	USER

📦 Running the Project
Clone the repository:
git clone https://github.com/DivyaAdabala07/ecommerce-product-catalog.git
Navigate to the folder:
cd ecommerce-product-catalog
Run the project:
mvn spring-boot:run

📬 API Testing Tools
Postman
Curl
Swagger UI (Optional setup)

📃 License
This project is open source and available under the MIT License.

🙋‍♀️ Author
Adabala Divya Sai Suseela
