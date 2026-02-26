# 🚀 VentureHub

### 🌐 A Multi-Role Startup–Investor–Manufacturer Networking Platform (Django)

<p align="center">

![Django](https://img.shields.io/badge/Django-4.x-green?style=for-the-badge\&logo=django)
![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey?style=for-the-badge\&logo=sqlite)
![Bootstrap](https://img.shields.io/badge/Frontend-Bootstrap-purple?style=for-the-badge\&logo=bootstrap)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

</p>

---

## 📌 Project Overview

**VentureHub** is a Django-based web platform designed to connect three key business stakeholders:

* 🚀 **Startups** – Seeking funding and manufacturing support
* 💰 **Investors** – Looking for high-potential ventures
* 🏭 **Manufacturers** – Partnering with scalable startups

The platform enables structured networking, investment applications, and business collaboration in a secure and role-based environment.

---

# 🎯 Core Objectives

* Build a multi-role authentication system
* Enable startup discovery and filtering
* Facilitate investment applications
* Provide structured connection workflows
* Simulate a real-world startup ecosystem platform

---

# 🏗️ System Architecture

```
VentureHub/
│
├── accounts/        # Authentication & user profiles
├── startups/        # Startup management module
├── investors/       # Investor interaction module
├── manufacturers/   # Manufacturer collaboration module
├── templates/       # Shared HTML templates
├── venturehub/      # Project configuration & settings
├── db.sqlite3       # Development database
└── manage.py        # Django management script
```

### 🔹 Architectural Highlights

* Role-based app modularization
* Separated business logic per stakeholder
* Django ORM-driven relational modeling
* Secure authentication handling
* Structured connection & approval workflow

---

# ✨ Key Features

## 🔐 Authentication System

* Separate registration & login for:

  * Startups
  * Investors
  * Manufacturers
* Django authentication framework
* Profile-based role identification
* Secure session management

---

## 🚀 Startup Module

* Register & login
* Manage detailed company profile
* Track investment applications
* View manufacturer connection requests
* Update startup stage, valuation & niche

---

## 💰 Investor Module

* Register & login
* Browse startups by niche & funding stage
* View startup valuation & details
* Apply for investment opportunities
* Manage submitted investment interests

---

## 🏭 Manufacturer Module

* Register & login
* Browse approved startups
* View startup contact information
* Connect via email or phone
* Track connection history
* Edit company profile

---

# 🔄 Platform Workflow

1️⃣ User selects role (Startup / Investor / Manufacturer)
2️⃣ Registers & logs in
3️⃣ Startups create and manage company profile
4️⃣ Investors browse and apply for investment
5️⃣ Manufacturers browse approved startups
6️⃣ Connections are initiated and tracked

---

# 🛠️ Tech Stack

## 🐍 Backend

* Django (Python)
* Django ORM

## 🎨 Frontend

* HTML
* Bootstrap
* Django Templates

## 🗄️ Database

* SQLite (Development)

---

# 🚀 Local Setup Guide

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/rahulbisht1301/final_project_aaah.git
cd final_project_aaah
```

## 2️⃣ Create Virtual Environment (Recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

## 3️⃣ Install Dependencies

```bash
pip install django
```

## 4️⃣ Apply Database Migrations

```bash
python manage.py migrate
```

## 5️⃣ Create Superuser (Optional)

```bash
python manage.py createsuperuser
```

## 6️⃣ Run Development Server

```bash
python manage.py runserver
```

Visit:

[http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

# 🌐 Application URLs

| Page               | URL                                                                                      |
| ------------------ | ---------------------------------------------------------------------------------------- |
| Home               | [http://127.0.0.1:8000/](http://127.0.0.1:8000/)                                         |
| Admin Panel        | [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)                             |
| Manufacturer Login | [http://127.0.0.1:8000/manufacturers/login/](http://127.0.0.1:8000/manufacturers/login/) |
| Startup Login      | [http://127.0.0.1:8000/startups/login/](http://127.0.0.1:8000/startups/login/)           |
| Investor Login     | [http://127.0.0.1:8000/investors/login/](http://127.0.0.1:8000/investors/login/)         |

---

# 🧪 Creating Sample Data

To add sample startups for testing:

```bash
python manage.py shell
```

```python
from startups.models import Startup

Startup.objects.create(
    name="TechVision AI",
    niche="Artificial Intelligence",
    stage="Series A",
    valuation=5000000,
    vision="Building next-gen AI solutions",
    status="APPROVED",
    email="contact@techvision.ai",
    phone="+1-555-0101"
)
```

---

# 📈 What This Project Demonstrates

* Multi-role Django architecture
* Business workflow modeling
* Secure authentication design
* Modular app separation
* Relational database handling
* Real-world startup ecosystem simulation

---

# 🔮 Future Enhancements

* Messaging system between stakeholders
* Funding analytics dashboard
* Role-based admin moderation panel
* Email notification integration
* Deployment on cloud (Render / Railway)
* REST API version using Django REST Framework

---

# 👨‍💻 Contributors

* Jeet Lohar – Backend & Admin Dashboard
* Rahul Bisht – Manufacturer Module & Messaging
* Rishabh Chaubey – Investor Module

---

## 👨‍💻 My Contribution
- Backend & Admin Dashboard Development
- Role-based authentication logic
- Database schema design
- Workflow implementation
- QA - Testing - Fixing

---

# ⭐ Why VentureHub Stands Out

Unlike simple CRUD applications, VentureHub models a real startup ecosystem with:

* Distinct stakeholder roles
* Structured approval workflows
* Investment & manufacturing collaboration logic
* Scalable modular architecture

It demonstrates practical backend development aligned with real-world business platforms.

---

# 📜 License

This project is licensed under the MIT License.
