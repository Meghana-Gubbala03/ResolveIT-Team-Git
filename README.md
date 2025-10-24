# ResolveIT - Smart Grievance & Feedback Management System

Here is our team collabration work

## 📋 Project Overview

ResolveIT is a comprehensive online complaint and grievance portal designed to bring transparency and efficiency to institutional complaint handling. The platform enables users to submit complaints (anonymously or publicly), track their status in real-time, and escalate unresolved issues, while administrators manage the entire resolution process through an intuitive dashboard.

## ✨ Key Features

### User Features
- **Dual Submission Modes**: Submit complaints publicly (trackable) or anonymously (private)
- **Real-time Status Tracking**: Track complaint progress through all resolution stages
- **Evidence Upload**: Attach supporting documents and images (JPG, PNG, PDF, DOC, DOCX)
- **Complaint History**: View all your past complaints with detailed information
- **Priority Levels**: Set urgency levels (Low, Medium, High, Critical)
- **Timeline View**: See chronological updates and admin comments

### Admin Features
- **Comprehensive Dashboard**: Overview of all complaints with filtering options
- **Status Management**: Update complaint status through the resolution workflow
- **Assignment System**: Assign complaints to specific staff members
- **Internal Notes**: Add private notes visible only to admin staff
- **Public Replies**: Communicate with users about their complaint progress
- **Analytics**: Visual insights into complaint trends and performance metrics
- **Auto-escalation**: Automatic escalation of unresolved critical issues

### Reporting & Analytics
- **Visual Dashboards**: Charts showing status distribution, category breakdown, and trends
- **Export Functionality**: Download complaint data in CSV or JSON format
- **Performance Metrics**: Track resolution time, resolution rate, and critical issues
- **Custom Filters**: Filter by status, category, priority, and date range

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI library
- **React Router** - Navigation
- **CSS3** - Styling with responsive design
- **Fetch API** - HTTP requests

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MySQL** - Database
- **Multer** - File upload handling
- **JWT** - Authentication
- **bcrypt.js** - Password hashing
- **node-cron** - Scheduled tasks

## 📁 Project Structure

```
resolveit-portal/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── AdminDashboard.js
│   │   │   ├── ComplaintForm.js
│   │   │   ├── ComplaintHistory.js
│   │   │   ├── ComplaintTracking.js
│   │   │   ├── Navbar.js
│   │   │   └── ReportsExport.js
│   │   ├── App.js
│   │   ├── App.css
│   │   ├── Dashboard.js
│   │   ├── home.js
│   │   ├── login.js
│   │   ├── signup.js
│   │   ├── index.js
│   │   └── index.css
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── Server.js
│   ├── createAdmin.js
│   ├── uploads/
│   ├── .env
│   └── package.json
│
└── README.md
```

## 🚀 Installation & Setup

### Prerequisites
- Node.js (v14 or higher)
- MySQL (v5.7 or higher)
- npm or yarn package manager

### Backend Setup

1. **Navigate to the backend directory:**
```bash
cd backend
```

2. **Install dependencies:**
```bash
npm install
```

3. **Create a `.env` file:**
```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD="Your_SQL_password"
DB_NAME=complaint_system
JWT_SECRET=your_secret_key_here
```

4. **Update database credentials in Server.js** (if needed):
```javascript
const pool = mysql.createPool({
  host: "localhost",
  port: 3306,
  user: "root",
  password: "Your_SQL_password",
  database: "complaint_system",
  waitForConnections: true,
  connectionLimit: 10,
  queueLimit: 0,
});
```

5. **Start the backend server:**
```bash
node Server.js
```

The server will run on `http://localhost:5000`

### Frontend Setup

1. **Navigate to the frontend directory:**
```bash
cd frontend
```

2. **Install dependencies:**
```bash
npm install
```

3. **Start the development server:**
```bash
npm start
```

The application will open at `http://localhost:3000`

### Creating Admin Account

1. **Run the admin creation script:**
```bash
node createAdmin.js
```

**Default Admin Credentials:**
- Email: `admin@resolveit.com`
- Password: `admin123`

**Important:** Change these credentials after first login!

## 📱 Usage Guide

### For Users

1. **Sign Up/Login**: Create an account or log in to submit complaints
2. **Submit Complaint**: Choose submission type (Public/Anonymous), fill in details
3. **Track Status**: Use the tracking feature to monitor complaint progress
4. **View History**: Access all your past complaints in "My Complaints" section

### For Admins

1. **Login**: Use admin credentials to access the admin dashboard
2. **View Dashboard**: See overview of all complaints with statistics
3. **Manage Complaints**: Update status, assign to staff, add notes
4. **Generate Reports**: View analytics and export data for analysis

## 🔐 Security Features

- Password encryption using bcrypt
- JWT-based authentication
- Role-based access control (User/Admin)
- Input validation and sanitization
- File type and size restrictions
- SQL injection prevention with parameterized queries

## 📊 Workflow

```
User Submission → Admin Review → Assignment → Resolution → Closure
                    ↓
              (If delayed) → Escalation → Higher Authority
```

### Status Flow
1. **New** - Complaint just submitted
2. **Under Review** - Admin reviewing the complaint
3. **In Progress** - Working on resolution
4. **Resolved** - Issue resolved
5. **Closed** - Complaint closed
6. **Escalated** - Escalated to higher authority

## 🎯 Project Milestones

- ✅ **Week 1-2**: Login and Complaint Input Module
- ✅ **Week 3-4**: Complaint Status System
- ✅ **Week 5**: Admin Dashboard
- ✅ **Week 6-7**: Escalation Logic
- ✅ **Week 8**: Reports and Export

## 🤝 Contributing

This is an academic project. For any issues or suggestions:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is created for educational purposes.

## 👥 Authors

G. Meghana (meghana.gubbala@gmail.com)

P Amarnath (amarnath21602@gmail.com)

K. Kavya (kavyakatragadda41@gmail.com)

E. Rajesh (rediga2@gitam.in)


## 🙏 Acknowledgments

- Built as part of Infosys SpringBoard Virtual Internship 6.0.
- Special thanks to faculty Maheshvaran sir, advisors and mentors.
- Great pleasure to work with the amazing team mates.
