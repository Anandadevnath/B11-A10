# 🏠 Roommate Finder

A modern, full-stack web application that helps users find compatible roommates and shared housing. Built with React, Node.js, and MongoDB, featuring a beautiful glassmorphism UI design.

![Roommate Finder](https://via.placeholder.com/800x400/1e293b/ffffff?text=Roommate+Finder+App)

## ✨ Features

### 🔐 Authentication & User Management
- **Firebase Authentication** with email/password and Google OAuth
- **Protected Routes** with private route implementation
- **Password Reset** functionality with email verification
- **User Profiles** with customizable information and photos

### 🏡 Roommate Listings
- **Create Listings** with detailed room information
- **Advanced Search & Filtering** by location, price, room type
- **Interactive Map Integration** for location visualization
- **Image Upload** with multiple photo support
- **Availability Status** tracking (Available/Occupied)

### 📊 Dashboard & Analytics
- **Personal Dashboard** with statistics and overview
- **My Listings Management** with CRUD operations
- **Platform Analytics** showing trends and insights
- **Recent Activity** tracking and notifications

### 💬 Communication & Social
- **Like System** for favorite listings
- **View Counting** to track listing popularity
- **Contact Information** for direct communication
- **User Reviews** and rating system

### 🎨 Modern UI/UX
- **Glassmorphism Design** with backdrop blur effects
- **Animated Backgrounds** with floating elements
- **Responsive Design** for all device sizes
- **Dark Theme** with purple/blue color scheme
- **Smooth Animations** and transitions

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks
- **React Router DOM** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **Firebase SDK** - Authentication and real-time features
- **SweetAlert2** - Beautiful alert modals
- **Axios** - HTTP client for API requests

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variable management

### Deployment & Tools
- **Frontend**: Netlify/Vercel
- **Backend**: Railway/Render
- **Database**: MongoDB Atlas
- **Version Control**: Git & GitHub

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- MongoDB Atlas account
- Firebase project setup

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/roommate-finder.git
   cd roommate-finder
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd frontend
   npm install
   ```

3. **Install Backend Dependencies**
   ```bash
   cd ../backend
   npm install
   ```

4. **Environment Setup**

   **Frontend (.env)**
   ```env
   REACT_APP_FIREBASE_API_KEY=your_firebase_api_key
   REACT_APP_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
   REACT_APP_FIREBASE_PROJECT_ID=your_firebase_project_id
   REACT_APP_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
   REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
   REACT_APP_FIREBASE_APP_ID=your_firebase_app_id
   REACT_APP_API_URL=http://localhost:5000
   ```

   **Backend (.env)**
   ```env
   MONGODB_URI=your_mongodb_connection_string
   PORT=5000
   NODE_ENV=development
   ```

5. **Run the Application**

   **Start Backend Server**
   ```bash
   cd backend
   npm start
   ```

   **Start Frontend Development Server**
   ```bash
   cd frontend
   npm start
   ```

6. **Open your browser**
   ```
   http://localhost:3000
   ```

## 📁 Project Structure

```
roommate-finder/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── NavBar/
│   │   │   ├── Footer/
│   │   │   ├── Login/
│   │   │   ├── Register/
│   │   │   ├── Dashboard/
│   │   │   ├── CreateRoom/
│   │   │   ├── AllItems/
│   │   │   ├── Support/
│   │   │   └── Contact/
│   │   ├── contexts/
│   │   │   └── AuthContext.js
│   │   ├── pages/
│   │   ├── utils/
│   │   └── App.js
│   ├── package.json
│   └── tailwind.config.js
├── backend/
│   ├── models/
│   │   ├── User.js
│   │   └── Roommate.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── roommates.js
│   │   └── analytics.js
│   ├── middleware/
│   ├── controllers/
│   ├── server.js
│   └── package.json
└── README.md
```

## 🎯 Key Features Overview

### 🔑 Authentication Flow
- **Register**: Create account with email/password or Google
- **Login**: Secure authentication with password reset option
- **Profile**: Manage user information and preferences
- **Logout**: Secure session management

### 🏠 Listing Management
- **Create**: Add new roommate listings with photos and details
- **Read**: Browse all available listings with filters
- **Update**: Edit your existing listings
- **Delete**: Remove listings with confirmation

### 📊 Dashboard Features
- **Overview**: Personal statistics and recent activity
- **All Items**: Browse platform listings
- **Add Item**: Quick access to create new listings
- **My Items**: Manage personal listings with table/card views

### 🎨 UI Components
- **Glassmorphism Cards**: Modern translucent design
- **Animated Backgrounds**: Dynamic floating elements
- **Responsive Grids**: Mobile-first responsive layouts
- **Interactive Elements**: Hover effects and smooth transitions

## 🌐 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Roommate Listings
- `GET /api/roommates` - Get all listings
- `POST /api/roommates` - Create new listing
- `GET /api/roommates/:id` - Get specific listing
- `PUT /api/roommates/:id` - Update listing
- `DELETE /api/roommates/:id` - Delete listing
- `PATCH /api/roommates/:id/like` - Like/unlike listing

### Analytics
- `GET /api/analytics` - Platform statistics
- `GET /api/dashboard/stats` - User dashboard stats

## 🎨 Design System

### Color Palette
- **Primary**: Purple (#8B5CF6) to Blue (#3B82F6)
- **Secondary**: Green (#10B981) to Emerald (#059669)
- **Accent**: Orange (#F59E0B) to Red (#EF4444)
- **Background**: Dark slate (#0F172A) to slate (#1E293B)

### Typography
- **Headers**: Bold gradient text effects
- **Body**: Clean, readable sans-serif
- **Interactive**: Smooth hover transitions

### Components
- **Glass Cards**: Backdrop blur with subtle borders
- **Buttons**: Gradient backgrounds with hover effects
- **Forms**: Consistent styling with validation states
- **Navigation**: Fixed navbar with smooth scrolling

## 🚀 Deployment

### Frontend (Netlify/Vercel)
1. Build the project: `npm run build`
2. Deploy the `build` folder
3. Configure environment variables
4. Set up custom domain (optional)

### Backend (Railway/Render)
1. Push code to GitHub
2. Connect repository to hosting service
3. Configure environment variables
4. Deploy with automatic builds

### Database (MongoDB Atlas)
1. Create cluster on MongoDB Atlas
2. Configure network access
3. Create database user
4. Get connection string

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Team

- **Your Name** - Full Stack Developer - [GitHub](https://github.com/yourusername)

## 🙏 Acknowledgments

- React community for excellent documentation
- Firebase for authentication services
- MongoDB for database solutions
- Tailwind CSS for utility-first styling
- All open-source contributors

## 📞 Support

For support, email support@roommatefinder.com or create an issue in this repository.

---

<div align="center">
  <p>Made with ❤️ for finding perfect roommates</p>
  <p>⭐ Star this repo if you found it helpful!</p>
</div>
