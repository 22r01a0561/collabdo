# 📌 CollabDo - Multi-User Collaborative To-Do List Web App

CollabDo is a powerful and user-friendly collaborative to-do list web application. It enables teams to efficiently organize, assign, and track tasks with real-time updates and role-based access control. Whether you're managing personal projects or working with a team, CollabDo simplifies task collaboration. 🚀✅

---

## 🔥 Key Features

### ✅ User Authentication

- Secure **Signup/Login** using JWT authentication.
- Password encryption for better security.

### ✅ Task & List Management

- Users can **create, edit, delete** to-do lists.
- Each list contains multiple **tasks with statuses** (Pending, In Progress, Completed).

### ✅ Team Collaboration

- Owners can **invite members** to view and contribute to lists.
- Team members can **collaborate in real-time**.

### ✅ Role-Based Access Control

- **Owners** can create lists, add tasks, and invite members.
- **Members** can view and complete assigned tasks.

### ✅ Real-Time Updates

- Changes are **instantly reflected** for all users.
- Ensures smooth collaboration.

### ✅ Email Invitations

- Invite users via **email notifications** to join lists.

### ✅ Dark Mode Support 🌙

- Toggle between **light and dark mode** for better UX.

---

## 🛠️ Tech Stack

### **Frontend:**

- React (Next.js)
- TailwindCSS (for styling)
- Context API (for state management)

### **Backend:**

- Node.js + Express.js
- MongoDB (Mongoose for schema modeling)
- JWT Authentication (for secure login)
- Nodemailer (for sending email invites)

### **Other Tools:**

- GitHub (Version Control)
- Postman (API Testing)
- Vercel/Netlify (Frontend Deployment)
- Render/Heroku (Backend Deployment)

---

## 📁 Project Structure

```
collabdo/
│── backend/                   # Express.js backend
│   ├── config/                # Database & JWT Configs
│   │   ├── db.js              # MongoDB connection
│   │   ├── auth.js            # JWT authentication
│   │
│   ├── models/                # Database Schemas
│   │   ├── User.js            # User Model
│   │   ├── List.js            # To-Do List Model
│   │
│   ├── routes/                # API Routes
│   │   ├── authRoutes.js      # Signup/Login Routes
│   │   ├── listRoutes.js      # List CRUD Routes
│   │   ├── inviteRoutes.js    # Invitation System
│   │
│   ├── controllers/           # Business Logic
│   │   ├── authController.js  # User Authentication Logic
│   │   ├── listController.js  # To-Do List Logic
│   │   ├── inviteController.js # Team Member Invitation Logic
│   │
│   ├── middleware/            # Middleware (Auth, Error Handling)
│   │   ├── authMiddleware.js  # Protect Routes
│   │
│   ├── utils/                 # Utility Functions (Email, etc.)
│   │   ├── sendInvite.js      # Send Invitation Emails
│   │
│   ├── server.js              # Main Express Server File
│
│── frontend/                  # React (Next.js) Frontend
│   ├── src/
│   │   ├── components/        # Reusable UI Components
│   │   │   ├── TaskItem.js    # Individual Task Component
│   │   │   ├── InviteForm.js  # Invite Members Component
│   │   │   ├── Navbar.js      # Navbar Component
│   │   │
│   │   ├── pages/             # Next.js Pages
│   │   │   ├── index.js       # Home Page (Lists)
│   │   │   ├── login.js       # Login Page
│   │   │   ├── register.js    # Register Page
│   │   │   ├── list/[id].js   # List Details Page
│   │   │
│   │   ├── context/           # Global State Management
│   │   │   ├── AuthContext.js # Authentication Context
│   │   │   ├── ListContext.js # Lists & Tasks Context
│   │   │
│   │   ├── services/          # API Calls (Frontend)
│   │   │   ├── authService.js # API calls for authentication
│   │   │   ├── listService.js # API calls for lists & tasks
│   │   │
│   │   ├── styles/            # Tailwind CSS / Global Styles
│   │   │   ├── globals.css    # Global Styles
│   │
│   ├── next.config.js         # Next.js Configuration
│   ├── package.json           # Frontend Dependencies
│
├── .env                       # Environment Variables
├── README.md                   # Project Documentation
├── package.json                # Root Dependencies
├── .gitignore                   # Ignore Node Modules, etc.
```

---

## 🚀 Getting Started

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

---

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

---

## 🚀 API Endpoints

| Method | Endpoint            | Description                          |
| ------ | ------------------- | ------------------------------------ |
| POST   | /api/auth/register  | Register new user                    |
| POST   | /api/auth/login     | User login                           |
| POST   | /api/lists          | Create a new to-do list (Owner only) |
| GET    | /api/lists/\:id     | Get list details (Owner & Members)   |
| POST   | /api/invites        | Send invitation to members           |
| POST   | /api/invites/accept | Accept an invitation                 |

---

## 🤝 Contributing

1. Fork the repo
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m "Added new feature"`)
4. Push to your branch (`git push origin feature-branch`)
5. Open a Pull Request 🎉

---

## 📜 License

This project is licensed under the **MIT License**.

---

🚀 **Start collaborating and boosting productivity with CollabDo today!**

