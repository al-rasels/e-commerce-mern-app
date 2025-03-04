

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

🔗 **Live Demo:** *[<img src="https://github.com/al-rasels/techo-fullstack-mern-app/blob/main/Techo.png" >](https://techo-on-live-app.onrender.com)*  




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

# **API Endpoints with Descriptions**  

## **1. Products**  
- **GET** `/ProductBrandList` – Retrieve a list of all available product brands.  
- **GET** `/ProductCategoryList` – Retrieve a list of all product categories.  
- **GET** `/ProductSliderList` – Fetch featured products for the homepage slider.  
- **GET** `/ProductListByBrand/:brandID` – Get products filtered by a specific brand.  
- **GET** `/ProductListByCategory/:categoryID` – Get products filtered by a specific category.  
- **GET** `/ProductListBySimilar/:categoryID` – Retrieve similar products based on category.  
- **GET** `/ProductListByKeyword/:keyword` – Search products using keywords.  
- **GET** `/ProductListByRemark/:remark` – Fetch products based on specific remarks (e.g., "new arrivals").  
- **GET** `/ProductDetails/:productID` – Get detailed information about a specific product.  
- **POST** `/ProductListByFilter` – Retrieve products filtered by brand, category, and price range.  

## **2. User Authentication & Profile**  
- **GET** `/UserOTP/:email` – Send a one-time password (OTP) to the user’s email for authentication.  
- **GET** `/VerifyLogin/:email/:otp` – Verify OTP and authenticate the user.  
- **GET** `/UserLogout` – Log the user out of the system.  
- **GET** `/ReadProfile` – Retrieve the user’s profile details.  
- **POST** `/CreateProfile` – Create a new user profile with personal and shipping details.  
- **POST** `/UpdateProfile` – Update the user’s profile information.  

## **3. Wishlist**  
- **POST** `/SaveWishList` – Add a product to the user’s wishlist.  
- **POST** `/RemoveWishList` – Remove a product from the wishlist.  
- **GET** `/WishList` – Retrieve all items saved in the user’s wishlist.  

## **4. Cart**  
- **POST** `/SaveCartList` – Add a product to the shopping cart with quantity and other details.  
- **POST** `/UpdateCartList/:cartID` – Update an item’s details in the cart (e.g., quantity, color, size).  
- **POST** `/RemoveCartList` – Remove a product from the cart.  
- **GET** `/CartList` – Retrieve all products currently in the cart.  

## **5. Orders & Invoices**  
- **GET** `/CreateInvoice` – Generate an order invoice after checkout.  
- **GET** `/InvoiceList` – Retrieve a list of all invoices for the user.  
- **GET** `/InvoiceProductList/:invoiceID` – Get a list of products included in a specific invoice.  

## **6. Features & Legal**  
- **GET** `/FeaturesList` – Retrieve details about the app’s features.  
- **GET** `/LegalDetails/:type` – Fetch legal information such as "how to buy" or return policies.  

## **7. Reviews**  
- **POST** `/CreateReview` – Submit a review for a purchased product.  
- **GET** `/ProductReviewList/:productID` – Retrieve all reviews for a specific product.  

This structured list provides clear descriptions of each endpoint. Let me know if you need any modifications.

For detailed information on request and response structures, refer to the API documentation or the source code.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## License

