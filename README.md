# Point of Sale (POS) System

A comprehensive e-commerce platform built with React, Node.js, and MongoDB, featuring PayPal integration and advanced search capabilities.

## Live Demo
- **Deployed Site**: [https://ecom-kosr.onrender.com/](https://ecom-kosr.onrender.com/)
- **GitHub Repository**: [https://github.com/s11saurabh/QEST_POS_ASSIGNMENT](https://github.com/s11saurabh/QEST_POS_ASSIGNMENT)
<img width="1469" alt="image" src="https://github.com/user-attachments/assets/8416ac05-c58d-415c-a940-58485cd27f01" />
<img width="1470" alt="image" src="https://github.com/user-attachments/assets/d9513542-3d29-4a1e-a5eb-500fe0235ed7" />
<img width="1470" alt="image" src="https://github.com/user-attachments/assets/f8a7e6c1-69fa-474b-80fe-5cd9c985f008" />
<img width="1470" alt="image" src="https://github.com/user-attachments/assets/4a86898a-e37c-4da1-b9b0-8ee82f7b1d47" />
<img width="1470" alt="image" src="https://github.com/user-attachments/assets/6a36c388-d9b0-4426-9437-ef0d70de1a17" />


## Features

### Authentication & Authorization
- JWT-based authentication system
- Role-based access control (Admin/User)
- Secure password hashing
- Protected routes and API endpoints

### Shopping Experience
- Advanced product filtering:
  - Category-based (Fashion, Footwear, Watches, Guitar)
  - Price ranges ($0-19, $20-39, $40-59, $60-79, $80-99, $100+)
- Shopping cart functionality
- Secure PayPal payment integration
- Product search functionality
- Responsive user interface

### Admin Dashboard
- Product management
- Order tracking
- User management
- Sales analytics
- Inventory control

## Tech Stack
- **Frontend**: React.js, JavaScript, CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT
- **Payment**: PayPal API
- **Deployment**: Render

## Project Structure
```
├── config/
├── controllers/
├── helpers/
├── middlewares/
├── models/
├── public/
├── routes/
├── README.md
├── package.json
├── package-lock.json
└── server.js
```

## Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/s11saurabh/QEST_POS_ASSIGNMENT.git
cd QEST_POS_ASSIGNMENT
```

2. Install dependencies:
```bash
npm install
```

3. Create a .env file with required environment variables:
```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PAYPAL_CLIENT_ID=your_paypal_client_id
```

4. Start the development server:
```bash
npm run dev
```

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get single product
- `POST /api/products` - Add new product (Admin)
- `PUT /api/products/:id` - Update product (Admin)
- `DELETE /api/products/:id` - Delete product (Admin)

### Cart & Orders
- `GET /api/cart` - Get user's cart
- `POST /api/cart/add` - Add item to cart
- `POST /api/orders` - Create new order
- `GET /api/orders` - Get user's orders

## Security Features
- CORS protection
- XSS prevention
- Rate limiting
- Input validation
- Secure password storage
- Protected API endpoints

## Contributing
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License
MIT License

## Contact
For support or queries, please create an issue in the GitHub repository.
