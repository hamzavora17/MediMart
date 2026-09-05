# MediMart — Development Rules

## 1. Required Technologies

Use the technology stack defined in the MediMart documentation:

- Python
- Django
- MySQL
- HTML
- Bootstrap
- Tailwind CSS
- JavaScript
- Git
- GitHub

Django should remain the main backend framework.

## 2. Libraries / Framework Guidance

Prefer Django's built-in facilities first:

- Django Authentication
- Django Forms
- Django ORM
- Django Admin
- Django validation
- Django CSRF protection
- Django file handling
- Django messages framework

Use additional third-party libraries only when a concrete project requirement needs them. Do not add dependencies simply because they are popular.

## 3. Password & Authentication Rule

Use Django's built-in authentication and password-hashing mechanisms.

Do **not** implement custom password hashing for the application.

All login-protected actions must use Django authentication and appropriate authorization checks.

## 4. Database Rules

- Use Django models and migrations.
- Use meaningful field names.
- Use foreign keys for relationships.
- Preserve data integrity with database constraints where appropriate.
- Prefer Django ORM queries.
- Avoid unnecessary raw SQL.
- Do not manually edit production database tables when a migration should be used.

## 5. Coding Standards

### Naming
- Python classes/models: `PascalCase`
- Functions/variables: `snake_case`
- Constants: `UPPER_SNAKE_CASE`
- Database fields: clear, descriptive names
- JavaScript variables: consistent descriptive naming

### Structure
- Keep functions concise.
- Follow Single Responsibility.
- Avoid duplicate code.
- Use reusable templates/components.
- Keep complex business logic out of HTML templates.
- Maintain separation of concerns.

## 6. Error Handling

Every user-facing workflow should fail safely.

### Expected approach
1. Validate user input.
2. Check authentication and permissions.
3. Check database/resource existence.
4. Perform the operation inside appropriate transaction boundaries where data consistency matters.
5. Return a clear user-facing message.
6. Log unexpected server-side failures.

### Do not
- Show raw Python/Django tracebacks to users.
- Expose database credentials or secrets.
- Silently ignore failed operations.
- Trust only client-side validation.

Use both client-side feedback and server-side validation, with server-side validation treated as authoritative.

## 7. File Upload Rules

Prescription and healthcare documents require special care.

- Validate file type and size.
- Store uploaded files through controlled media handling.
- Do not trust the original filename.
- Restrict access to authorized users.
- Do not expose private records through unrestricted public URLs.
- Store file references in database records.
- Keep uploaded health documents separate from normal public static assets.

## 8. Security Rules

Use Django mechanisms for:

- Authentication
- Password hashing
- CSRF protection
- Access control
- Server-side validation
- Protected file handling

Role checks must prevent customers from accessing administrative/provider operations.

## 9. What to Avoid

Avoid:

- Unnecessary frameworks or databases.
- Hard-coded secrets.
- Custom authentication when Django authentication is sufficient.
- Custom password hashing.
- Raw SQL for routine CRUD operations.
- Business logic inside templates.
- Duplicate model logic.
- Unvalidated file uploads.
- Client-only authorization.
- Exposing health records to unauthorized users.
- Implementing future enhancements before the core requirements are stable.

## 10. AI Boundaries

AI may be used as a development assistant for:

- Explaining code.
- Generating boilerplate.
- Suggesting UI structure.
- Helping write tests.
- Helping debug development errors.
- Drafting documentation.
- Suggesting refactoring.

AI must not be treated as the authority for:

- Medical diagnosis.
- Medical treatment decisions.
- Prescription approval.
- Professional healthcare advice.
- Security-critical decisions without human review.
- Automatically making clinical decisions.

Any AI-generated code must be reviewed, tested and integrated deliberately by the developer.

## 11. Future Features Rule

These are future enhancements in the documentation and should not be treated as mandatory core features:

- Flutter Android/iOS application
- Razorpay or Stripe payment integration
- AI health recommendations
- Real-time email/SMS/push notifications
- Advanced security/privacy infrastructure
- Large-scale performance/scalability infrastructure

The core web application should be completed first.
