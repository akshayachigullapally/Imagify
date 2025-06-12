# Imagify

Imagify is a web application that allows users to generate stunning images from text prompts using AI-powered technology. Users can create, download, and share their generated images effortlessly. The application also includes a credit-based system for generating images and purchasing additional credits.

## Features

- **Text-to-Image Generation**: Transform text prompts into high-quality images.
- **User Authentication**: Secure login and registration system.
- **Credit System**: Users can generate images using credits and purchase additional credits via Razorpay.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **AI-Powered**: Powered by advanced AI technology for image generation.
- **Social Sharing**: Share generated images directly from the platform.

## Tech Stack

### Client
- **React**: Frontend framework for building user interfaces.
- **Vite**: Development environment for fast builds and HMR.
- **TailwindCSS**: Utility-first CSS framework for styling.
- **Axios**: HTTP client for API requests.
- **Framer Motion**: Animation library for React.
- **React Router**: Routing library for navigation.
- **React Toastify**: Notifications for user feedback.

### Server
- **Node.js**: Backend runtime environment.
- **Express**: Web framework for building APIs.
- **MongoDB**: Database for storing user and transaction data.
- **Mongoose**: ODM for MongoDB.
- **Razorpay**: Payment gateway for credit purchases.
- **JWT**: Authentication using JSON Web Tokens.
- **Bcrypt**: Password hashing for secure authentication.

## Installation

### Prerequisites
- Node.js and npm installed.
- MongoDB database setup.
- Razorpay account for payment integration.

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/imagify.git
   cd imagify

    ```
2. Set up the server:
   ```sh
   cd server
   npm install
   
Create a .env file in the server directory and add the following:
   ```sh
   MONGODB_URI=<your-mongodb-uri>
   JWT_SECRET=<your-jwt-secret>
   CLIPDROP_API=<your-clipdrop-api-key>
   RAZORPAY_KEY_ID=<your-razorpay-key-id>
   RAZORPAY_KEY_SECRET=<your-razorpay-key-secret>
   CURRENCY=INR

   ```
   Start the server:
   ```sh
   npm run server
   ```

3. Set up the client:
   ```sh
   cd ../client
   npm install

Create a .env file in the client directory and add the following:
   ```sh
   VITE_BACKEND_URL=http://localhost:4000
   VITE_RAZORPAY_KEY_ID=<your-razorpay-key-id>

   ```
   Start the client:
   ```sh
   npm run dev

```
Open the application in your browser at http://localhost:5173.



Folder Structure
```sh
imagify/
├── client/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   ├── index.css
│   ├── .env
│   ├── package.json
│   ├── vite.config.js
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── .env
│   ├── package.json
│   ├── server.js
   
