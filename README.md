# Railway Management System

A comprehensive full-stack web application for managing railway operations, built with the SERN stack (SQL, Express, React, Node.js). This system provides end-to-end functionality for train booking, seat management, and passenger operations.

## 🚀 Features

- **User Authentication**: Secure JWT-based authentication system with session management
- **Train Search & Booking**: Real-time train search with availability checking across 10 different classes
- **Seat Management**: Dynamic seat allocation and availability tracking
- **Passenger Management**: Complete passenger information handling with booking history
- **Payment Integration**: Automated billing system with tax calculation and concession management
- **Admin Dashboard**: Comprehensive admin panel for train and route management
- **Responsive Design**: Mobile-friendly interface with modern UI components

## 🛠️ Tech Stack

- **Frontend**: React.js, HTML5, CSS3, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Authentication**: JWT (JSON Web Tokens)
- **API**: RESTful architecture with 15+ endpoints

## 📊 Project Statistics

- **Database Tables**: 6 interconnected tables (passengers, trains, routes, seats, tickets, status)
- **API Endpoints**: 15+ RESTful endpoints
- **Server Code**: 632 lines of Express.js code
- **Frontend Components**: 13+ responsive React components
- **Train Classes**: 10 different booking classes supported

## 🏗️ Database Architecture

├── passengers (user information)
├── trains (train details and schedules)
├── routes (route information and stations)
├── seats (seat allocation and availability)
├── tickets (booking records)
└── status (booking status tracking)


## 🚀 Installation

### Prerequisites

- Node.js (v14 or higher)
- MySQL (v8.0 or higher)
- npm or yarn package manager

### Setup Instructions

1. **Clone the repository**
git clone https://github.com/ARU5H/Railway-Management-System.git
cd Railway-Management-System


2. **Install dependencies**
Install backend dependencies
npm install
Install frontend dependencies
cd client
npm install


3. **Database Setup**
Create MySQL database
mysql -u root -p
CREATE DATABASE railway_management;
Import database schema
mysql -u root -p railway_management < database/schema.sql


4. **Environment Configuration**
Create .env file in root directory
cp .env.example .env
Configure database connection
DB_HOST=localhost
DB_USER=your_username
DB_PASSWORD=your_password
DB_NAME=railway_management
JWT_SECRET=your_jwt_secret


5. **Start the Application**
Start backend server
npm run server
Start frontend (in new terminal)
cd client
npm start


## 📖 Usage

### For Users
1. **Registration**: Create an account with personal details
2. **Login**: Authenticate using email and password
3. **Search Trains**: Enter source, destination, and travel date
4. **Book Tickets**: Select train, class, and seats
5. **Payment**: Complete booking with integrated payment system
6. **View Bookings**: Check booking history and status

### For Administrators
1. **Train Management**: Add, update, and remove trains
2. **Route Management**: Configure routes and stations
3. **Seat Management**: Monitor seat availability and allocations
4. **User Management**: View and manage user accounts
5. **Reports**: Generate booking and revenue reports

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Train Operations
- `GET /api/trains` - Get all trains
- `GET /api/trains/search` - Search trains by route and date
- `POST /api/trains` - Add new train (Admin)
- `PUT /api/trains/:id` - Update train details (Admin)

### Booking System
- `POST /api/bookings` - Create new booking
- `GET /api/bookings/:userId` - Get user bookings
- `PUT /api/bookings/:id` - Update booking status
- `DELETE /api/bookings/:id` - Cancel booking

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Arush Singh Kiron**
- GitHub: [@ARU5H](https://github.com/ARU5H)
- LinkedIn: [Arush Singh Kiron](https://www.linkedin.com/in/arush-singh-kiron-a27387339/)
- Email: arush.singhkiron@gmail.com

## 🙏 Acknowledgments

- Express.js team for the robust backend framework
- React.js community for the excellent frontend library
- MySQL team for the reliable database system
- IIT Patna for the learning environment and resources

---

**Note**: This project was developed as part of academic coursework to demonstrate full-stack web development skills and database management capabilities.
