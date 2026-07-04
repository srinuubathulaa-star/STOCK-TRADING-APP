## Architecture Description

In this architecture diagram:

The **Frontend** is represented by the **Frontend** section, which includes user interface components such as the Landing Page, Patient Dashboard, Appointment Management, Medication Reminder Management, Health Log Tracking, AI Summary Viewer, and Health Report Dashboard. These components provide an intuitive and responsive interface for users to manage their healthcare activities.

The **Backend** is represented by the **Google Apps Script Backend** section, which processes client requests, manages business logic, performs CRUD operations for appointments, medications, and health records, generates AI-powered visit summaries, sends SMS reminders through Twilio, and communicates with Google Calendar for appointment scheduling.

The **Database** section represents **Google Sheets**, which acts as the cloud database for storing patient information, appointment records, medication schedules, health logs, reminder history, and generated health reports.

The **External Services** section includes **Twilio SMS API** for sending medication and appointment reminders, **Google Calendar API** for scheduling and managing appointments, and the **Groq AI API** for generating intelligent healthcare visit summaries and insights.

The architecture enables secure communication between the frontend, backend, cloud database, and external services, providing a centralized, automated, and user-friendly healthcare management platform.
