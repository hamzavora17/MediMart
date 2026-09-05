# MediMart — DESIGN.md

## 1. Design Direction

MediMart should have a clean, modern, trustworthy healthcare-commerce interface based on the provided MediMart logo.

The logo establishes the visual identity:
- Primary brand color: Red
- Secondary brand color: Orange-red / coral
- Brand mark: Rounded medical cross / healthcare symbol
- Wordmark: MediMart
- Overall feel: Healthcare-focused, energetic, modern and trustworthy

The UI should support the logo rather than compete with it.

## 2. Logo Usage

Use the provided MediMart logo as the primary brand identity in:
- Navbar
- Login and registration
- Customer dashboard
- Admin dashboard
- Footer
- Favicon/browser assets where appropriate

Rules:
- Preserve original proportions.
- Never stretch or distort the logo.
- Do not change its colors.
- Maintain clear space around it.
- Prefer a transparent-background version.
- Use a compact mark on small screens when appropriate.

## 3. Brand Colors

The exact HEX values are recommended design choices based on the visual appearance of the supplied logo.

### Primary Red
`#EF1B2D`

Use for:
- Primary buttons
- Active navigation
- Main links
- Important actions
- Primary icons

### Coral / Orange-Red
`#FF5A3D`

Use for:
- Secondary accents
- Hover effects
- Decorative elements
- Promotional highlights
- Gradients

### Deep Red
`#C8102E`

Use for:
- Dark hover states
- Strong brand accents

### Brand Gradient

```css
linear-gradient(135deg, #FF5A3D 0%, #EF1B2D 100%)
```

Use sparingly for hero areas, special CTAs and promotional sections. Do not make the entire website red.

### Neutral Colors

| Purpose | Color |
|---|---|
| Page Background | `#FAFAFA` |
| Card / Surface | `#FFFFFF` |
| Primary Text | `#171717` |
| Secondary Text | `#666666` |
| Border | `#E5E5E5` |

## 4. Semantic Colors

| Purpose | Color | Examples |
|---|---|---|
| Success | `#16A34A` | Verified, Completed, Delivered |
| Warning | `#D97706` | Pending, Waiting |
| Error | `#DC2626` | Rejected, Cancelled, Errors |
| Information | `#2563EB` | Information, neutral status |
| Brand | `#EF1B2D` | Primary actions |

Do not use brand red for every status.

## 5. Theme

### Light Theme — Default

The core application should use a light theme:
- White cards
- Very light neutral backgrounds
- Red/orange brand accents
- Dark readable text
- Subtle borders
- Moderate shadows
- Professional rounded components

### Dark Theme

Dark mode is not required for the core academic version. If added later, maintain readable contrast and the MediMart brand identity.

## 6. Typography

The project documentation does not specify a font family.

### Recommended Font

**Inter**

Fallback:

```text
Inter, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
```

### Typography Scale

| Element | Size | Weight |
|---|---:|---:|
| Hero Heading | 36–44px | 700 |
| Page Heading | 28–36px | 700 |
| Section Heading | 22–28px | 600–700 |
| Card Heading | 18–20px | 600 |
| Body | 14–16px | 400 |
| Supporting Text | 12–14px | 400–500 |
| Buttons | 14–16px | 500–600 |

## 7. Logo-to-UI Relationship

Use red for:
- Login / Register
- Add to Cart
- Place Order
- Book Test
- Book Consultation
- Active navigation
- Important actions

Use coral/orange-red for:
- Hover states
- Secondary accents
- Promotional highlights
- Hero gradients

Use neutral colors for:
- Main backgrounds
- Product cards
- Tables
- Forms
- Medical information
- Long text

This prevents the strong red logo from overwhelming the interface.

## 8. Buttons

### Primary

```text
Background: #EF1B2D
Text: #FFFFFF
Border Radius: 8px
```

Use for important actions.

### Secondary

```text
Background: #FFFFFF
Text: #EF1B2D
Border: 1px solid #EF1B2D
Border Radius: 8px
```

### Destructive

Use semantic error red for destructive actions such as Delete, Reject and Cancel.

## 9. Navbar

Recommended structure:

```text
[ MediMart Logo ]  Home  Medicines  Lab Tests  Doctors  [Search]  [Cart]  [Account]
```

Guidelines:
- White background
- Logo on the left
- Clear navigation
- Red active state
- Subtle bottom border/shadow
- Responsive mobile navigation

## 10. Hero Section

Use:
- Light/white background
- Strong heading
- Supporting text
- Red primary CTA
- Outlined secondary CTA
- Optional subtle red/orange decorative elements

Do not make the entire hero solid red.

## 11. Product Cards

Display:
- Product image
- Product name
- Brand
- Price
- MRP where applicable
- Stock status
- Prescription requirement
- Rating where available
- Add-to-cart action

Recommended:
```text
Background: #FFFFFF
Border: #E5E5E5
Border Radius: 12px
Shadow: subtle
Primary Action: #EF1B2D
```

## 12. Healthcare Service Cards

Use consistent cards for:
- Diagnostic tests
- Health packages
- Doctors
- Consultations
- Health records

Every card should clearly communicate title, key information, status/availability and primary action.

## 13. Dashboard Design

### Customer Dashboard

```text
Welcome / Profile
        ↓
Quick Actions
        ↓
Recent Orders
        ↓
Prescription Status
        ↓
Upcoming Lab / Doctor Bookings
        ↓
Health Records
```

### Admin Dashboard

```text
Key Statistics
        ↓
Recent Orders
        ↓
Pending Prescriptions
        ↓
Lab Bookings
        ↓
Consultations
        ↓
Inventory Alerts
```

Keep dashboards information-focused and avoid unnecessary decoration.

## 14. Status Badges

Use consistent status treatment:
- Pending → Amber
- Confirmed → Blue
- Verified → Green
- Completed → Green
- Delivered → Green
- Dispatched → Blue
- Cancelled → Red
- Rejected → Red

Do not rely on color alone; include readable status text.

## 15. Forms

Forms should have:
- Visible labels
- Clear borders
- Required-field indicators
- Helpful validation feedback
- Consistent spacing
- Clear success/error messages

Recommended input:

```text
Background: #FFFFFF
Border: #DADADA
Focus Border: #EF1B2D
Border Radius: 8px
```

## 16. Prescription & Health Records

These screens should prioritize clarity and privacy.

Use:
- Document cards/list rows
- File type
- Upload date
- Verification status
- Authorized view/download actions
- Clear access restrictions

Avoid unnecessary decoration.

## 17. Spacing

Use a 4px-based scale:

```text
4px
8px
12px
16px
24px
32px
48px
64px
```

Recommended:
- Card padding: 16–24px
- Section spacing: 32–48px
- Page horizontal padding: 16–40px

## 18. Border Radius

```text
Inputs: 8px
Buttons: 8px
Cards: 12px
Large Panels: 16px
Status Pills: 999px
```

Keep the style professional rather than excessively rounded.

## 19. Shadows

Use subtle shadows only when they improve hierarchy:
- Cards: very subtle
- Dropdowns: moderate
- Modals: stronger

Avoid heavy shadows throughout the website.

## 20. Icons

Use one consistent icon style for:
- Search
- Cart
- User
- Medicine
- Lab tests
- Doctor
- Prescription
- Health records
- Orders
- Notifications
- Settings

Icons should support labels rather than replace important text.

## 21. Responsive Design

The website must support:
- Desktop
- Tablet
- Mobile browsers

### Desktop
Use multi-column layouts where useful.

### Tablet
Reduce columns and spacing.

### Mobile
- Mobile-friendly navigation
- Stack cards vertically
- Full-width forms
- Easy-to-tap CTAs
- Horizontally scrollable tables when necessary
- Readable product information

## 22. Accessibility

Use:
- Semantic HTML
- Proper heading hierarchy
- Visible labels
- Sufficient contrast
- Keyboard-accessible controls
- Descriptive buttons
- Alt text for meaningful images
- Clear validation messages

Do not rely on color alone for order, prescription, booking or consultation status.

## 23. Animation

Animations should be subtle and purposeful.

Allowed:
- Button hover transitions
- Card hover effects
- Modal transitions
- Loading indicators
- Small navigation transitions

Avoid:
- Excessive animations
- Long transitions
- Distracting background animations

Recommended transition duration:

```text
150–250ms
```

## 24. UX Priorities

On every major screen prioritize:

1. Search/discovery
2. Important healthcare information
3. Current status
4. Primary action
5. Supporting information

Example product-page priority:

```text
Product
  ↓
Price + Availability
  ↓
Prescription Requirement
  ↓
Quantity
  ↓
Add to Cart
  ↓
Details
```

## 25. Design Consistency Rules

Always:
- Use MediMart red consistently.
- Keep buttons consistent.
- Keep card styles consistent.
- Use the same spacing system.
- Use consistent status meanings.
- Keep typography consistent.
- Maintain responsive behavior.
- Preserve the logo exactly.

Avoid:
- Random colors
- Random fonts
- Multiple unrelated button styles
- Excessive gradients
- Excessive shadows
- Inconsistent border radii
- Cluttered layouts

## 26. Final Visual Identity

MediMart should communicate:

**Healthcare + Trust + Convenience + Modern E-commerce**

Visual formula:

```text
MediMart Logo
     +
Red / Orange-Red Brand Accents
     +
Clean White Surfaces
     +
Readable Dark Typography
     +
Simple Responsive Layout
     +
Clear Healthcare Workflows
```

The provided red/orange MediMart logo should remain the recognizable brand anchor throughout the application.
