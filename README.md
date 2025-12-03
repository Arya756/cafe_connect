# ☕ CafeConnect

A modern, full-stack cafe management platform where cafes can manage their menu and customers can browse and order items seamlessly.

![CafeConnect](https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?w=1200&h=400&fit=crop)

## 🌟 Features

### For Customers
- 🔐 **User Authentication** - Secure signup and login
- 📱 **Browse Menu** - View available items with beautiful images
- 🛒 **Shopping Cart** - Add items and manage quantities
- 📦 **Order Tracking** - View order status and history
- ⚡ **Real-time Updates** - Instant order status notifications

### For Admins
- 👨‍💼 **Admin Dashboard** - Manage all cafe operations
- 📋 **Menu Management** - Add, edit, delete menu items
- 🔄 **Order Management** - View and update order status
- ⏱️ **Estimated Wait Time** - Set delivery estimates for orders
- 📊 **Order Overview** - Track all orders in one place

## 🛠️ Tech Stack

### Frontend
- **React** - UI library
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations
- **React Router** - Navigation

### Backend
- **Node.js** - Runtime
- **Express** - Web framework
- **JWT** - Authentication
- **bcrypt** - Password hashing
- **Mock Data** - In-memory storage (demo mode)

### Deployment
- **Frontend**: Vercel
- **Backend**: Render
- **Database**: Mock data (in-memory)

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ installed
- npm or yarn package manager

### Local Development

1. **Clone the repository**
```bash
git clone https://github.com/Arya756/cafe_connect.git
cd cafe_connect
```

2. **Install dependencies**
```bash
# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

3. **Start the backend**
```bash
cd server
node server.js
```
Backend runs on `http://localhost:5001`

4. **Start the frontend**
```bash
cd client
npm run dev
```
Frontend runs on `http://localhost:5173`

## 🔑 Demo Credentials

### Admin Account
- **Email**: `admin@cafe.com`
- **Password**: `admin123`

### User Account
- **Email**: `user@test.com`
- **Password**: `user123`

## 📁 Project Structure

```
cafe_connect/
├── client/                 # Frontend React app
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Page components
│   │   ├── context/       # React Context (Auth, Cart)
│   │   └── services/      # API service layer
│   └── public/
├── server/                # Backend Express app
│   ├── controllers/       # Route controllers
│   ├── routes/           # API routes
│   ├── mockData.js       # In-memory data store
│   └── server.js         # Entry point
└── README.md
```

## 🌐 Live Demo

- **Frontend**: [https://cafe-connect-pi.vercel.app/](https://cafe-connect-pi.vercel.app/)
- **Backend API**: [https://cafe-connect-q1c7.onrender.com/api](https://cafe-connect-q1c7.onrender.com/api)

## 📝 API Endpoints

### Authentication
- `POST /api/auth/signup` - Register new user
- `POST /api/auth/login` - Login user

### Menu
- `GET /api/menu` - Get all menu items
- `POST /api/menu` - Create menu item (admin)
- `PUT /api/menu/:id` - Update menu item (admin)
- `DELETE /api/menu/:id` - Delete menu item (admin)

### Orders
- `POST /api/orders` - Place order
- `GET /api/orders/user/:userId` - Get user orders
- `GET /api/orders/all` - Get all orders (admin)
- `PUT /api/orders/:id` - Update order status (admin)

## 🎨 Screenshots

### Landing Page
Beautiful landing page with animated food elements and smooth transitions.

### User Dashboard
Browse menu items by category with real-time cart updates.

### Admin Dashboard
Manage menu items and orders with an intuitive interface.

## ⚠️ Important Notes

> **Demo Mode**: This project uses in-memory mock data for fast performance during demos. Data resets on server restart.

> **Production Use**: For production, replace `mockData.js` with a real database (MySQL, PostgreSQL, MongoDB).

## 🔄 Switching to Database Mode

To use a real database instead of mock data:

1. Uncomment database code in `server/server.js`
2. Set up database credentials in `server/.env`
3. Update controllers to use Sequelize models
4. Run database migrations

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Ayush Aryan**
- GitHub: [@Arya756](https://github.com/Arya756)

## 🙏 Acknowledgments

- Images from [Unsplash](https://unsplash.com/)
- Icons from [Heroicons](https://heroicons.com/)
- UI inspiration from modern cafe websites

---

Made with ☕ and ❤️ by Ayush Aryan
