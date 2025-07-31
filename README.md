<a id="top"></a>

# 🎬 Yamdb API — Reviews & Ratings Platform

[![Python](https://img.shields.io/badge/Python-3.8.3-blue.svg)](https://python.org)
[![Django](https://img.shields.io/badge/Django-2.2.16-green.svg)](https://djangoproject.com)
[![DRF](https://img.shields.io/badge/DRF-3.12.4-red.svg)](https://www.django-rest-framework.org/)

> A powerful REST API platform for collecting reviews and building ratings for creative works across multiple categories.

## 📖 Description

Yamdb API is a comprehensive platform designed for users to share reviews and create ratings for various creative works. The platform supports multiple categories including **Books**, **Movies**, and **Music**, with the ability to expand or modify categories through the admin interface.

### ✨ Key Features

- **📝 Review System**: Users can write detailed reviews and rate works
- **💬 Comment System**: Engage with other users' reviews through comments
- **🔐 JWT Authentication**: Secure token-based authentication system
- **👥 User Roles**: Four distinct access levels (Anonymous, User, Moderator, Admin)
- **📊 Rating System**: Comprehensive rating and review aggregation
- **🔒 Role-Based Access**: Granular permissions for different user types

### 🎯 User Access Levels

| Role | Read Access | Write Reviews | Moderate Content | Admin Access |
|------|-------------|---------------|------------------|--------------|
| **Anonymous** | ✅ | ❌ | ❌ | ❌ |
| **User** | ✅ | ✅ | ❌ | ❌ |
| **Moderator** | ✅ | ✅ | ✅ | ❌ |
| **Admin** | ✅ | ✅ | ✅ | ✅ |

## 🛠 Technologies

- **Python 3.8.3** - Core programming language
- **Django 2.2.16** - Web framework
- **Django REST Framework 3.12.4** - API framework
- **PyJWT 2.1.0** - JSON Web Token authentication

📋 **Complete dependency list**: [`requirements.txt`](requirements.txt)

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- Git
- Virtual environment tool

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone git@github.com:andrey-kolesnik-moscow/Yamdb_API.git
   cd Yamdb_API
   ```

2. **Create and activate virtual environment**
   
   **For Windows:**
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```
   
   **For macOS/Linux:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run database migrations**
   ```bash
   python3 manage.py migrate
   ```

5. **Import sample data (optional)**
   ```bash
   python3 manage.py import_csv
   ```

6. **Start the development server**
   ```bash
   python3 manage.py runserver
   ```

### 📚 API Documentation

Once the server is running, you can access the interactive API documentation at:

- **ReDoc**: `http://localhost:8000/redoc/`
- **Swagger UI**: `http://localhost:8000/swagger/`

## 🔐 Authentication

The API uses JWT (JSON Web Token) authentication:

1. **Register** with your username and email
2. **Verify** your email with the confirmation code
3. **Receive** a JWT token for authenticated access
4. **Use** the token in the `Authorization: Bearer <token>` header

## 📁 Project Structure

```
Yamdb_api/
├── api_yamdb/          # Main Django project
│   ├── api/           # Core API functionality
│   ├── reviews/       # Reviews and ratings app
│   ├── users/         # User management app
│   └── static/        # Static files and data
├── tests/             # Test suite
└── requirements.txt   # Dependencies
```

## 🧪 Testing

Run the test suite to ensure everything works correctly:

```bash
python -m pytest
```

## 👥 Contributors

- **Andrey Kolesnik** - Project Lead
- **Georgy Kuznetsov** - Backend Development
- **Pavel Firsov** - API Design

---

<div align="center">

[⬆️ Back to Top](#top)

</div>

