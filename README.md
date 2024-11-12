# Eazy-Buy-Ecommerce_website_2024
Easy-Buy E-commerce Web Application
Overview
Easy-Buy is a fully-functional e-commerce web application built using the MERN stack (MongoDB, Express, React, and Node.js). The application provides a user-friendly interface for browsing products, adding items to the cart, and completing purchases. Admin functionalities allow for product management, including adding, updating, and deleting items.

Features
User Features
User Authentication: Sign up, login, and logout with JWT-based authentication.
Product Browsing: View a list of products with filtering and sorting options.
Product Details: Detailed view of each product, including description, images, price, and reviews.
Shopping Cart: Add, update, and remove products in the shopping cart.
Checkout: Complete the purchase with an order summary and payment gateway integration.
Order History: View past orders with status and delivery tracking.
Admin Features
Product Management: Add new products, edit existing ones, and remove products from inventory.
Order Management: View and manage customer orders.
User Management: Manage registered users and their roles.
Dashboard: Insights into sales and customer activity.
Technologies Used
Frontend: React, Redux (for state management), Bootstrap for responsive design
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JWT (JSON Web Tokens)
Payment Gateway: [Integrate with payment provider, e.g., Stripe/PayPal]
Hosting: [Frontend and Backend Hosting Platforms, e.g., Heroku, Vercel]
Installation Guide
Prerequisites
Node.js and npm installed
MongoDB database running locally or on a cloud provider like MongoDB Atlas
Steps to Install
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/easy-buy.git
cd easy-buy
Install Backend Dependencies:

bash
Copy code
cd backend
npm install
Set up Environment Variables:

Create a .env file in the backend directory.
Add the following keys:
env
Copy code
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
Run the Backend Server:

bash
Copy code
npm run server
Install Frontend Dependencies:

bash
Copy code
cd ../frontend
npm install
Run the Frontend Server:

bash
Copy code
npm start
Visit the Application: Open http://localhost:3000 in your browser.

Folder Structure
backend: Contains Express server, database models, controllers, routes, and configuration files.
frontend: Contains the React application with components, pages, Redux store, and styles.
API Endpoints
User Routes
POST /api/users/register: Register a new user
POST /api/users/login: Authenticate a user and return a JWT
Product Routes
GET /api/products: Get a list of all products
GET /api/products/:id: Get details of a specific product
Cart and Order Routes
POST /api/cart: Add items to the user's cart
POST /api/orders: Place an order
GET /api/orders/user/:userId: Get user order history
Admin Routes (Requires Admin Role)
POST /api/admin/products: Add a new product
PUT /api/admin/products/:id: Update product information
DELETE /api/admin/products/:id: Delete a product
