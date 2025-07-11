# Car Repair Management System

A comprehensive car repair management system built with the MERN stack (MongoDB, Express.js, React.js, Node.js). This application allows users to manage car repairs, purchase parts, and handle vehicle replacement services.

## Features

### 🔧 Repair Management
- Schedule and track car repairs
- Assign mechanics to repair jobs
- Monitor repair progress and status
- Generate repair estimates and invoices

### 🛒 Parts Management
- Browse available car parts catalog
- Search parts by car model, brand, or part type
- Add parts to cart and purchase
- Track inventory and stock levels
- Manage suppliers and part orders

### 🚗 Vehicle Services
- Vehicle registration and management
- Car replacement services
- Vehicle history tracking
- Service appointment scheduling

### 👥 User Management
- Customer registration and profiles
- Mechanic accounts and specializations
- Admin dashboard for system management
- Role-based access control

## Tech Stack

**Frontend:**
- React.js
- Tailwind CSS
- React Router
- Axios for API calls

**Backend:**
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Bcrypt for password hashing

**Additional Tools:**
- Vite (Build tool)
- ESLint (Code linting)
- PostCSS (CSS processing)

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ariful129/Car-doctor-client.git
   cd Car-doctor-client
   ```

2. **Install dependencies**
   ```bash
   # Install frontend dependencies
   npm install
   
   # Install backend dependencies (if separate folder)
   cd server
   npm install
   ```

3. **Environment Variables**
   Create a `.env` file in the root directory:
   ```env
   MONGODB_URI=mongodb://localhost:27017/car-repair-db
   JWT_SECRET=your-jwt-secret-key
   PORT=5000
   REACT_APP_API_URL=http://localhost:5000/api
   ```

4. **Start the application**
   ```bash
   # Start backend server
   npm run server
   
   # Start frontend (in new terminal)
   npm run dev
   ```

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Repairs
- `GET /api/repairs` - Get all repairs
- `POST /api/repairs` - Create new repair
- `PUT /api/repairs/:id` - Update repair status
- `DELETE /api/repairs/:id` - Delete repair

### Parts
- `GET /api/parts` - Get all parts
- `POST /api/parts` - Add new part
- `PUT /api/parts/:id` - Update part
- `DELETE /api/parts/:id` - Delete part

### Orders
- `POST /api/orders` - Create new order
- `GET /api/orders/user/:userId` - Get user orders
- `PUT /api/orders/:id/status` - Update order status

## Project Structure

```
car-repair-system/
├── public/
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   ├── Dashboard/
│   │   ├── Parts/
│   │   ├── Repairs/
│   │   └── Common/
│   ├── pages/
│   ├── hooks/
│   ├── services/
│   ├── utils/
│   └── App.jsx
├── server/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── controllers/
│   └── server.js
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

**Developer:** Ariful Islam  
**Email:** [your-email@example.com]  
**GitHub:** [@Ariful129](https://github.com/Ariful129)

## Acknowledgments

- Thanks to all contributors
- Inspired by modern car service management systems
- Built with love for the automotive industry

---

⭐ **If you find this project helpful, please give it a star!**
