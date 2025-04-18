🤖 AI Interview Coach

AI Interview Coach is a smart and interactive web-based platform that helps users practice for interviews using AI-driven tools, quizzes, and real-time video-based mock interviews.

Features:

- Live interview rooms with webcam and microphone
- AI-based interview Q&A with adaptive difficulty
- Domain-specific quizzes with evaluation
- Resume-based profile and progress tracker
- Real-time peer-to-peer room system

Tech Stack:

Frontend: ReactJS (Vite), Tailwind CSS  
Backend: Node.js, Express.js  
Database: MongoDB Atlas  
AI Integration: Google Gemini API  
Real-time: Socket.io  
Deployment: Vercel (frontend) and Render (backend)

Local Setup Instructions:

1. Clone the repository

   git clone https://github.com/ayusssh01/AI-Interview-Coach.git
   cd AI-Interview-Coach

 🖥️ 2. Backend Setup

```bash
cd backend
npm install
```

🔐 Create a `.env` file inside `/backend` and add the following:

```env
JWT_SECRET=your_jwt_secret
MONGODB_URI=your_mongodb_uri
GEMINI_API_KEY=your_gemini_key
CLOUDINARY_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
PORT=3000
NODE_ENV=development
```

➡️ Start the backend server:

```bash
npm run dev
```

---

🌐 3. Frontend Setup

```bash
cd ../frontend
npm install
```

🔐 Create a `.env` file inside `/frontend` and add:

```env
VITE_API_URL=http://localhost:3000
```

➡️ Start the frontend server:

```bash
npm run dev
```

🔗 Open in browser:
```
http://localhost:5173
```

---

📡 API Endpoints Overview

| Endpoint                                | Description                      |
|----------------------------------------|----------------------------------|
| `POST /api/v1/auth/signup`             | User registration                |
| `POST /api/v1/auth/login`              | User login                       |
| `POST /api/v1/auth/logout`             | Logout session                   |
| `POST /api/v1/auth/editUser`           | Update user profile              |
| `POST /api/v1/auth/updateAvatar`       | Upload profile picture           |
| `GET /api/v1/auth/getAuth`             | Check authentication status      |
| `POST /api/v1/rooms/addroom/:roomID`   | Create video interview room      |
| `POST /api/v1/rooms/deleteroom/:roomID`| Delete a room                    |
| `GET /api/v1/rooms/getroom/:roomID`    | Get room data                    |
| `POST /api/v1/quiz/generate-quiz`      | Generate new quiz                |
| `POST /api/v1/quiz/save-answer`        | Save quiz answer                 |
| `POST /api/v1/quiz/evaluate-answer`    | Evaluate quiz                    |
| `POST /api/v1/quiz/terminate-quiz`     | End quiz session                 |
| `POST /api/v1/questions/chat`          | AI-based chat questions          |

---

🌍 Deployment

This project is deployed using:

- 🚀 Frontend: Vercel  
- ⚙️ Backend: Render  
- 🌐 [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for database hosting

🔗 Demo URLs (after deployment):

```text
Frontend: https://your-vercel-app.vercel.app
Backend:  https://ai-interview-coach-backend.onrender.com
```

---

🤝 Contributing

We welcome improvements, bug reports, and ideas!  
Feel free to fork the repo, create a branch, and raise a pull request.

---

🙏 Acknowledgements

- [Gemini API](https://ai.google.dev) for powerful AI integration
- [MongoDB](https://www.mongodb.com/) for seamless data storage
- [Vercel](https://vercel.com/) for frontend hosting
- [Render](https://render.com/) for backend deployment

---

💼 Built with ❤️ by Ayush & Team  
_Interview confidently. Grow continuously._
