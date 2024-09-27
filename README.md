# Inventory Management System

## Overview

This Inventory Management System is a robust backend application built with the MERN stack (MongoDB, Express, React, Node.js). It provides a secure and scalable solution for managing product inventories, with features including user authentication, product upload and management, and admin review processes.

## Features

- User registration and authentication
- JWT-based authorization
- Product upload with image storage (AWS S3)
- Admin dashboard for product review and management
- RESTful API architecture
- Input validation and error handling
- Pagination and search functionality
- Comprehensive logging
- Unit testing
- API documentation with Swagger/OpenAPI

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js (v14 or later)
- MongoDB
- AWS account with S3 bucket set up

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/inventory-management-system.git
   cd inventory-management-system
   ```

2. Install the dependencies:
   ```
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the following:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   AWS_ACCESS_KEY_ID=your_aws_access_key_id
   AWS_SECRET_ACCESS_KEY=your_aws_secret_access_key
   AWS_S3_BUCKET_NAME=your_s3_bucket_name
   ```

## Usage

To run the server in development mode:
```
npm run dev
```

To run the server in production mode:
```
npm start
```

To run tests:
```
npm test
```

## API Documentation

Once the server is running, you can access the Swagger API documentation at:
```
http://localhost:5000/api-docs
```

## Main Endpoints

- POST `/api/auth/register`: Register a new user
- POST `/api/auth/login`: Authenticate a user
- POST `/api/products/upload`: Upload a new product (authenticated users only)
- GET `/api/products`: Get list of published products (with pagination and search)
- GET `/api/admin/products`: Get list of products pending review (admin only)
- PUT `/api/admin/products/:id/approve`: Approve a product (admin only)
- PUT `/api/admin/products/:id/reject`: Reject a product (admin only)

## Contributing

Contributions to the Inventory Management System are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Your Name - sahilsuman1202@gmail.com

Project Link: [https://github.com/your-username/inventory-management-system](https://github.com/your-username/inventory-management-system)

## Acknowledgements

- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [JSON Web Tokens](https://jwt.io/)
- [AWS SDK](https://aws.amazon.com/sdk-for-javascript/)
- [Jest](https://jestjs.io/)
- [Swagger](https://swagger.io/)
