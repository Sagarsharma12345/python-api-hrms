# Python API - HRMS (Backend)

This is the core backend engine for the HRMS system, built with **Django** and **Django REST Framework (DRF)**. It provides secure JWT-based authentication and modular services for employee management.

---

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
