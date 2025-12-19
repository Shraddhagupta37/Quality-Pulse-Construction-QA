# Construction Quality Pulse 📘

A full-stack, real-time web application for daily construction quality assurance, site progress monitoring, QA reporting, analytics, and instant notifications.

**Built with:** React.js • TailwindCSS • Node.js • Express.js • MongoDB • Socket.io

## ✨ Features

### 👥 User Roles
- **Admin** – Manage users, sites, reports, and analytics
- **Engineer** – Submit QA reports with photo uploads

### 🏗️ Construction Sites
- Create, edit, and manage construction sites
- Assign engineers to specific sites
- Track progress, status, and timeline, and compliance

### 📝 Daily QA Reports
- Submit detailed inspection reports with photos
- Report approval workflow (Pending → Approved/Rejected)
- Real-time updates via Socket.io

### 📊 Analytics Dashboard
- Compliance percentage and Pass/Fail statistics
- day-wise QA trend visualization
- Site-wise performance comparison
- Material failure distribution

### 🔔 Real-Time Notifications
- Toast alerts, notification panel, and live dashboard feed
- Triggered on: new reports, site assignments, failures, and status updates

### 🔐 Security
- JWT authentication with bcrypt password hashing
- Role-based API access control
- Protected frontend routes

### 📁 Additional Features
- CSV/PDF export functionality
- Audit logging with timestamps

## 🚀 Quick Start

### Prerequisites
- Node.js v16+
- MongoDB (local or cloud)
- npm

### Installation

```bash
git clone https://github.com/YOUR_USERNAME/construction-quality-pulse.git
cd construction-quality-pulse
```

### Backend Setup
```bash
cd server
npm install
```

Create `.env`:
```
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
```

```bash
npm run dev  # Runs at http://localhost:5000
```

### Frontend Setup
```bash
cd client
npm install
```

Create `.env`:
```
VITE_API_URL=http://localhost:5000
```

```bash
npm run dev  # Runs at http://localhost:5173
```

## 📚 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/sites` | List all sites |
| POST | `/api/sites` | Create site (Admin) |
| GET | `/api/reports` | Get QA reports |
| POST | `/api/reports` | Submit report |

## 🧪 Testing

```bash
npm run test
```

## 📦 Deployment

**Backend:** Push to Render/Railway with environment variables

**Frontend:** Build and deploy to Vercel/Netlify
```bash
npm run build
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push and open a Pull Request

## 📄 License
MIT License – feel free to use and modify

## 💬 Support
Have questions? [Open an issue](https://github.com/YOUR_USERNAME/construction-quality-pulse/issues) or contact the maintainer.
