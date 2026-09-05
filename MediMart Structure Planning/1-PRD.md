# MediMart — Product Requirements Document

## 1. Product Overview

MediMart is a web-based healthcare platform that combines medicine and health-product discovery, 
prescription handling, diagnostic test booking, doctor consultation, consultation chat, health records, 
and centralized administration in one application.

The project is an academic full-stack website designed to simplify fragmented healthcare workflows 
through a single responsive web interface.

## 2. What to Build

Build a Django-based healthcare web application with these major modules:

1. User authentication and profile management
2. Medicine and health-product catalog
3. Search, category navigation and filtering
4. Cart and medicine order management
5. Prescription upload and verification
6. Diagnostic test and health-package booking
7. Doctor consultation and supported consultation chat
8. Health-record and medical-document management
9. Product reviews and ratings
10. Administration and partner management

## 3. Targeted Users

### Customer / Patient
- Register, log in and manage profile.
- Manage saved addresses.
- Search and browse medicines/products.
- Manage cart and place orders.
- Upload prescriptions.
- Track orders.
- Book diagnostic tests.
- Book doctor consultations.
- Chat with doctors where supported.
- View prescriptions, reports and health records.

### Administrator
- Manage users and roles.
- Manage doctors, labs and pharmacy partners.
- Manage categories, products, inventory and pricing.
- Review prescriptions.
- Manage orders, tests, bookings, consultations and reviews.
- View reports and operational information.

### Doctor / Health Expert
- Maintain professional profile and specialization.
- Manage consultation availability.
- Manage consultation bookings.
- Communicate with customers through supported chat.

### Laboratory Partner
- Manage tests/packages.
- Manage available slots.
- Manage booking status.
- Link/upload completed reports.

### Pharmacy Partner
- Manage assigned products and inventory.
- Review prescription-related orders.
- Update operational order status.

## 4. Core Features

### Authentication
- Registration, login and logout
- Password management
- Session handling
- Role-based authorization
- Profile and address management

### Medicine & Product Catalog
- Categories
- Product search
- Filters
- Product details
- Brand, price and stock
- Prescription-required flag
- Product images and descriptions

### Cart & Orders
- Add/remove cart items
- Update quantities
- Calculate totals
- Select delivery address
- Place orders
- Order history
- Order tracking

Supported order statuses: Pending, Confirmed, Dispatched, Delivered, Cancelled.

### Prescription Management
- Upload prescription
- Store file reference
- View status
- Authorized review
- Verify/reject prescription

### Diagnostic Tests
- Browse tests and packages
- Category filters
- Pricing and sample type
- Appointment-slot selection
- Patient/address information
- Home sample-collection workflow
- Booking status
- Report reference

### Doctor Consultation
- Doctor profiles
- Specializations
- Consultation fee
- Available slots
- Consultation booking
- Consultation status
- Private chat/message exchange

### Health Records
- Prescriptions
- Lab reports
- Uploaded healthcare documents
- Record date/type
- Customer account access

### Reviews
- Product rating from 1–5
- Optional comments
- Administrative moderation

### Administration
- Users and roles
- Providers
- Categories/products
- Inventory
- Prescriptions
- Orders
- Lab tests/bookings
- Consultations
- Reviews
- Reports and operational records

## 5. Success Criteria

The academic core is complete when customers can authenticate, search products, manage a cart, 
place/track orders, upload prescriptions, book tests and consultations, access health records, 
and when administrators can manage the major modules with role-based access.

## 6. Boundaries

The core academic version does **not** require actual medicine dispensing, physical laboratory procedures, 
professional medical diagnosis, or advanced external payment/notification infrastructure.

The documentation lists mobile apps, online payment gateways, AI recommendations, real-time notifications, 
stronger security infrastructure, and advanced scalability as future enhancements rather than core requirements.
