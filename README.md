# Python API - HRMS (Backend)

This is the core backend engine for the HRMS system, built with **Django** and **Django REST Framework (DRF)**. It provides secure JWT-based authentication and modular services for employee management.

---

## 🌐 Live URLs

### 🖥️ Frontend (Production)

👉 https://hrms.trafficvenue.co.in

```bash
#### Credentials For login ####

username: admin@123
password: admin@123
```

### 🔐 Backend API (Production)

👉 https://backend.hrms.trafficvenue.co.in

### 🐍 Backend Source Code (Django API)

👉 https://github.com/Sagarsharma12345/python-api-hrms

### ⚛️ Frontend Source Code (React UI)

👉 https://github.com/Sagarsharma12345/react-ui-hrms

### 🛠️ Local Development Environment

```bash
Frontend [React (Vite)]: http://localhost:5173/
Backend [Django]: http://localhost:8000/
```

## Tech Stack

- **Language:** Python 3.10+
- **Framework:** Django 5.x
- **API Toolkit:** Django REST Framework
- **Auth:** SimpleJWT
- **Middleware:** Django-CORS-Headers

---

## Setup & Installation (For New Developers)

### 1. Clone the Repository

```bash
git clone https://github.com/Sagarsharma12345/python-api-hrms.git
cd python-api-hrms
```

### 2. Virtual Environment Setup

```bash
# Create Virtual Environment
python -m venv venv

# Activate (Windows)
.\venv\Scripts\activate

# Activate (Linux/macOS)
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install django djangorestframework djangorestframework-simplejwt django-cors-headers
```

### 4. Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Start Development Server

```bash
python manage.py runserver
API Access: http://127.0.0.1:8000/
```

## Project Structure

```bash
core/: Global settings & URL routing.
accounts/: User authentication, roles, and permissions.
employees/: Employee lifecycle and data management.
attendance/: Check-in/out and leave tracking logic.
```

## For Production

```
passenger_wsgi.py
```

## API End Point

Method, Endpoint, Description

POST /api/login/
POST /api/logout/

GET, /api/employees, Fetch all employees
POST, /api/employees, Add a new employee
DELETE, /api/employees/:id, Remove an employee

GET, /api/attendance, Get all attendance records
POST, /api/attendance, Mark attendance for an employee

## ✨ Functional Requirements Covered

### 1. Employee Management

- **Add Employee:** Form with fields for Unique ID, Name, Email, and Department.
- **Validation:** Prevents duplicate Employee IDs and invalid email formats.
- **List View:** A clean, searchable table of all employees.
- **Delete:** Remove employee records instantly.

### 2. Attendance Management

- **Mark Status:** Toggle between "Present" and "Absent" for any date.
- **History:** View specific attendance logs for each employee.
- **Bonus:** Automated count of "Total Present Days" for each staff member.

### 3. Dashboard (Bonus Feature)

- **Summary Cards:** Quick stats for Total Employees and Today's Attendance.
- **Analytics:** Visual charts showing attendance trends.

---
