# MediMart — Architecture

## 1. Architecture Overview

MediMart follows a full-stack web architecture centered on **Python Django** with **MySQL** as the relational database.

High-level flow:

```text
Browser / User
      |
      v
HTML + Bootstrap + Tailwind CSS + JavaScript
      |
      v
Django URL Routing
      |
      v
Django Views / Forms / Services
      |
      v
Django ORM
      |
      v
MySQL Database

Uploaded Files
      |
      v
Media Storage
      |
      +--> Prescriptions
      +--> Lab Reports
      +--> Health Records
```

## 2. Application Flow

```text
User
  |
  +--> Register / Login
          |
          +--> Customer Dashboard
          |      +--> Products
          |      +--> Cart
          |      +--> Orders
          |      +--> Prescriptions
          |      +--> Lab Tests
          |      +--> Doctors
          |      +--> Consultations / Chat
          |      +--> Health Records
          |      +--> Reviews
          |
          +--> Doctor Area
          +--> Lab Partner Area
          +--> Pharmacy Partner Area
          +--> Admin Area
```

All protected areas should be controlled using Django authentication and role-based authorization.

## 3. Recommended Django App Structure

```text
medimart/
├── manage.py
├── requirements.txt
├── .env
├── .gitignore
│
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── accounts/
│   ├── migrations/
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── products/
│   ├── migrations/
│   ├── admin.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── orders/
│   ├── migrations/
│   ├── admin.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── prescriptions/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── labs/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── doctors/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── consultations/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── health_records/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── reviews/
│   ├── migrations/
│   ├── models.py
│   ├── urls.py
│   ├── views.py
│   └── tests.py
│
├── templates/
│   ├── base.html
│   ├── registration/
│   ├── accounts/
│   ├── products/
│   ├── orders/
│   ├── prescriptions/
│   ├── labs/
│   ├── doctors/
│   ├── consultations/
│   ├── health_records/
│   └── reviews/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
└── media/
    ├── prescriptions/
    ├── reports/
    └── health_records/
```

This is a recommended implementation structure. The documentation specifies Django apps/modules separated by business responsibility; it does not prescribe these exact app names.

## 4. Data Model Direction

Core entities documented for the system include:

- Users
- Addresses
- Categories
- Products
- Cart
- CartItems
- Orders
- OrderItems
- Prescriptions
- LabTests
- LabBookings
- Doctors
- Consultations
- Messages
- HealthRecords
- Reviews

These should be represented as Django models with appropriate foreign-key relationships and database constraints.

## 5. Technology Stack

### Frontend
- HTML
- Bootstrap
- Tailwind CSS
- JavaScript

### Backend
- Python
- Django
- Django ORM
- Django Models
- Forms
- Templates
- URL routing
- Migrations

### Database
- MySQL

### Version Control
- Git
- GitHub

## 6. Architectural Rules

- Keep presentation, business logic and data management separated.
- Keep Django apps focused on business responsibility.
- Use reusable templates/components.
- Keep views and service functions focused.
- Use Django ORM instead of unnecessary raw SQL.
- Use migrations for schema changes.
- Keep secrets and database credentials outside source code.
