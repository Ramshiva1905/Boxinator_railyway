# 🚂 Boxinator Railway - Shipping Management System

[![Railway](https://img.shields.io/badge/Railway-Deployed-success)](https://railway.app)
[![Node.js](https://img.shields.io/badge/Node.js-18+-green)](https://nodejs.org)
[![React](https://img.shields.io/badge/React-19+-blue)](https://reactjs.org)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Railway-blue)](https://railway.app)

A full-stack shipping management system built for Railway deployment with PostgreSQL database.

## 🚀 **Railway Deployment Ready**

This version is specifically configured for Railway deployment with:
- ✅ **PostgreSQL Integration** - Direct Railway database connection
- ✅ **Environment Configuration** - Railway-optimized settings  
- ✅ **SSL Support** - Production-ready security
- ✅ **Auto-scaling** - Railway platform benefits

## 🏗️ **Architecture**

```
Frontend (React + Vite)     Backend (Node.js + Express)     Database (PostgreSQL)
├── React 19               ├── Express.js                   ├── Railway PostgreSQL
├── React Router           ├── Sequelize ORM                ├── SSL Enabled
├── Axios                  ├── JWT Authentication           ├── Auto-backups
└── Responsive CSS         └── bcrypt Encryption            └── Connection pooling
```

## 🎯 **Features**

### **User Management**
- Secure registration and login
- JWT-based authentication  
- Profile management
- Password encryption with bcrypt

### **Shipment System**
- Create and track shipments
- Real-time cost calculator
- Shipment status updates
- History tracking

### **Admin Dashboard**
- User management
- Shipment oversight
- System analytics
- Audit logging

## 🚀 **Quick Railway Deployment**

### **1. Create Railway Project**
```bash
# 1. Go to railway.app and create new project
# 2. Connect this GitHub repository
# 3. Add PostgreSQL service
```

### **2. Set Environment Variables**
```env
NODE_ENV=production
JWT_SECRET=your-super-secure-jwt-secret-key
PORT=3000
```

### **3. Deploy**
Railway automatically deploys when you push to main branch!

## 💻 **Local Development**

### **Backend Setup**
```bash
cd Backend
npm install
cp .env.development .env
npm run dev
```

### **Frontend Setup**  
```bash
cd Frontend
npm install
npm run dev
```

## 🔧 **Configuration**

### **Database Options**
- **Production**: Railway PostgreSQL (automatic)
- **Development**: SQLite (set `USE_LOCAL_DB=true`)

### **Environment Variables**

| Variable | Purpose | Required |
|----------|---------|----------|
| `DATABASE_URL` | Railway PostgreSQL | ✅ Auto-set |
| `NODE_ENV` | Environment | ✅ |
| `JWT_SECRET` | Token encryption | ✅ |
| `PORT` | Server port | ✅ |

## 📁 **Project Structure**

```
Boxinator_Railway/
├── Backend/                 # Node.js API server
│   ├── config/
│   │   └── database.js      # Railway PostgreSQL config
│   ├── controllers/         # Route handlers
│   ├── middleware/          # Auth & validation
│   ├── models/             # Sequelize models
│   ├── routes/             # API endpoints
│   └── services/           # Business logic
├── Frontend/               # React application
│   ├── src/
│   │   ├── components/     # React components
│   │   └── services/       # API client
├── RAILWAY_SETUP_GUIDE.md  # Detailed deployment guide
├── RAILWAY_CHECKLIST.md    # Quick setup checklist  
└── MIGRATION_SUMMARY.md    # Changes from Supabase
```

## 🛠️ **Tech Stack**

### **Backend**
- **Node.js** + **Express.js** - Server framework
- **Sequelize** - PostgreSQL ORM  
- **Railway PostgreSQL** - Database hosting
- **JWT** - Authentication
- **bcrypt** - Password hashing
- **Helmet** - Security middleware

### **Frontend**  
- **React 19** - UI framework
- **Vite** - Build tool
- **React Router** - Navigation
- **Axios** - HTTP client

## 📊 **Database Schema**

- **Users** - Authentication and profiles
- **Shipments** - Package tracking
- **Countries** - Shipping destinations  
- **BoxTypes** - Package categories
- **WeightTiers** - Pricing structure

## 🔒 **Security Features**

- JWT token authentication
- Password encryption (bcrypt)
- Input validation (Joi)
- Rate limiting
- CORS protection
- SQL injection prevention
- XSS protection

## 📚 **Documentation**

- [`RAILWAY_SETUP_GUIDE.md`](./RAILWAY_SETUP_GUIDE.md) - Complete deployment guide
- [`RAILWAY_CHECKLIST.md`](./RAILWAY_CHECKLIST.md) - Quick setup checklist
- [`MIGRATION_SUMMARY.md`](./MIGRATION_SUMMARY.md) - Migration details

## 🚨 **Support**

- **Railway Docs**: [docs.railway.app](https://docs.railway.app)
- **Issues**: [GitHub Issues](https://github.com/Ramshiva1905/Boxinator_railyway/issues)
- **Railway Community**: [Discord](https://discord.gg/railway)

## 📄 **License**

This project is licensed under the MIT License.

---

**🚂 Powered by Railway | 🚀 Ready for Production**
