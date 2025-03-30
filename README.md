# 📌 CollabDo - Multi-User Collaborative To-Do List Web App

**CollabDo** is a collaborative to-do list web app that allows teams to efficiently organize, assign, and track tasks. With seamless user authentication, role-based access, and real-time updates, CollabDo makes teamwork effortless. Owners can create lists, invite team members, and manage tasks while ensuring transparency and productivity. 🚀✅

## 🚀 Features

✅ **User Authentication** (Signup/Login with JWT)  
✅ **Task Management** (Create, Read, Update, Delete)  
✅ **Team Collaboration** (Invite members to view lists)  
✅ **Role-Based Access** (Owner & Member permissions)  
✅ **Real-Time Updates** (Live sync for team members)  
✅ **Email Invitations** (Invite users via email)  
✅ **Dark Mode Support** 🌙  

## 🛠️ Tech Stack

### **Frontend:**
- React (Next.js)
- TailwindCSS (for UI design)
- Context API (for state management)

### **Backend:**
- Node.js + Express.js
- MongoDB (Mongoose for schema modeling)
- JWT Authentication
- Nodemailer (for sending invitations)

## 📂 Project Structure
```
collabdo/
│── backend/
│   ├── config/              # Database & JWT Configs
│   ├── models/              # Database Schemas (User, List)
│   ├── routes/              # API Routes (Auth, Lists, Invites)
│   ├── controllers/         # Business Logic
│   ├── middleware/          # Auth Middleware
│   ├── utils/               # Utility Functions (Email, etc.)
│   ├── server.js            # Main Express Server File
│
│── frontend/
│   ├── src/
│   │   ├── components/      # UI Components
│   │   ├── pages/           # Next.js Pages
│   │   ├── context/         # Global State (Auth, Lists)
│   │   ├── services/        # API Calls (Auth, Lists)
│   │   ├── styles/          # Tailwind CSS
│   ├── next.config.js       # Next.js Configuration
│
├── .env                     # Environment Variables
├── README.md                # Project Documentation
├── package.json             # Dependencies
```

## 📌 Installation & Setup

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/your-username/collabdo.git
cd collabdo
```

### **2️⃣ Backend Setup**
```sh
cd backend
npm install
# Configure .env file (MongoDB URI, JWT Secret, Email Configs)
npm start
```

### **3️⃣ Frontend Setup**
```sh
cd frontend
npm install
npm run dev
```

## 🔑 Environment Variables (.env Example)
```env
# Backend
MONGO_URI=your-mongodb-connection-string
JWT_SECRET=your-secret-key
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-email-password

# Frontend
NEXT_PUBLIC_API_URL=http://localhost:5000
```

## 🚀 API Endpoints

| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | /api/auth/register | Register new user |
| POST   | /api/auth/login | User login |
| POST   | /api/lists | Create a new to-do list (Owner only) |
| GET    | /api/lists/:id | Get list details (Owner & Members) |
| POST   | /api/invites | Send invitation to members |
| POST   | /api/invites/accept | Accept an invitation |

## 🤝 Contributing
1. Fork the repo
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m "Added new feature"`)
4. Push to your branch (`git push origin feature-branch`)
5. Open a Pull Request 🎉

## 📜 License
This project is licensed under the **MIT License**.

---

🚀 **Start collaborating and boosting productivity with CollabDo today!**

