

# CourseHub

CourseHub is a comprehensive online ed-tech platform where students can purchase and filter courses, while instructors can create, edit, and manage their courses. This project leverages the MERN stack and integrates Razorpay for seamless payment processing.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Razorpay Integration](#razorpay-integration)

## Features

- **User Authentication:** Secure login and registration for students and instructors.
- **Course Management:** Instructors can create, edit, and manage their courses.
- **Course Purchase:** Students can purchase courses using Razorpay.
- **Course Filtering:** Students can filter courses based on various criteria.
- **Responsive Design:** Accessible on all devices for a seamless user experience.
- **Dashboard:** Personalized dashboards for both students and instructors.

## Technologies Used

- **Frontend:** React, Redux, HTML, CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Payment Gateway:** Razorpay
- **Authentication:** JWT (JSON Web Tokens)
- **Others:** Mongoose

## Setup and Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/CourseHub.git
    cd CourseHub
    ```

2. **Install dependencies for both frontend and backend:**
    ```sh
    # For backend
    cd backend
    npm install

    # For frontend
    cd ../frontend
    npm install
    ```

3. **Set up environment variables:**
    Create a `.env` file in the backend directory and add the following:
    ```env
    PORT=4000
    MONGO_URI=your_mongo_db_connection_string
    JWT_SECRET=your_jwt_secret
    RAZORPAY_KEY_ID=your_razorpay_key_id
    RAZORPAY_KEY_SECRET=your_razorpay_key_secret
    ```

4. **Run the application:**
    ```sh
    # For backend
    cd backend
    npm start

    # For frontend
    cd ../frontend
    npm start
    ```

    The frontend will be served on `http://localhost:3000` and the backend on `http://localhost:4000`.

## Usage

- **Students:**
  - Signu and log in to your account.
  - Browse and filter courses based on your preferences.
  - Purchase courses using Razorpay and access the course content.

- **Instructors:**
  - Register and log in to your account.
  - Create new courses and manage existing ones.
  - Edit course details, add content, and track student enrollments.
 
- **Admin:**
  - Creatings categories for courses. 

## Project Structure

```
CourseHub/
│
├── backend/              # Backend code
│   ├── controllers/      # Controllers for handling requests
│   ├── models/           # Mongoose models
│   ├── routes/           # Express routes
│   ├── middleware/       # Custom middleware
│   └── server.js         # Entry point for the backend
│
├── frontend/             # Frontend code
│   ├── public/           # Public assets
│   ├── src/
│   │   ├── components/   # React components
│   │   ├── pages/        # Page components
│   │   ├── redux/        # Redux setup
│   │   ├── utils/        # Utility functions
│   │   └── App.js        # Main App component
│   └── index.js          # Entry point for the frontend
│
└── README.md             # This README file
```

## Razorpay Integration

Razorpay is integrated to handle secure payment transactions. Ensure you have your Razorpay API keys set up in the `.env` file as mentioned above.

- **Creating an Order:**
  The backend API creates an order and sends the order ID to the frontend.
- **Processing Payment:**
  The frontend uses Razorpay's checkout script to handle the payment process.

## Contact

For any inquiries or feedback, please reach out to:

- **Name:** Ronak Sharma
- **Email:** ronaksharma.rk77@gmail.com
- **GitHub:** [ronakshama77](https://github.com/ronaksharma77)
