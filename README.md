# Loan Management System (LMS) 💰

A **Full-Stack Loan Management System** built to manage loan applications, approvals, EMI schedules, payments, and penalties.
This project demonstrates **secure authentication**, **role-based access control**, and **real-time data retrieval** using modern web technologies.

---

## 🚀 Features

* **User & Admin Authentication** using JWT (JSON Web Token)
* **Role-based access control** (`USER` & `ADMIN`) with Spring Security
* **Automatic data retrieval** for EMI and payment details using **EMI ID** and **User ID**
* REST APIs for:
  * Loan application & approval
  * EMI scheduling & payments
  * Loan disbursements & penalties
* **Secure logout handling** using token blacklisting
* Backend testing with **JUnit and Mockito**
* API testing with **Postman**
* Clean dependency management with **Maven**

---

## 🛠 Tech Stack

| **Category**          | **Technologies Used**                                                   |
| --------------------- | ----------------------------------------------------------------------- |
| **Frontend**          | HTML, CSS, JavaScript, Angular                                          |
| **Backend**           | Java, Spring Boot, Spring Framework, Spring Data JPA, Hibernate, Lombok |
| **Security**          | Spring Security, JWT                                                    |
| **Database**          | MySQL                                                                   |
| **Testing**           | JUnit, Mockito, Postman                                                 |
| **Build Tool**        | Maven                                                                   |
| **Development Tools** | IntelliJ IDEA, VS Code                                                  |
| **Architecture**      | Monolithic                                                              |


## 📂 Project Structure

```
Loan-Management-System/
├── backend/                   # Backend (Spring Boot)
│   ├── src/
│   │   ├── main/java/com/module/
│   │   ├── main/resources/
│   │   └── test/java/          # Unit tests
│   └── pom.xml                 # Maven build file
│
├── frontend/                  # Frontend (Angular)
│   ├── src/
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation & Setup

### **Backend Setup (Spring Boot)**

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/loan-management-system.git
   ```
2. Navigate to the backend folder:

   ```bash
   cd backend
   ```
3. Update **MySQL configuration** in `application.properties`:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/lms
   spring.datasource.username=your_mysql_username
   spring.datasource.password=your_mysql_password
   ```
4. Run the backend:

   ```bash
   mvn spring-boot:run
   ```

---

### **Frontend Setup (Angular)**

1. Navigate to the frontend folder:

   ```bash
   cd frontend
   ```
2. Install dependencies:

   ```bash
   npm install
   ```
3. Start the Angular app:

   ```bash
   ng serve
   ```
4. Open in browser:
   [http://localhost:4200](http://localhost:4200)

---

## 🌱 Future Enhancements

* Migrating to **Microservices Architecture** for better scalability
* **Integrating a payment gateway** for real-world transactions
* Adding **analytics dashboards** for better financial insights
* Deploying to cloud platforms like **AWS** or **Azure**
