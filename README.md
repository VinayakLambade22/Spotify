# 🎵 Spotify Clone

A full-stack Spotify clone built with modern web technologies, featuring real-time music streaming, user authentication, and a responsive design.

## ✨ Features

- 🎶 Music streaming and playback controls
- 👤 User authentication with Clerk
- 📱 Responsive design with Tailwind CSS
- 🔄 Real-time updates with Socket.IO
- ☁️ Cloud storage integration with Cloudinary
- 📊 Music library management
- 🎵 Album and song organization
- 🔍 Search functionality

## 🛠️ Tech Stack

### Frontend
- **React 19** - Modern UI library
- **TypeScript** - Type-safe development
- **Vite** - Fast build tool
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Accessible component library
- **Zustand** - State management
- **Clerk** - Authentication
- **Socket.IO Client** - Real-time communication

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** with Mongoose - Database
- **Socket.IO** - Real-time communication
- **Cloudinary** - Media storage
- **Clerk** - Authentication middleware
- **Node-cron** - Scheduled tasks

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- MongoDB database
- Cloudinary account
- Clerk account

### Installation

1. **Clone the repository**
```bash
git clone <your-repository-url>
cd Spotify
```

2. **Install dependencies for both frontend and backend**
```bash
npm run build
```
*This command installs dependencies for both frontend and backend*

3. **Environment Variables**

Create `.env` files in both `backend/` and `frontend/.env.local`:

**Backend (.env):**
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
```

**Frontend (.env.local):**
```env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
VITE_API_URL=http://localhost:5000
```

### 🏃‍♂️ Running the Application

#### Development Mode

1. **Start the backend server**
```bash
cd backend
npm run dev
```

2. **Start the frontend development server**
```bash
cd frontend
npm run dev
```

#### Production Mode

1. **Build the frontend**
```bash
cd frontend
npm run build
```

2. **Start the production server**
```bash
npm start
```

### 📊 Database Seeding

To populate your database with sample data:

```bash
cd backend
npm run seed:albums
npm run seed:songs
```

## 📁 Project Structure

```
Spotify/
├── backend/
│   ├── src/
│   │   ├── index.js          # Main server file
│   │   └── seeds/            # Database seeding scripts
│   ├── .env                  # Backend environment variables
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── App.tsx           # Main App component
│   │   ├── main.tsx          # Entry point
│   │   └── components/       # React components
│   ├── .env.local            # Frontend environment variables
│   └── package.json
└── package.json              # Root package.json with build scripts
```

## 🔧 Available Scripts

### Root Level
- `npm run build` - Install dependencies for both frontend and backend
- `npm start` - Start the production server

### Backend
- `npm run dev` - Start development server with nodemon
- `npm start` - Start production server
- `npm run seed:songs` - Seed database with songs
- `npm run seed:albums` - Seed database with albums

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 🎯 Key Features Implementation

- **Authentication**: Integrated with Clerk for secure user management
- **Real-time Features**: Socket.IO for live updates and interactions
- **File Upload**: Express-fileupload with Cloudinary integration
- **Database**: MongoDB with Mongoose for data modeling
- **UI Components**: Custom components built with Radix UI and Tailwind CSS
- **State Management**: Zustand for efficient state handling
- **Responsive Design**: Mobile-first approach with Tailwind CSS

## 🔍 API Endpoints

The backend provides RESTful APIs for:
- User authentication and management
- Music library operations
- Song and album management
- File uploads and media handling
- Real-time communication endpoints

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 🎨 Screenshots

*Add screenshots of your application here*

## 🔗 Deployment

For deployment instructions, refer to your hosting platform's documentation:
- **Frontend**: Vercel, Netlify, or similar
- **Backend**: Heroku, Railway, or similar
- **Database**: MongoDB Atlas

---

Made with ❤️ and 🎵