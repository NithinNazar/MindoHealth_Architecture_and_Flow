# Mindo Health – UX Flow Diagrams (Phase 1)

This document defines the core UX flows for the Mindo Health platform.
All diagrams are written using GitHub-compatible Mermaid syntax.

---

## 1. User Onboarding and Booking Flow

```mermaid
flowchart TD

    A[Landing Page] --> B[Sign Up or Login]
    B --> C[Consent and Privacy Acceptance]
    C --> D[User Dashboard]
    D --> E[Find Expert]

    E --> F[Browse Experts]
    E --> G[Take Assessment]

    F --> H[Expert Profile]
    G --> H[Recommended Expert Profile]

    H --> I[Select Date and Time]
    I --> J[Payment]
    J --> K[Booking Confirmation]
    K --> L[Online Consultation]
```

---

## 2. Assessment Based Expert Matching Flow

```mermaid
flowchart TD

    A[Start Assessment] --> B[Assessment Instructions]
    B --> C[Answer Questions]
    C --> D[Submit Answers]
    D --> E[Matching Logic]
    E --> F[Recommended Experts]
    F --> G[Book Session]
```

---

## 3. Consultation Flow

```mermaid
flowchart TD

    A[Upcoming Session] --> B[Reminder Notification]
    B --> C[Join Session]
    C --> D[Waiting Room]
    D --> E[Video or Audio Consultation]
    E --> F[Session Ends]
    F --> G[Session Summary]
```

---

## 4. Professional Onboarding Flow

```mermaid
flowchart TD

    A[Professional Sign Up] --> B[Email or Phone Verification]
    B --> C[Create Professional Profile]
    C --> D[Upload Credentials]
    D --> E[Submit for Review]

    E --> F[Admin Review]
    F --> G[Approved]
    F --> H[Rejected]

    G --> I[Professional Dashboard Access]
    H --> J[Edit Profile and Resubmit]
```

---

## 5. Professional Session and Earnings Flow

```mermaid
flowchart TD

    A[Professional Dashboard] --> B[Upcoming Sessions]
    B --> C[Join Session]
    C --> D[Consultation Completed]
    D --> E[Earnings Updated]
    E --> F[Payout Processing]
```

---

## 6. Admin Role and Permission Management Flow

```mermaid
flowchart TD

    A[Admin Login] --> B[Admin Dashboard]
    B --> C[Roles and Permissions]
    C --> D[Create Role]
    D --> E[Assign Permissions]
    E --> F[Save Role]
    F --> G[Create Admin User]
    G --> H[Assign Role]
```
