# Application Workflow

## 1. Entry Point

The user visits the **RK Health** web application using a desktop, tablet, or mobile browser.

---

## 2. Authentication

### New User

- Click **Register**
- Enter personal details (Name, Email, Password, Phone Number)
- Create an account
- Redirect to the Login page

### Existing User

- Click **Login**
- Enter registered Email and Password
- Successfully authenticate
- Redirect to the Home Dashboard

---

## 3. Home Dashboard

The dashboard serves as the central hub for healthcare management.

Users can:

- View upcoming appointments
- Check medication reminders
- Monitor dashboard statistics
- View recent healthcare activities
- Access AI-generated health summaries
- Generate health reports

---

## 4. Appointment Management

Users can:

- Add a new doctor appointment
- Enter doctor name
- Select appointment date and time
- Add visit notes
- Edit existing appointments
- Delete appointments
- View appointment history
- Add appointments to Google Calendar

---

## 5. Medication Management

Users can:

- Add medication details
- Enter dosage information
- Schedule reminder times
- Update medication records
- Delete medications
- Track medication schedules

---

## 6. AI Health Summary

Users can:

- Select an appointment
- Generate an AI-powered health summary
- View patient-friendly visit summaries
- Review recommendations and follow-up guidance
- Save summaries to the healthcare record

---

## 7. SMS Reminder Service

The system automatically:

- Sends appointment reminders
- Sends medication reminders
- Tracks SMS delivery status
- Updates reminder history

---

## 8. Health Reports

Users can:

- View complete healthcare history
- Review appointments
- View medication schedules
- Read AI-generated summaries
- Print or download health reports

---

## 9. Activity History

Users can review:

- Appointment history
- Medication records
- Reminder history
- AI summaries
- Health reports
- Dashboard statistics

---

## 10. Logout

Users can securely log out of the application to end their session.

---

# Complete Application Workflow

```text
User Opens RK Health
          │
          ▼
Register / Login
          │
          ▼
Home Dashboard
          │
          ├───────────────┐
          ▼               ▼
Appointments      Medications
          │               │
          └───────┬───────┘
                  ▼
        Google Apps Script
                  │
                  ▼
         Google Sheets Database
                  │
      ┌───────────┼─────────────┐
      ▼           ▼             ▼
  Groq AI     Twilio SMS   Google Calendar
      │           │             │
      └───────────┼─────────────┘
                  ▼
        AI Summary & Reports
                  │
                  ▼
          Dashboard Updated
                  │
                  ▼
              User Logout
```

---

# Key Functionalities

- User Registration and Login
- Dashboard Overview
- Appointment Management
- Medication Management
- AI Health Summary Generation
- SMS Reminder Notifications
- Google Calendar Integration
- Health Report Generation
- Activity Tracking
- Secure Logout
