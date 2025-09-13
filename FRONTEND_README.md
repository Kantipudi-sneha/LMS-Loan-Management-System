
# Loan Management System - Frontend

A modern, responsive **Angular frontend** for the Loan Management System backend built with **Spring Boot**.

---

## 🚀 Features

### 🔐 Authentication & Security
- JWT-based authentication
- Role-based access control (User/Admin)
- Secure password handling
- Protected routes with route guards

### 👥 User Management
- User registration with form validation
- User login/logout functionality
- Profile management
- Password change functionality

### 🏦 Loan Management
- Loan application submission
- Loan status tracking
- EMI schedule management
- Payment management

### 👨‍💼 Admin Panel
- Admin registration and login
- User management (activate/deactivate/delete)
- Loan application review and approval
- System statistics and monitoring

### 🎨 Modern UI/UX
- Responsive design with **Bootstrap 5**
- Clean and user-friendly interface
- Mobile-friendly layout

---

## 🛠 Prerequisites

Make sure you have the following installed:

- **Node.js** (v18 or higher)
- **npm** (comes with Node.js)
- **Angular CLI** (v17 or higher)
- **Backend Server** running on `http://localhost:8080`

---

## ⚙️ Installation

1. **Navigate to the project folder:**
   ```bash
   cd FINAL_FE
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Install Angular CLI globally (if not installed):**
   ```bash
   npm install -g @angular/cli
   ```

---

## 🔧 Configuration

### Backend Connection
Ensure the backend is running at `http://localhost:8080`.  
Update the environment file (`environment.ts`) if necessary.

### CORS
The backend must allow requests from `http://localhost:4200`.

---

## ▶️ Running the Application

### Development Mode
```bash
ng serve
```
App will run at: [http://localhost:4200](http://localhost:4200)

### Production Build
```bash
ng build
```
Files will be generated in the `dist/` folder.

---

## 📂 Project Structure

```
src/
├── app/
│   ├── components/          # UI Components
│   │   ├── auth/            # Authentication components
│   │   ├── home/            # Landing page
│   │   ├── user/            # User-specific components
│   │   └── admin/           # Admin-specific components
│   ├── services/            # Business logic services
│   ├── models/              # TypeScript interfaces
│   ├── guards/              # Route protection
│   └── interceptors/        # HTTP interceptors
├── assets/                  # Static files
└── styles.css               # Global styles
```

---

## 🌐 Key Components

### Authentication
- **LoginComponent** – User login form
- **RegisterComponent** – User registration form
- **AdminLoginComponent** – Admin login
- **AdminRegisterComponent** – Admin registration

### User Features
- **UserDashboardComponent** – Overview of loans
- **UserProfileComponent** – Profile management
- **UserLoansComponent** – View applied loans
- **ApplyLoanComponent** – Apply for a new loan
- **UserPaymentsComponent** – Manage payments

### Admin Features
- **AdminDashboardComponent** – Overview with stats
- **ManageUsersComponent** – Manage users
- **ManageLoansComponent** – Review loan applications
- **ReportsComponent** – Generate system reports

---

## 🧪 Services

- **AuthService** – Handles authentication & JWT token management
- **LoanService** – Manages loan applications & EMI schedules
- **PaymentService** – Handles payments and penalties
- **AdminService** – Admin operations like user and loan management

---

## 🔒 Security

- **Route Guards** – Protect sensitive routes
- **HTTP Interceptors** – Add JWT to API requests
- **Token Management** – Secure handling of authentication tokens

---

## 🗄 API Integration

### Authentication
- `POST /user/register` – Register a new user
- `POST /user/login` – Login for users
- `POST /admin/register` – Register a new admin
- `POST /admin/login` – Login for admins

### Loan Management
- `POST /api/loans/apply` – Apply for a loan
- `GET /api/loans` – Fetch loans
- `PUT /api/loans/{id}/status` – Update loan status

### Admin Operations
- `GET /admin/users` – Fetch all users
- `PUT /admin/users/{id}/activate` – Activate user
- `PUT /admin/users/{id}/deactivate` – Deactivate user

---

## 🎨 Styling

- **Bootstrap 5** for layout and responsiveness
- **Font Awesome** for icons
- Custom gradients and animations

---

## 🌱 Future Enhancements

- Integration with a real **Payment Gateway**
- Advanced **Analytics Dashboard**
- **Microservices architecture** migration
- Deployment to cloud platforms like **AWS**

---

## 🐞 Troubleshooting

### Backend Connection Error
- Ensure backend runs on port `8080`
- Verify CORS settings

### JWT Token Issues
- Clear browser localStorage and re-login
- Check token validity

### Build Errors
- Clear `node_modules` and reinstall:
  ```bash
  rm -rf node_modules && npm install
  ```
- Update Angular CLI:
  ```bash
  npm update -g @angular/cli
  ```

---

## 🤝 Contributing

1. Follow Angular coding standards
2. Write clean and maintainable code
3. Use TypeScript interfaces properly
4. Test on multiple browsers before pushing changes

---

## 📜 License

This project is part of the **Loan Management System** and follows the same license as the backend.

---

## 💬 Support

For support or questions:
- Check backend documentation
- Visit Angular official docs
- Use browser console & DevTools for debugging
