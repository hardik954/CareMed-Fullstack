# Caremed – Full Stack Project Setup Guide

> Run Backend first →  Then Admin Panel → Then Frontend 

---

## ✅ Requirements
- Node.js installed
- MongoDB Atlas account
- Cloudinary account
- (Optional) Stripe / Razorpay accounts

---

Open the project in VS Code

Right-click on backend folder → Open in Integrated Terminal

Install dependencies:
npm install

Create a .env file inside the backend folder and add:

 <!--Currency-->
CURRENCY="INR"

 <!--JWT Secret (change this to a secure random value)-->
JWT_SECRET="your_jwt_secret_here"

 <!--Admin Panel Credentials-->
ADMIN_EMAIL="your_admin_email_here"
ADMIN_PASSWORD="your_admin_password_here"

<!-- MongoDB Setup (required)-->
MONGODB_URI="your_mongodb_connection_string_here"

<!-- Cloudinary Setup (required)-->
CLOUDINARY_NAME="your_cloudinary_name_here"
CLOUDINARY_API_KEY="your_cloudinary_api_key_here"
CLOUDINARY_SECRET_KEY="your_cloudinary_secret_key_here"

<!-- Razorpay Payment Integration (optional)-->
(Optional)
RAZORPAY_KEY_ID="your_razorpay_key_id_here"
RAZORPAY_KEY_SECRET="your_razorpay_key_secret_here"

<!-- Stripe Payment Integration (optional)-->
STRIPE_SECRET_KEY="your_stripe_secret_key_here"

# Admin Panel Setup
Create .env file and add:
VITE_CURRENCY = '₹'
VITE_BACKEND_URL = 'http://localhost:4000'

Right-click admin folder → Open in Integrated Terminal

Install dependencies:
npm install

Start admin panel:
npm run dev

Open in browser:
http://localhost:5174

# Frontend Setup
Create .env file and add:
VITE_BACKEND_URL = 'http://localhost:4000'
VITE_RAZORPAY_KEY_ID = '------ Razorpay Key Id here ------'(Optional)

Right-click frontend folder → Open in Integrated Terminal

Install dependencies:
npm install

Start frontend:
npm run dev

Open in browser:
http://localhost:5173


# Important Notes

Backend must be running before frontend or admin

Do not expose .env file publicly

Restart terminal if commands fail

If you begin directly in Admin Panel and not on the login page,
simply logout first and then login using your defined credentials.

