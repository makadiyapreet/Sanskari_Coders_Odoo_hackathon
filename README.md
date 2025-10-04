# 💰 Expense Management System with Smart Approvals

<div align="center">

![MERN Stack](https://img.shields.io/badge/MERN-Stack-green?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)

**Streamline expense tracking with intelligent multi-level approval workflows**

[View Demo](#-screenshots) • [Quick Start](#-quick-start) • [Features](#-features)

</div>

---

## 🎯 What This Solves

Manual expense reimbursements are slow and error-prone. This system automates the entire workflow - from submission to approval - with configurable rules that match your company's structure. No more chasing approvals through email chains.

## ⚡ Features

### 🔐 Smart Authentication
- Auto-creates company and admin account on signup
- Sets company currency based on selected country
- Role-based access: Admin, Manager, Employee
- Dynamic manager-employee relationships

### 💸 Expense Submission
- Quick form entry or **OCR receipt scanning** (auto-extracts amount, date, merchant, line items)
- Multi-currency support with real-time conversion
- Live approval status tracking
- Complete expense history with filters

### 🔄 Flexible Approval Workflows

Two powerful systems that work independently or together:

**Sequential Approvals**
- Chain multiple approvers (Manager → Finance → CFO)
- Each step requires approval before moving forward
- Optional manager pre-approval stage

**Conditional Rules**
- **Percentage**: Auto-approve at 60% consensus
- **Key Person**: CFO approval = instant approval
- **Hybrid**: Combine conditions (60% OR CFO)

Mix both systems for complex workflows like: "Manager approval required, then 2 of 3 finance team members, OR direct CFO approval skips all."

### 👥 Role Capabilities

| Role | What You Can Do |
|------|-----------------|
| **Employee** | Submit expenses, scan receipts, track approval status, view history |
| **Manager** | Approve/reject with comments, view team spending, see amounts in company currency |
| **Admin** | Manage users, configure approval rules, view all expenses, override decisions |

### 📊 Dashboard & Analytics
- Visual expense overview with charts
- Category-wise breakdowns
- Date range filtering
- Spending pattern analysis
- Real-time updates

## 🛠️ Tech Stack

**Frontend**
- React.js with Redux for state management
- React-Bootstrap + Material Icons
- TSParticles for visual effects
- react-datepicker, moment, unique-names-generator

**Backend**
- Node.js + Express.js REST API
- JWT authentication with protected routes
- Mongoose ODM for MongoDB

**Integrations**
- [REST Countries API](https://restcountries.com/v3.1/all) - Currency data
- [Exchange Rate API](https://api.exchangerate-api.com/v4/latest/) - Live conversions

## 🚀 Quick Start

### Prerequisites
- Node.js v14+
- MongoDB
- npm/yarn

### Installation

```bash
# Clone repository
git clone https://github.com/makadiyapreet/Sanskari_Coders_Odoo_hackathon
cd Sanskari_Coders_Odoo_hackathon

# Frontend setup
cd frontend
npm install

# Backend setup
cd backend
npm install
```

### Configuration

Create `backend/config/config.env`:

```env
MONGO_URL=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_secret_key
```

### Run Application

```bash
# Terminal 1 - Backend
cd backend
npm run dev

# Terminal 2 - Frontend
cd frontend
npm start
```

Application runs at `http://localhost:3000`

## 📸 Screenshots

<div align="center">

### Dashboard Overview
![Dashboard](https://i.postimg.cc/6qLR3WNt/Expense-Management-System-Brave-19-04-2023-11-08-53.png)

### Expense Submission
![Submission](https://i.postimg.cc/DynLNXqZ/Expense-Management-System-Brave-19-04-2023-11-08-59.png)

### Approval Workflow
![Workflow](https://i.postimg.cc/Dy6L3wgc/Expense-Management-System-Brave-19-04-2023-11-15-46.png)

### Analytics & Reports
![Reports](https://i.postimg.cc/13YF47bn/Expense-Management-System-Brave-19-04-2023-11-15-54.png)

### Manager Dashboard
![Manager View](https://i.postimg.cc/rwpWV2Z2/Expense-Management-System-Brave-19-04-2023-11-16-01.png)

</div>

## 🎨 Design Resources

UI/UX Mockups: [View on Excalidraw](https://link.excalidraw.com/l/65VNwvy7c4X/4WSLZDTrhkA)

## 🔄 Workflow Example

1. **Setup**: Admin creates company → Adds employees & managers → Configures approval rules
2. **Submit**: Employee uploads receipt → OCR extracts data → Submits expense
3. **Route**: System automatically routes to correct approvers based on rules
4. **Approve**: Each approver reviews → Approves/rejects with comments
5. **Notify**: Employee receives final decision → Amount processed

## 🌟 Standout Features

- **Smart OCR**: Just snap a photo of your receipt - the system handles the rest
- **Currency Intelligence**: All amounts automatically convert to company currency for managers
- **Rule Flexibility**: Create simple or complex approval chains that match your workflow
- **Real-time Sync**: See approvals happen live across all dashboards

## 📋 Future Enhancements

- [ ] React Native mobile app
- [ ] Budget tracking and alerts
- [ ] Accounting software integrations
- [ ] Bulk import/export functionality
- [ ] Advanced analytics dashboard
- [ ] Custom expense categories per company

## 🤝 Contributing

Contributions welcome! Open an issue or submit a PR.

```bash
git checkout -b feature/amazing-feature
git commit -m 'Add amazing feature'
git push origin feature/amazing-feature
```

## 📄 License

MIT License - see [LICENSE](LICENSE) file

## 👨‍💻 Built By

**Preet Makadiya - Dhairyasinh Parmar**

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/makadiyapreet/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/preetmakadiya)

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Built with 💙 using MERN Stack

</div>
