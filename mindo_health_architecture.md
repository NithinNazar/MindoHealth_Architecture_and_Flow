# Mindo Health – Website Architecture (Phase 1)

---

## 1. Project Overview

Mindo Health is a fully online mental health platform connecting users with licensed therapists, psychologists, counselors, and related professionals.

The platform supports:

- Online audio/video consultations
- Direct expert selection
- Assessment-based expert matching
- Gig-based professionals
- Automated payments and payouts
- A dynamic, role-based admin panel

The system must comply with **HIPAA** and **GDPR** regulations.

---

## 2. High-Level System Architecture

### Frontend

- React + TypeScript
- Applications:
  - Public Website
  - User Dashboard
  - Professional Dashboard
  - Admin Panel

### Backend

- Python (Django + Django REST Framework)
- JWT-based authentication
- Dynamic role & permission engine

### Databases

- **PostgreSQL (Primary)**

  - Users
  - Professionals
  - Bookings
  - Payments & payouts
  - Roles & permissions
  - Consent records
  - Audit logs

- **MongoDB (Secondary)**
  - Assessments & questionnaires
  - Assessment responses
  - Non-clinical session metadata

### Third-Party Integrations

- Video/Audio: Agora or ZegoCloud
- Payments: Stripe (International), Razorpay (India)
- Notifications: Email, SMS, OTP
- Hosting: HIPAA-eligible cloud infrastructure

---

## 3. Authentication & Authorization

- Email/Password login
- Phone number + OTP
- JWT access & refresh tokens
- Role-based access control
- Permission-based API enforcement

---

## 4. Dynamic Roles & Permissions (Admin)

- Admins can create custom roles
- Each role has configurable permissions
- Permissions define dashboard visibility and API access
- No hard-coded admin roles (except super-admin)

---

## 5. Compliance & Security

### HIPAA

- Encrypted data at rest and in transit
- No PHI in logs
- Audit trails for sensitive actions

### GDPR

- Explicit consent collection
- Right to data access & deletion
- Data minimization principles

---

## 6. Phase 1 Scope

### Included

- Website
- Admin panel
- Booking & consultation
- Payments & payouts

### After Initial Launch

- AI Assistant (Text Based)
