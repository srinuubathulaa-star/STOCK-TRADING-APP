# System Roles

## 1. User (Patient)

The Patient is the primary user of the RK Health application.

### Responsibilities

- Register and securely log in to the application.
- Manage personal healthcare information.
- Schedule doctor appointments.
- Add and manage medication schedules.
- View appointment history and medication records.
- Receive SMS reminders for appointments and medications.
- Generate AI-powered health summaries.
- View and download health reports.
- Add appointments to Google Calendar.
- Monitor healthcare activities through the dashboard.

---

## 2. System (RK Health Platform)

The RK Health platform manages healthcare operations and integrates cloud services.

### Responsibilities

- Process user requests through Google Apps Script.
- Store healthcare records in Google Sheets.
- Generate AI-powered health summaries using the Groq API.
- Send appointment and medication reminders through Twilio SMS.
- Generate Google Calendar event links.
- Maintain dashboard statistics and healthcare reports.
- Validate user input before processing.
- Ensure secure and reliable cloud communication.
- Provide a responsive and user-friendly interface.

---

## 3. Administrator

The Administrator manages the overall application and ensures smooth operation.

### Responsibilities

- Monitor application performance.
- Maintain backend services.
- Manage Google Sheets database.
- Configure Google Apps Script deployment.
- Manage Groq API and Twilio integration.
- Monitor system logs and application errors.
- Ensure data accuracy and consistency.
- Perform system maintenance and updates.
- Manage application security and access permissions.
- Resolve technical issues and monitor cloud services.

---

# Role Interaction

```text
Patient
    │
    ▼
RK Health Dashboard
    │
    ▼
Google Apps Script Backend
    │
    ├── Google Sheets
    ├── Groq AI
    ├── Twilio SMS
    └── Google Calendar
    │
    ▼
Administrator Monitoring
```
