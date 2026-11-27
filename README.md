# Audit Firm Management System

A desktop-based Audit Firm Management System developed using **C#, Windows Forms, and Microsoft SQL Server**. The application is designed to manage audit firm operations through role-based dashboards for CEO, Manager, and Auditor.

The system provides centralized management of users, auditors, projects, assignments, and audit reports.

## Project Overview

The Audit Firm Management System helps an audit organization manage its daily operations and coordinate activities among different organizational roles.

The application provides separate dashboards with role-based functionalities to ensure that users can perform their assigned tasks.

### Key Highlights

- Role-Based Login System
- Separate Dashboards for CEO, Manager, and Auditor
- User Management
- Auditor Management
- Project Management
- Assignment Management
- Audit Report Management
- Report Approval and Rejection
- SQL Server Database Integration
- Windows Forms Desktop Interface

## Technology Stack

| Technology | Purpose |
|---|---|
| C# | Main Programming Language |
| .NET Framework 4.8 | Application Framework |
| Windows Forms | Desktop User Interface |
| Microsoft SQL Server | Database Management |
| ADO.NET | Database Connectivity |
| SQL | Database Queries |
| Visual Studio | Development Environment |

## User Roles and Functionalities

### 1. CEO Dashboard

The CEO has access to the main management functionalities of the organization.

**Features:**
- User Management
- Create, Update, and Delete Users
- Project Management
- Create, Update, and Delete Projects
- Assignment Management
- Assign Tasks to Auditors
- Audit Report Management
- Approve Audit Reports
- Reject Audit Reports
- Dashboard Overview

### 2. Manager Dashboard

The Manager is responsible for managing auditors, projects, assignments, and audit reports.

**Features:**
- Auditor Management
- Add, Update, and Delete Auditors
- Project Management
- Assignment Management
- Assign Tasks to Auditors
- Audit Report Management
- Approve and Reject Reports
- Dashboard Overview

### 3. Auditor Dashboard

The Auditor dashboard allows auditors to manage their assigned work and submit audit reports.

**Features:**
- View Assigned Projects
- Assignment Management
- Create and Update Assignments
- Manage Assignment Status
- Submit Audit Reports
- View and Manage Reports
- Dashboard Overview

## Project Modules

| Module | Description |
|---|---|
| Authentication | User login and role-based dashboard access |
| User Management | Manage system users |
| Auditor Management | Manage auditor information |
| Project Management | Create and manage audit projects |
| Assignment Management | Create, assign, and track audit tasks |
| Report Management | Submit and manage audit reports |
| Report Approval | Approve or reject submitted reports |
| Dashboard | Display role-based management information |

## Project Architecture

The application follows a Windows Forms-based desktop architecture.

```text
Audit Firm Management System/
│
├── Program.cs
│
├── LoginPage.cs
├── LoginPage.Designer.cs
│
├── CEO_Dashboard.cs
├── CEO_Dashboard.Designer.cs
│
├── Manager_Dashboard.cs
├── Manager_Dashboard.Designer.cs
│
├── Auditor_Dashboard.cs
├── Auditor_Dashboard.Designer.cs
│
├── DataAccess.cs
│
├── App.config
│
├── Properties/
│   ├── AssemblyInfo.cs
│   ├── Resources.resx
│   ├── Resources.Designer.cs
│   └── Settings.settings
│
├── Database/
│   └── AuditFirm.bak
│
└── LoginPage.sln
```

## Database Management

The application uses **Microsoft SQL Server** as its database management system.

ADO.NET is used to establish database connectivity and execute SQL queries.

### Data Access Layer

The `DataAccess.cs` file handles database operations.

The main methods include:

- `ExecuteQuery()` – Executes SELECT queries and returns a DataSet.
- `ExecuteQueryTable()` – Executes SELECT queries and returns a DataTable.
- `ExecuteUpdateQuery()` – Executes INSERT, UPDATE, and DELETE queries.

### Database Backup

The repository includes a database backup file:

```text
Database/AuditFirm.bak
```

The database backup can be restored using SQL Server Management Studio (SSMS).

## Application Setup and Installation

Follow these steps to run the application locally.

### Prerequisites

- Microsoft Visual Studio
- .NET Framework 4.8
- Microsoft SQL Server
- SQL Server Management Studio (SSMS)

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the Project

Navigate to the downloaded project directory and open:

```text
LoginPage.sln
```

Open the solution using Microsoft Visual Studio.

### Step 3: Restore the Database

1. Open SQL Server Management Studio.
2. Connect to your SQL Server instance.
3. Restore the provided `AuditFirm.bak` database backup.
4. Make sure the restored database is named `AuditFirm`.

### Step 4: Configure Database Connection

Open `DataAccess.cs` and update the SQL Server connection string according to your local SQL Server configuration.

**Important:** Do not publish database usernames, passwords, or other sensitive credentials in a public repository.

### Step 5: Build the Application

In Visual Studio:

1. Open the solution.
2. Build the project.
3. Resolve any missing reference or configuration issues.

### Step 6: Run the Application

Press:

```text
F5
```

The application will launch with the Login Page.

## Application Workflow

The general application workflow is:

```text
          Login Page
               |
               v
       User Authentication
               |
       +-------+-------+
       |       |       |
       v       v       v
      CEO   Manager  Auditor
       |       |       |
       v       v       v
    User    Auditor  Projects
   Management Manage  |
       |       |      Assignments
       v       v       |
    Projects Projects  v
       |       |     Reports
       v       v
   Assignments Assignments
       |       |
       v       v
    Reports  Reports
       |       |
       v       v
   Approve / Reject
```

## Future Improvements

The following improvements can further enhance the application:

- Password Hashing and Secure Authentication
- Parameterized SQL Queries
- Improved Database Connection Management
- Enhanced Role-Based Authorization
- Advanced Search and Filtering
- Audit Trail and Activity Logging
- Export Reports to PDF and Excel
- Automated Backup and Recovery
- Improved Dashboard Analytics
- Better Exception Handling

## Learning Outcomes

Through this project, practical experience was gained in:

- C# Desktop Application Development
- Object-Oriented Programming
- Windows Forms Development
- SQL Server Database Management
- ADO.NET Database Connectivity
- CRUD Operations
- Role-Based Application Design
- Multi-User Management Systems
- Database-Driven Application Development

## Author

**MD Shakib Hasan Shafin**

Computer Science & Engineering

**Project:** Audit Firm Management System

---

⭐ If you find this project interesting, feel free to explore the repository.

**Developed using C#, Windows Forms, .NET Framework 4.8, ADO.NET, and Microsoft SQL Server.**
