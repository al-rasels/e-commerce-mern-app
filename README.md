

### **Full-Stack E-Commerce Application (MERN Stack)**  
🚀 **Overview:**  
Developed a dynamic and fully functional **MERN Stack E-Commerce Application** that allows users to seamlessly browse, search, filter, and purchase products. The platform features a smooth user experience with authentication, cart management, wishlist functionality, and an integrated review system.  

🔹 **Key Features:**  
- 🔍 **Product Search & Filtering** – Search by **brand** and **category**; filter products by **price range, brand, and category**.  
- 🛍️ **Product Details & Cart** – View product details, **add to cart** or **wishlist**, and proceed to checkout.  
- ✅ **User Authentication & Authorization** – Secure **email verification via OTP**, login/logout, and profile updates.  
- 🚚 **Order & Delivery Management** – Users can add delivery addresses and place orders effortlessly.  
- ⭐ **Review & Rating System** – Customers can leave reviews after purchasing.  

💡 **Tech Stack:**  
- **Frontend:** React.js, React-Bootstrap, Zustand (State Management), SweetAlert, and other UI libraries.  
- **Backend:** Node.js, Express.js, JWT, Mongoose, MongoDB, and essential backend tools.  

🎯 **Outcome:**  
Successfully built a **scalable and responsive** e-commerce platform with **secure authentication, real-time updates**, and a **user-friendly shopping experience**.  

🔗 **GitHub Repository / Live Demo:** *(https://techo-on-live-app.onrender.com)*  

<img src="techo.png">
---

This version is polished, professional, and LinkedIn-ready. Let me know if you'd like to tweak anything! 🚀

## Getting Started

### Prerequisites

Ensure you have the following installed on your system:

- **Node.js**: [Download and install](https://nodejs.org/).
- **MongoDB**: [Download and install](https://www.mongodb.com/try/download/community).

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/shant0786/e-commerce-mern-app.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd e-commerce-mern-app
   ```

3. **Install dependencies**:

   ```bash
   npm install
   ```

### Configuration

1. **Environment Variables**:

   Create a `.env` file in the root directory and add the following variables:

   ```env
   PORT=8000
   MONGO_URI=mongodb://localhost:27017/ecommerce
   JWT_SECRET=your_jwt_secret
   ```

   Replace `your_jwt_secret` with a secure secret key of your choice.

### Seeding the Database

To populate the database with initial data, run:

```bash
npm run seed
```

This will add sample users, products, and other necessary data to your MongoDB database.

### Running the Application

Start the development server with:

```bash
npm run dev
```

The server will run on `http://localhost:8000`.

## API Endpoints

The API provides the following endpoints:

- **User Routes**:
  - `POST /api/users/register`: Register a new user.
  - `POST /api/users/login`: Authenticate a user.
  - `GET /api/users/profile`: Retrieve user profile (requires authentication).

- **Product Routes**:
  - `GET /api/products`: Retrieve all products.
  - `GET /api/products/:id`: Retrieve a single product by ID.
  - `POST /api/products`: Create a new product (admin only).
  - `PUT /api/products/:id`: Update a product by ID (admin only).
  - `DELETE /api/products/:id`: Delete a product by ID (admin only).

- **Order Routes**:
  - `POST /api/orders`: Create a new order.
  - `GET /api/orders/:id`: Retrieve order by ID.
  - `GET /api/orders/user/:userId`: Retrieve orders for a specific user.
  - `PUT /api/orders/:id`: Update order status (admin only).

- **Cart Routes**:
  - `GET /api/cart`: Retrieve user's cart.
  - `POST /api/cart`: Add item to cart.
  - `PUT /api/cart/:itemId`: Update cart item quantity.
  - `DELETE /api/cart/:itemId`: Remove item from cart.

- **Wishlist Routes**:
  - `GET /api/wishlist`: Retrieve user's wishlist.
  - `POST /api/wishlist`: Add item to wishlist.
  - `DELETE /api/wishlist/:itemId`: Remove item from wishlist.

- **Review Routes**:
  - `POST /api/products/:id/reviews`: Add a review to a product.
  - `GET /api/products/:id/reviews`: Retrieve reviews for a product.

For detailed information on request and response structures, refer to the API documentation or the source code.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## License

