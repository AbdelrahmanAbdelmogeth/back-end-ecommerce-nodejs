# E-Commerce Backend - Features & Functionalities  

## 0. Project Overview  
This backend application powers a complete e-commerce platform, handling product management, user authentication, order processing, payments, and more. It is built with **Node.js, Express.js, and MongoDB**, following best practices for security, scalability, and performance.  

## 1. Installation & Setup  

### **Prerequisites**  
Make sure you have the following installed:  
- **Node.js** (>= 16.x)  
- **MongoDB** (local or cloud, e.g., MongoDB Atlas)  
- **Git**  

### **Clone the Repository**  
```sh
git clone https://github.com/AbdelrahmanAbdelmogeth/back-end-ecommerce-nodejs.git
cd back-end-ecommerce-nodejs
```

### **Install Dependencies**
```sh
npm install
```

### **Environment Variables**
Create a config.env file in the root directory and add the following:
```
NODE_ENV=development
PORT=8000

BASE_URL=http://127.0.0.1:8000



DB_URI="mongodb://127.0.0.1:27017/ecommerce"

# JWT OPTIONS
JWT_SECRET=this-is-my-random-jwt-secret
JWT_EXPIRES_IN=90d

# EMAIL SETTINGS
EMAIL_USERNAME=abdelrahman@gmail.com
EMAIL_PASSWORD=In@in2016
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=465


# STRIPE CONFIG
STRIPE_SECRET_KEY=<put your key here>
STRIPE_WEBHOOK_SECRET=<put your key here>
```

### **Run the Development Server**
```
sh
npm run start:dev
```
The server will start on http://localhost:8000.

### **Run in Production Mode**
```
sh
npm start
```

## 2. Core Functionalities  

### 📌 **System & Environment Setup**  
- Setting up the development environment with required tools and dependencies.  
- Configuring Express.js as the backend framework.  
- Connecting to MongoDB for database operations.  

### 📌 **Categories & Subcategories Management**  
- CRUD operations (Create, Read, Update, Delete) for **categories** (e.g., Clothing, Electronics).  
- CRUD operations for **subcategories**, allowing hierarchical classification.  

### 📌 **Brand & Product Management**  
- CRUD operations for **brands**.  
- Full product management:  
  - Add, update, delete, and fetch products.  
  - Implement **search, filtering, and sorting** (by price, popularity, etc.).  
  - Relate products to categories and brands.  

### 📌 **Image Upload & Processing**  
- Upload single or multiple product images.  
- Image optimization for better performance.  
- Validation to restrict file uploads to images only.  

### 📌 **User Authentication & Authorization**  
- **User registration & login** with password hashing.  
- **Token-based authentication** (JWT).  
- Password recovery and reset functionality.  
- Role-based access control (Admin, Manager, User).  

### 📌 **User Features**  
- **Product reviews & ratings**:  
  - Users can leave reviews and rate products.  
  - Calculate **average ratings** and **total reviews** for each product.  
- **Wishlist management**:  
  - Users can add/remove products from their wishlist.  
- **Address management**:  
  - Users can save multiple delivery addresses.  

### 📌 **Shopping Cart & Checkout**  
- Users can **add, update, and remove products** in their cart.  
- Stock validation to prevent over-purchasing.  
- **Apply discount coupons** for order total reduction.  

### 📌 **Order Processing & Payments**  
- **Order creation & tracking**.  
- **Payment gateway integration** for online payments (e.g., Apple Pay, Stripe).  
- Support for **cash-on-delivery** orders.  
- Validate and confirm successful payments before finalizing an order.  

### 📌 **Advanced Error Handling & Validation**  
- Centralized error handling for API responses.  
- Input validation to ensure data integrity.  
- Catching and managing errors beyond Express.js.  

### 📌 **Security Enhancements**  
- Protect API routes with authentication and authorization.  
- Secure password handling with hashing.  
- Implement best practices to prevent vulnerabilities.  

---

This backend efficiently manages the core functionalities of an e-commerce system, ensuring a smooth and scalable experience for users. 🚀  
