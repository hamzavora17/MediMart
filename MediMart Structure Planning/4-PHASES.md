# MediMart — Development Phases

## Phase 1 — Project Setup

### Goal
Create the base Django project and connect MySQL.

### Work
- Install Python and Django.
- Create Django project.
- Configure MySQL.
- Configure templates, static files and media files.
- Configure environment variables.
- Initialize Git repository.
- Create initial apps.

### Deliverable
Running Django application with a working MySQL connection.

---

## Phase 2 — Authentication & User Management

### Goal
Build the foundation for all user roles.

### Work
- Registration page
- Login page
- Logout
- Password management
- Session handling
- Role-based access
- Profile page
- Saved addresses

### Roles
- Customer
- Doctor
- Lab Partner
- Pharmacy Partner
- Administrator

### Deliverable
Users can authenticate and reach the correct role-based area.

---

## Phase 3 — Base Layout & Dashboard

### Goal
Create the reusable UI shell.

### Work
- Header/navbar
- Footer
- Sidebar where required
- Responsive layout
- Customer dashboard
- Admin dashboard
- Provider dashboard foundations
- Flash/success/error messages

### Deliverable
Consistent responsive interface across the application.

---

## Phase 4 — Medicine & Product Catalog

### Goal
Build the main healthcare shopping module.

### Work
- Categories
- Product model
- Product listing page
- Product detail page
- Search
- Filters
- Brand
- Price
- Stock
- Prescription-required indicator
- Product images

### Deliverable
Customers can discover medicines and health products.

---

## Phase 5 — Cart & Orders

### Goal
Implement the complete medicine-order workflow.

### Work
- Add to cart
- Remove from cart
- Quantity updates
- Cart totals
- Address selection
- Order creation
- Order items
- Order history
- Order status
- Tracking page

### Deliverable
Customer can move from product discovery to a recorded order and track its status.

---

## Phase 6 — Prescription Management

### Goal
Handle prescription-required medicine workflows.

### Work
- Prescription upload
- Prescription list
- File validation
- Verification status
- Admin/pharmacy review
- Verify/reject workflow
- Connect prescription status with relevant order workflow

### Deliverable
Authorized staff can review prescriptions and customers can see their status.

---

## Phase 7 — Diagnostic Test Booking

### Goal
Build the laboratory booking workflow.

### Work
- Lab-test list
- Health packages
- Categories
- Test details
- Pricing
- Sample type
- Report ETA
- Slot selection
- Patient information
- Address/collection details
- Home sample collection workflow
- Booking status
- Report reference

### Deliverable
Customer can book a diagnostic test and later access its available report.

---

## Phase 8 — Doctor Consultation

### Goal
Build doctor discovery and consultation booking.

### Work
- Doctor profiles
- Specialization
- Verification status
- Consultation fee
- Availability
- Slot selection
- Booking
- Consultation status
- Customer/doctor consultation history

### Deliverable
Customers can discover doctors and book consultations.

---

## Phase 9 — Consultation Chat

### Goal
Support the documented private consultation messaging workflow.

### Work
- Consultation-specific message list
- Sender/recipient association
- Timestamp
- Message input
- Permission checks
- Consultation-based access control

### Deliverable
The customer and doctor can exchange messages within an authorized consultation.

---

## Phase 10 — Health Records & Reviews

### Goal
Centralize healthcare records and feedback.

### Work
- Health record listing
- Prescription record linking
- Lab report linking
- File access controls
- Record type/date
- Product ratings
- Product review comments
- Review moderation

### Deliverable
Customers have one account area for supported records and product feedback.

---

## Phase 11 — Administration & Partner Operations

### Goal
Complete centralized management.

### Work
- User management
- Provider management
- Category management
- Product management
- Inventory
- Prescription review
- Order management
- Lab-test management
- Lab-booking management
- Doctor/consultation management
- Reviews
- Reports/operational screens

### Deliverable
Administrators and partners can operate the platform from protected interfaces.

---

## Phase 12 — Validation, Security & Testing

### Goal
Make the application reliable and secure.

### Work
- Form validation
- Permission testing
- Authentication testing
- File-upload testing
- Order workflow testing
- Booking testing
- Database integrity testing
- Error handling
- Responsive UI testing
- Regression testing
- Bug fixing

### Deliverable
Stable academic release candidate.

---

## Phase 13 — Final Documentation & Presentation

### Goal
Prepare the project for submission.

### Work
- Final screenshots
- UML verification
- Database documentation
- Feature descriptions
- Installation instructions
- Testing summary
- GitHub repository cleanup
- Final presentation/demo

### Deliverable
Complete MediMart academic submission and demonstrable application.

## Recommended Build Order

```text
Setup
  ↓
Authentication
  ↓
Dashboard/Layout
  ↓
Products
  ↓
Cart
  ↓
Orders
  ↓
Prescriptions
  ↓
Lab Booking
  ↓
Doctors
  ↓
Consultation + Chat
  ↓
Health Records + Reviews
  ↓
Admin/Partners
  ↓
Testing & Security
  ↓
Documentation
```
