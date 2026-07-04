## System Architecture

### Description

In this architecture diagram:

### Frontend

The **Frontend** section represents the user interface developed using **HTML, CSS, and JavaScript**. It provides an interactive dashboard where users can manage healthcare information.

Frontend components include:

- Login Page
- Home Dashboard
- Add Patient Entry
- Appointment Management
- Medication Management
- AI Health Summary Viewer
- Health Report Dashboard
- Reminder History
- Notification System

---

### Backend

The **Backend** section is implemented using **Google Apps Script**, which processes all application requests and communicates with external services.

Backend functions include:

- `doGet(e)` – Loads the application.
- `addLog()` – Stores patient appointments and medication records.
- `getLogs()` – Retrieves healthcare records.
- `updateLog()` – Updates patient information.
- `deleteLog()` – Deletes healthcare records.
- `getStats()` – Calculates dashboard statistics.
- `generateSummary()` – Generates AI-powered healthcare summaries using the Groq API.
- `sendSMS()` – Sends medication and appointment reminders through Twilio.
- `runOnce()` – Performs scheduled backend operations and initialization.

The backend also integrates with:

- Google Sheets
- Groq AI API
- Twilio SMS API
- Google Calendar API

---

### Database

The **Database** section is implemented using **Google Sheets**, which acts as the cloud database for the application.

It stores:

- Patient Records
- Appointment Details
- Medication Schedules
- Reminder Status
- AI Health Summaries
- Health Reports
- Activity Logs
- Timestamps

---

### External Services

The application integrates with several cloud services:

- **Groq API** – Generates AI-powered patient-friendly health summaries.
- **Twilio SMS API** – Sends medication and appointment reminder notifications.
- **Google Calendar** – Creates appointment events and reminder links.
- **Google Sheets** – Stores all healthcare records securely.

---

### Application Workflow

```text
User
   │
   ▼
Frontend Dashboard
(HTML • CSS • JavaScript)
   │
   ▼
Google Apps Script Backend
   │
   ├── Patient Management
   ├── Appointment Management
   ├── Medication Management
   ├── AI Summary Generation
   ├── Report Generation
   └── SMS Reminder Service
   │
   ▼
Google Sheets Database
   │
   ├───────────────┬─────────────────┐
   ▼               ▼                 ▼
Groq AI      Twilio SMS      Google Calendar
   │               │                 │
   └───────────────┴─────────────────┘
                   │
                   ▼
          RK Health Dashboard
```
