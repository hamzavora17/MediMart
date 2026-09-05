# MediMart

> A full-stack web-based healthcare platform for medicines, health products, diagnostic tests, doctor consultations, prescriptions, and health records.

## 📌 Overview

**MediMart** is an academic full-stack healthcare platform developed to bring multiple healthcare-related services into one centralized web application.

The platform is designed to simplify healthcare workflows by allowing customers to discover medicines and health products, upload prescriptions, place medicine orders, book diagnostic tests, consult doctors, communicate through supported consultation chat, and access health records from a single account.

MediMart also provides role-based functionality for administrators, doctors/health experts, laboratory partners, and pharmacy partners.

## 🎯 Objectives

- Provide a single platform for medicines, health products, diagnostic tests, and doctor consultation.
- Simplify medicine and health-product discovery.
- Support prescription upload and verification.
- Enable diagnostic test and health-package booking.
- Enable doctor consultation and supported consultation chat.
- Maintain centralized health records and medical documents.
- Provide role-based access for different users and partners.
- Maintain structured and secure healthcare-related data.

## 👥 Target Users

### Customer / Patient
- Register and log in.
- Manage profile and saved addresses.
- Search medicines and health products.
- Browse categories and product details.
- Add products to cart and place orders.
- Upload prescriptions when required.
- Track orders and view order history.
- Book diagnostic tests and health packages.
- Book doctor consultations.
- Use consultation chat where supported.
- View prescriptions, lab reports, and health records.

### Administrator
- Manage users and roles.
- Manage doctors, laboratory partners, and pharmacy partners.
- Manage categories, products, inventory, and pricing.
- Review and verify prescriptions.
- Manage orders, lab tests, bookings, consultations, and reviews.
- Monitor reports and operational records.

### Doctor / Health Expert
- Maintain professional profile and specialization.
- Manage consultation availability.
- Manage consultation bookings.
- Communicate with customers through supported consultation chat.

### Laboratory Partner
- Manage diagnostic tests and health packages.
- Manage available appointment slots.
- Manage booking status.
- Manage completed report references.

### Pharmacy Partner
- Manage assigned product catalog and inventory.
- Review prescription-related orders.
- Update operational order status.

## ✨ Core Features

1. **User Authentication & Profile Management**
   - Registration, login, logout, password management, sessions, profiles, and saved addresses.

2. **Medicine & Health Product Catalog**
   - Categories, search, filters, product details, brands, pricing, stock availability, images, and prescription requirements.

3. **Cart & Order Management**
   - Add/remove products, quantity management, address selection, order creation, order history, and order tracking.

4. **Prescription Management**
   - Prescription upload, stored file references, verification status, and authorized review.

5. **Diagnostic Test Booking**
   - Test/package browsing, categories, pricing, sample information, appointment slots, home sample collection workflow, booking status, and report references.

6. **Doctor Consultation**
   - Doctor profiles, specializations, consultation fees, availability, booking, consultation status, and supported consultation messaging.

7. **Health Records**
   - Prescriptions, laboratory reports, uploaded healthcare documents, record types, and record dates.

8. **Reviews & Ratings**
   - Product ratings and optional customer comments with administrative moderation.

9. **Role-Based Access**
   - Separate permissions and workflows for customers, doctors, laboratories, pharmacies, and administrators.

10. **Administration**
   - Centralized management of users, providers, products, inventory, prescriptions, orders, tests, bookings, consultations, reviews, and operational records.

## 🛠️ Technology Stack

### Frontend
- HTML5
- CSS3
- Bootstrap
- Tailwind CSS
- JavaScript

### Backend
- Python
- Django
- Django ORM
- Django Forms
- Django Templates
- Django URL Routing
- Django Migrations

### Database
- MySQL

### Version Control
- Git
- GitHub

## 🏗️ Project Architecture

```text
MediMart
│
├── Frontend
│   ├── HTML
│   ├── Bootstrap
│   ├── Tailwind CSS
│   └── JavaScript
│
├── Backend
│   └── Python / Django
│
├── Database
│   └── MySQL
│
└── Core Modules
    ├── Authentication & User Management
    ├── Medicine & Product Catalog
    ├── Cart & Orders
    ├── Prescription Management
    ├── Laboratory Tests & Bookings
    ├── Doctor Consultation & Chat
    ├── Health Records
    ├── Reviews & Ratings
    └── Administration
```

## 🔄 Main Application Flow

```text
User
  │
  ├── Register / Login
  │
  ├── Customer
  │    ├── Browse/Search Products
  │    ├── Cart
  │    ├── Orders
  │    ├── Prescriptions
  │    ├── Lab Tests
  │    ├── Doctors
  │    ├── Consultations / Chat
  │    └── Health Records
  │
  ├── Doctor
  │    ├── Profile
  │    ├── Availability
  │    ├── Consultations
  │    └── Chat
  │
  ├── Lab Partner
  │    ├── Tests / Packages
  │    ├── Slots
  │    ├── Bookings
  │    └── Reports
  │
  ├── Pharmacy Partner
  │    ├── Products
  │    ├── Inventory
  │    ├── Prescriptions
  │    └── Orders
  │
  └── Administrator
       ├── Users
       ├── Products
       ├── Inventory
       ├── Prescriptions
       ├── Orders
       ├── Lab Tests / Bookings
       ├── Doctors / Consultations
       ├── Reviews
       └── Reports
```

## 📂 Recommended Project Structure

```text
MediMart/
├── manage.py
├── requirements.txt
├── .env
├── .gitignore
│
├── config/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── accounts/
├── products/
├── orders/
├── prescriptions/
├── labs/
├── doctors/
├── consultations/
├── health_records/
├── reviews/
│
├── templates/
├── static/
└── media/
```

## 🔐 Security

The project is designed to use Django's security mechanisms, including:

- Authentication
- Password hashing
- CSRF protection
- Role-based access control
- Server-side validation
- Protected file handling

Sensitive files such as prescriptions and medical reports should only be accessible to authorized users.

## 🚀 Development Approach

MediMart follows an Agile-oriented development approach in which the system is divided into manageable modules and implemented incrementally.

The planned development flow is:

```text
Project Setup
      ↓
Authentication & User Management
      ↓
Dashboard & Common UI
      ↓
Medicine & Product Catalog
      ↓
Cart & Order Management
      ↓
Prescription Management
      ↓
Diagnostic Test Booking
      ↓
Doctor Consultation
      ↓
Consultation Chat
      ↓
Health Records & Reviews
      ↓
Administration & Partner Operations
      ↓
Testing & Security
      ↓
Documentation & Final Presentation
```

## 🌿 Git Branch Strategy

The documented Git workflow uses:

```text
main
│
└── test-env
     │
     ├── feature/authentication
     ├── feature/products
     ├── feature/cart-orders
     ├── feature/prescriptions
     ├── feature/lab-booking
     ├── feature/doctor-consultation
     ├── feature/health-records
     └── feature/admin
```

- `main` → stable releases
- `test-env` → feature integration and testing
- `feature/*` → individual module development

Pull requests should be reviewed before merging feature work into `test-env`.

## 💻 Local Development Setup

### Prerequisites

Make sure the following are installed:

- Python
- MySQL
- Git

### Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd MediMart
```

### Create a Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file for sensitive configuration such as:

```env
SECRET_KEY=your-secret-key
DEBUG=True

DB_NAME=medimart
DB_USER=your-db-user
DB_PASSWORD=your-db-password
DB_HOST=localhost
DB_PORT=3306
```

> Never commit `.env` to GitHub.

### Apply Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### Create an Admin User

```bash
python manage.py createsuperuser
```

### Run the Development Server

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

## 🧪 Testing

Testing should be performed throughout development and should cover:

- Authentication and authorization
- Form validation
- Product search and filtering
- Cart calculations
- Order creation and status updates
- Prescription upload and verification
- Lab booking
- Doctor consultation booking
- Consultation messaging
- Health-record access
- Role-based permissions
- Database integrity
- Responsive UI

## 📌 Project Scope

### Included in the Core Academic Version

- Medicine and health-product discovery
- Cart and order workflow
- Prescription management
- Diagnostic test booking
- Doctor consultation
- Supported consultation chat
- Health records
- Product reviews and ratings
- Administration
- Partner management

### Future Enhancements

The project documentation identifies the following as future enhancements:

- Android and iOS mobile applications using Flutter
- Integrated online payment gateways such as Razorpay or Stripe
- AI-based health recommendations
- Real-time email, SMS, or push notifications
- Advanced security and privacy features
- Further performance and scalability improvements

## ⚠️ Disclaimer

MediMart is an academic software project.

It does not replace:

- Professional medical diagnosis
- Professional medical advice
- Physical laboratory procedures
- Actual medicine dispensing

The actual fulfillment of healthcare services depends on the relevant doctor, laboratory, pharmacy, and deployment environment.

## 👨‍💻 Contributors

| Name | Role |
|---|---|
| Kaushal Pithva | Backend Developer & Database Designer |
| Hamza Vora | Frontend Developer, UI/UX, Tester & Documentation Lead |

## 🎓 Academic Information

- **Project:** MediMart
- **Project Type:** Full-Stack Website
- **Department:** Department of Computer Applications
- **University:** LJ University
- **Program:** Master of Computer Application (Integrated)
- **Academic Year:** 2024–2027

## 📄 License

This project is developed for academic purposes.

No open-source license has been specified for this repository.
