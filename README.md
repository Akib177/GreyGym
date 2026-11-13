# 🏋️ GreyGym – Gym Management System

GreyGym is a database-driven gym management system designed to streamline the daily operations of a fitness center by managing users, trainers, memberships, workouts, diet plans, equipment, incidents, and payments in an organized and efficient manner.

The system supports multiple user roles, including **Admin, Trainer, Employee, and Customer**, each with role-based access and responsibilities. GreyGym is built as a Windows Forms application using **C#** with **SQL Server** as the backend database.

---

## 📌 Features

### 👤 User Management
- Role-based login (Admin, Trainer, Employee, Customer)
- Secure authentication
- Centralized user information storage

### 🏋️ Trainer & Customer Management
- Assign trainers to customers
- Trainers can view and manage only their assigned customers
- Track training assignments and schedules

### 📋 Workout & Diet Plans
- Admin can create workout and diet plans
- Trainers can assign or update workouts for customers
- Customers can view assigned workout and diet plans

### 💳 Payment & Package Management
- Gym packages with duration and pricing
- Payment tracking with confirmation status
- Automatic package activation after payment approval

### 🏢 Gym Operations
- Gym equipment management
- Incident reporting and resolution
- Membership tracking

---

## 🛠️ Tech Stack

- **Frontend:** C# (Windows Forms)
- **Backend:** SQL Server
- **Database Access:** ADO.NET (SqlConnection, SqlCommand, DataAdapter)
- **IDE:** Visual Studio
- **Version Control:** Git & GitHub


---

## 🗄️ Database Design

The project uses a normalized SQL Server database with key tables such as:

- `UserInfo`
- `TrainerUser`
- `Packages`
- `WorkoutPlan`
- `DietPlan`
- `Payment`
- `UserPackage`
- `GymEquipment`
- `IncidentReports`

All table schemas and sample data scripts are included in the repository.

📂 **Database Files**
- `schema.sql` – Table creation scripts
- `data.sql` – Sample insert queries

---

## ▶️ How to Run the Project

### 1️⃣ Database Setup
1. Open **SQL Server Management Studio (SSMS)**
2. Create a new database (e.g., `GreyGym`)
3. Run `schema.sql`
4. Run `data.sql`

### 2️⃣ Application Setup
1. Open the project in **Visual Studio**
2. Update the SQL connection string in: ApplicationHelper.cs
3. Build and run the project

---

## 🧪 Sample Login Roles

| Role      | Access Level |
|-----------|--------------|
| Admin     | Full system control |
| Trainer   | Assigned customers only |
| Employee  | Payments & user support |
| Customer  | View workouts, diet, payments |

---

## 👨‍💻 Maintainer

**Adnan Akib**  
GitHub: https://github.com/Akib177

📥 **Project Download**  
Clone the repository

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!  
Feel free to open an issue or submit a pull request to help improve the project.

---

## 📄 License

This project is open-source and available under the **MIT License**.  
You are free to use, modify, and distribute this project with proper attribution.

