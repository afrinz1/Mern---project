# 💬 Kudumbashri - Real-Time Chat Application

<div align="center">

![MERN](https://img.shields.io/badge/MERN-Stack-green)
![React](https://img.shields.io/badge/React-18.x-blue)
![Node.js](https://img.shields.io/badge/Node.js-18.x-green)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-brightgreen)
![Socket.io](https://img.shields.io/badge/Socket.io-Real--Time-black)
![License](https://img.shields.io/badge/License-MIT-yellow)

**Everyone can see everyone's messages in here! Just login and say hi to me or someone you don't even know. But don't mess things up though... we can ALL see ya! 👀**

[Live Demo](https://mern-project-unzm.onrender.com/)

</div>

## 🌟 Features

| Feature | Description |
|---------|-------------|
| 💬 **Real-Time Messaging** | Messages delivered instantly using Socket.io |
| 📸 **Image Sharing** | Share images seamlessly via Cloudinary |
| 🟢 **Online Status** | See who's online and who's pretending to be busy |
| 🔐 **Secure Authentication** | JWT-based auth with httpOnly cookies |
| 🎨 **30+ Themes** | Customize your chat experience with DaisyUI themes |## 🙏 Acknowledgments

### Special Thanks

A huge shoutout to **[Codesistency](codettps://www.youtube.com/@codesistency)** for their incredible [MERN Stack Chat App Tutorial](https://www.youtube.com/watch?v=ntKkVrQqBYY&list=LL&index=1). This project was built following their comprehensive guide, which provided excellent explanations of:
- Real-time messaging with Socket.io
- JWT authentication implementation
- Zustand state management
- Cloudinary integration
- Full-stack deployment

### Resources

- [React Documentation](https://react.dev/)
- [Socket.io Documentation](https://socket.io/docs/)
- [Tailwind CSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)
- [Cloudinary](https://cloudinary.com/)
- [MongoDB Atlas](https://www.mongodb.com/atlas)
- **Responsive Design**
- **Profile Management** 
- **User Presence**

---

## 🛠️ Tech Stack

### Frontend

| Technology | Purpose |
|------------|---------|
| React.js | UI Library |
| Vite | Build Tool |
| Tailwind CSS | Styling |
| DaisyUI | UI Components |
| Zustand | State Management |
| React Router | Client-side Routing |
| Axios | HTTP Client |
| Lucide React | Icons |

### Backend

| Technology | Purpose |
|------------|---------|
| Node.js | Runtime Environment |
| Express.js | Web Framework |
| MongoDB | Database |
| Mongoose | ODM |
| Socket.io | Real-Time Communication |
| JWT | Authentication |
| bcrypt | Password Hashing |
| Cloudinary | Image Storage |

---

## 📁 Project Structure
```
chat-mern/
├── 📂 backend/
│   ├── 📂 src/
│   │   ├── 📂 controllers/
│   │   │   ├── auth.controller.js
│   │   │   └── message.controller.js
│   │   ├── 📂 models/
│   │   │   ├── user.model.js
│   │   │   └── message.model.js
│   │   ├── 📂 routes/
│   │   │   ├── auth.route.js
│   │   │   └── message.route.js
│   │   ├── 📂 middleware/
│   │   │   └── auth.middleware.js
│   │   ├── 📂 lib/
│   │   │   ├── db.js
│   │   │   ├── cloudinary.js
│   │   │   └── socket.js
│   │   └── index.js
│   ├── package.json
│   └── .env
│
├── 📂 frontend/
│   ├── 📂 public/
│   │   └── avatar.png
│   ├── 📂 src/
│   │   ├── 📂 components/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   ├── ChatContainer.jsx
│   │   │   ├── ChatHeader.jsx
│   │   │   ├── MessageInput.jsx
│   │   │   ├── NoChatSelected.jsx
│   │   │   ├── AuthImagePattern.jsx
│   │   │   └── 📂 skeletons/
│   │   │       ├── MessageSkeleton.jsx
│   │   │       └── SidebarSkeleton.jsx
│   │   ├── 📂 pages/
│   │   │   ├── HomePage.jsx
│   │   │   ├── LoginPage.jsx
│   │   │   ├── SignUpPage.jsx
│   │   │   ├── ProfilePage.jsx
│   │   │   └── SettingsPage.jsx
│   │   ├── 📂 store/
│   │   │   ├── useAuthStore.js
│   │   │   ├── useChatStore.js
│   │   │   └── useThemeStore.js
│   │   ├── 📂 lib/
│   │   │   ├── axios.js
│   │   │   └── utils.js
│   │   ├── 📂 constants/
│   │   │   └── themes.js
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   └── package.json
│
└── package.json
```

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- **Node.js** (v18 or higher)
- **npm** or **yarn**
- **MongoDB** account (Atlas or local)
- **Cloudinary** account

### Installation

1. **Clone the repository**

bash
git clone https://github.com/afrinz1/Mern---project.git
cd Mern---project

2. Install dependencies

# Install root dependencies
npm install

# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install

Set up environment variables
Create a .env file in the backend folder:

# MongoDB
MONGODB_URI=mongodb+srv://your_username:your_password@cluster.xxxxx.mongodb.net/chat_db

# JWT
JWT_SECRET=your_super_secret_jwt_key_here

# Cloudinary
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Server
PORT=5000
NODE_ENV=development

Run the Application

# Run backend (from backend folder)
cd backend
npm run dev

# Run frontend (from frontend folder - new terminal)
cd frontend
npm run dev

Open your browser

Frontend: http://localhost:5173
Backend:  http://localhost:5000

 Environment Variables
Variable	Description	Required
MONGODB_URI	MongoDB connection string	✅
JWT_SECRET	Secret key for JWT tokens	✅
CLOUDINARY_CLOUD_NAME	Cloudinary cloud name	✅
CLOUDINARY_API_KEY	Cloudinary API key	✅
CLOUDINARY_API_SECRET	Cloudinary API secret	✅
PORT	Server port (default: 5000)	❌
NODE_ENV	Environment (development/production)	❌


## 🔧 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `MONGODB_URI` | MongoDB connection string | ✅ |
| `JWT_SECRET` | Secret key for JWT tokens | ✅ |
| `CLOUDINARY_CLOUD_NAME` | Cloudinary cloud name | ✅ |
| `CLOUDINARY_API_KEY` | Cloudinary API key | ✅ |
| `CLOUDINARY_API_SECRET` | Cloudinary API secret | ✅ |
| `PORT` | Server port (default: 5000) | ❌ |
| `NODE_ENV` | Environment (development/production) | ❌ |

---

## 📡 API Endpoints

### Authentication Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/signup` | Register a new user |
| `POST` | `/api/auth/login` | Login user |
| `POST` | `/api/auth/logout` | Logout user |
| `GET`  |`/api/auth/check` | Check authentication status |
| `PUT` | `/api/auth/update-profile` | Update profile picture |

### Message Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/messages/users` | Get all users for sidebar |
| `GET` | `/api/messages/:id` | Get messages with a user |
| `POST` | `/api/messages/send/:id` | Send a message |

---

## 🔌 Socket.io Events

| Event | Direction | Description |
|-------|-----------|-------------|
| `connection` | Client → Server | User connects |
| `disconnect` | Client → Server | User disconnects |
| `getOnlineUsers` | Server → Client | List of online users |
| `newMessage` | Server → Client | New message received |


## 🎨 Available Themes

This app uses DaisyUI themes. Available options:

| | | | | | |
|---|---|---|---|---|---|
| light | dark | cupcake | bumblebee | emerald | corporate |
| synthwave | retro | cyberpunk | valentine | halloween | garden |
| forest | aqua | lofi | pastel | fantasy | wireframe |
| black | luxury | dracula | cmyk | autumn | business |
| acid | lemonade | night | coffee | winter | dim |
| nord | sunset | | | | |

---

## 🛡️ Security Features

- ✅ Password hashing with **bcrypt**
- ✅ JWT tokens stored in **httpOnly cookies**
- ✅ Protected routes with **authentication middleware**
- ✅ **CORS** configuration for cross-origin requests
- ✅ Input validation and sanitization
- ✅ Secure password requirements

---

## 📦 Scripts

### Backend

```bash
npm run dev      # Start development server with nodemon
npm run start    # Start production server
```

### Frontend

```bash
npm run dev      # Start Vite development server
npm run build    # Build for production
npm run preview  # Preview production build
```

### Root

```bash
npm run build    # Build both frontend and backend
npm run start    # Start production server
```



## 🚀 Deployment

### Deploy on Render

1. Create a new **Web Service** on [Render](https://render.com)
2. Connect your GitHub repository
3. Configure the following:
   - **Build Command:** `npm run build`
   - **Start Command:** `npm run start`
4. Add environment variables in Render dashboard
5. Deploy! 🎉

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a new branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit** your changes
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push** to the branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open** a Pull Request

---

## 📋 Future Enhancements

- [ ] Group chat functionality
- [ ] Voice and video calls (WebRTC)
- [ ] Message reactions (emoji)
- [ ] File sharing (documents, PDFs)
- [ ] Message search
- [ ] Push notifications
- [ ] End-to-end encryption
- [ ] Typing indicators
- [ ] Read receipts
- [ ] Message deletion

---

## 🐛 Known Issues

- Free tier on Render sleeps after 15 minutes of inactivity
- Large images may take time to upload
- First load may be slow due to free tier limitations

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Afrin**

[![GitHub](https://img.shields.io/badge/GitHub-afrinz1-181717?style=for-the-badge&logo=github)](https://github.com/afrinz1)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/your-linkedin)

---

## 🙏 Acknowledgments

### Resources

- [React Documentation](https://react.dev/)
- [Socket.io Documentation](https://socket.io/docs/)
- [Tailwind CSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)
- [Cloudinary](https://cloudinary.com/)
- [MongoDB Atlas](https://www.mongodb.com/atlas)

---

<div align="center">

### ⭐ Star this repo if you found it helpful!

**Made with ❤️ and mass lots of coffee ☕**

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=afrinz1.Mern---project)

</div>
```