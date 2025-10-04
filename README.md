# 💰 Advanced Expense Management System

<div align="center">

![Expense Management](https://img.shields.io/badge/Expense-Management-blue?style=for-the-badge)
![MERN Stack](https://img.shields.io/badge/MERN-Stack-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**A comprehensive expense tracking and approval workflow system built with MERN Stack**

[Live Demo](https://main.d1sj7cd70hlter.amplifyapp.com/) • [Report Bug](https://github.com/Priyanshu9898/Expense-Tracker-App/issues) • [Request Feature](https://github.com/Priyanshu9898/Expense-Tracker-App/issues)

</div>

---

## 🌟 Overview

The Advanced Expense Management System streamlines expense tracking and reimbursement processes for organizations. With intelligent approval workflows, multi-currency support, and OCR-powered receipt scanning, it eliminates manual, error-prone processes while providing complete transparency.

## ✨ Key Features

### 🔐 Authentication & User Management
- **Auto-Company Creation**: Company and Admin user created automatically on signup
- **Multi-Currency Support**: Company currency set based on selected country
- **Role-Based Access Control**: Admin, Manager, and Employee roles
- **Dynamic Role Assignment**: Admins can create employees, assign managers, and modify roles

### 💳 Expense Submission (Employee)
- Submit expense claims with amount, category, description, and date
- **Multi-Currency Expenses**: Support for expenses in different currencies
- **OCR Receipt Scanning**: Auto-extract expense details from receipt images
- View expense history with approval status (Approved/Rejected)
- Track approval progress in real-time

### ✅ Intelligent Approval Workflows

#### Multi-Level Approval
- Configure sequential approval chains (Manager → Finance → Director)
- Manager approver checkbox for first-level approval
- Admin-defined approval sequences
- Expense moves to next approver only after current approval/rejection

#### Conditional Approval Rules
- **Percentage Rule**: Auto-approve when X% of approvers approve (e.g., 60%)
- **Specific Approver Rule**: Auto-approve when key person approves (e.g., CFO)
- **Hybrid Rules**: Combine percentage AND specific approver conditions
- **Mixed Workflows**: Support for both multi-level and conditional flows together

### 👔 Manager Capabilities
- View expenses pending approval
- Approve/reject with comments
- View team expense history
- Amounts displayed in company's default currency
- Escalate expenses per configured rules

### 🛠️ Admin Capabilities
- Company management (auto-created on signup)
- User management (create, update, delete)
- Role assignment and permissions
- Configure approval rules and workflows
- View all expenses across organization
- Override approvals when necessary

### 📊 Dashboard & Reporting
- Visual overview of expenses with charts
- Total expenses and category breakdowns
- Recent transaction history
- Date range filtering
- Pie charts and bar graphs for spending patterns

### 📱 Responsive Design
- Seamless experience across desktop, tablet, and mobile
- Clean, intuitive user interface
- Real-time updates

### 🤖 Advanced Features
- **OCR Receipt Processing**: Scan receipts to auto-generate expenses with:
  - Amount
  - Date
  - Description
  - Expense lines
  - Expense type
  - Merchant name
- **Real-Time Currency Conversion**: Automatic conversion to company currency
- **Multi-Currency Support**: Handle expenses in any currency

## 🏗️ Technical Architecture

### Frontend
- **React.js**: Component-based UI with state management
- **Redux**: Centralized state management
- **Styling**: React-Bootstrap, Material Icons
- **Effects**: TSParticles for dynamic backgrounds
- **Libraries**: react-datepicker, moment, unique-names-generator

### Backend
- **Node.js & Express.js**: RESTful API architecture
- **Authentication**: JWT-based secure authentication
- **Middleware**: Protected endpoints with role-based access

### Database
- **MongoDB**: NoSQL database for scalability
- **Mongoose**: ORM for schema definition and validation
- **Collections**: Users, Companies, Expenses, Approval Rules, Approvals

### External APIs
- **Country & Currency Data**: [REST Countries API](https://restcountries.com/v3.1/all)
- **Currency Conversion**: [Exchange Rate API](https://api.exchangerate-api.com/v4/latest/)

### Deployment
- **Frontend**: AWS Amplify
- **Backend**: Render
- **CI/CD**: Automated build and deployment pipelines

## 🚀 Getting Started

### Prerequisites
- Node.js (v14+)
- MongoDB
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/makadiyapreet/Sanskari_Coders_Odoo_hackathon
cd Expense-Tracker-App
```

2. **Setup Frontend**
```bash
cd frontend
npm install
```

3. **Setup Backend**
```bash
cd backend
npm install
```

### Environment Configuration

Create `backend/config/config.env` with:

```env
MONGO_URL=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_jwt_secret
EXCHANGE_RATE_API_KEY=your_api_key
```

### Running the Application

**Start Backend Server**
```bash
cd backend
npm run dev
```

**Start Frontend Server**
```bash
cd frontend
npm start
```

Access the application at `http://localhost:3000`

## 📸 Screenshots

<div align="center">

### Dashboard Overview
![Dashboard](https://i.postimg.cc/6qLR3WNt/Expense-Management-System-Brave-19-04-2023-11-08-53.png)

### Expense Submission
![Submission](https://i.postimg.cc/DynLNXqZ/Expense-Management-System-Brave-19-04-2023-11-08-59.png)

### Approval Workflow
![Approval](https://i.postimg.cc/Dy6L3wgc/Expense-Management-System-Brave-19-04-2023-11-15-46.png)

### Reports & Analytics
![Reports](https://i.postimg.cc/13YF47bn/Expense-Management-System-Brave-19-04-2023-11-15-54.png)

### Manager View
![Manager](https://i.postimg.cc/rwpWV2Z2/Expense-Management-System-Brave-19-04-2023-11-16-01.png)

</div>

## 🎭 User Roles & Permissions

| Role | Permissions |
|------|------------|
| **Admin** | Create company, manage users, set roles, configure approval rules, view all expenses, override approvals |
| **Manager** | Approve/reject expenses, view team expenses, escalate per rules, see expenses in company currency |
| **Employee** | Submit expenses, view own expenses, check approval status, scan receipts |

## 🛣️ Roadmap

- [ ] Mobile app (React Native)
- [ ] Budget tracking and alerts
- [ ] Integration with accounting software
- [ ] Advanced analytics and forecasting
- [ ] Bulk expense import/export
- [ ] Custom expense categories per company

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

[![Portfolio](https://img.shields.io/badge/Portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/Priyanshu9898/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/priyanshumalaviya/)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/Priyanshu2281)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@priyanshumalaviya9210)

## 🙏 Acknowledgments

- [REST Countries API](https://restcountries.com/) for country and currency data
- [Exchange Rate API](https://exchangerate-api.com/) for currency conversion
- [Excalidraw](https://excalidraw.com/) for UI mockups

---

<div align="center">

**⭐ Star this repo if you find it helpful!**

Made with ❤️ using MERN Stack

</div>
