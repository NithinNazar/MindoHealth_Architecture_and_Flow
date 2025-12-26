# Mindo Health – UX Flow Diagrams (Phase 1)

---

## 1. User Onboarding & Booking Flow

```mermaid
flowchart TD
    A[Landing Page] --> B[Sign Up / Login]
    B --> C[Consent & Privacy Acceptance]
    C --> D[User Dashboard]
    D --> E{Find Expert}
    E -->|Browse Experts| F[Expert Listing]
    E -->|Take Assessment| G[Assessment]
    F --> H[Expert Profile]
    G --> H[Recommended Expert Profile]
    H --> I[Select Date & Time]
    I --> J[Payment]
    J --> K[Booking Confirmation]
    K --> L[Online Consultation]



flowchart TD
    A[Start Assessment] --> B[Instructions]
    B --> C[Questionnaire]
    C --> D[Submit Answers]
    D --> E[Matching Logic]
    E --> F[Recommended Experts]
    F --> G[Book Session]



flowchart TD
    A[Upcoming Session] --> B[Reminder Notification]
    B --> C[Join Session]
    C --> D[Waiting Room]
    D --> E[Video / Audio Consultation]
    E --> F[Session Ends]
    F --> G[Session Summary]


flowchart TD
    A[Professional Sign Up] --> B[Verification]
    B --> C[Create Profile]
    C --> D[Upload Credentials]
    D --> E[Submit for Review]
    E --> F{Admin Decision}
    F -->|Approved| G[Dashboard Access]
    F -->|Rejected| H[Feedback & Edit]


flowchart TD
    A[Admin Login] --> B[Dashboard]
    B --> C[Roles & Permissions]
    C --> D[Create Role]
    D --> E[Assign Permissions]
    E --> F[Save Role]
    F --> G[Create Admin User]
    G --> H[Assign Role]
```
