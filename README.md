# Backend Project Structure

The backend is organized into multiple folders to separate configuration, business logic, database models, middleware, and API routes, making the application modular and easy to maintain.

---

## Config

### db.js

Handles the database connection and configuration.

**Responsibilities**

- Connect to MongoDB database
- Handle database connection errors
- Export database connection

---

## Controllers

### appointmentController.js

Handles appointment-related operations.

**Responsibilities**

- Create appointments
- Update appointments
- Delete appointments
- Retrieve appointment records

---

### medicationController.js

Handles medication management.

**Responsibilities**

- Add medications
- Update medication schedules
- Delete medication records
- Retrieve medication information

---

### reportController.js

Handles health report generation.

**Responsibilities**

- Generate patient reports
- Retrieve report history
- Export reports

---

### summaryController.js

Handles AI summary generation.

**Responsibilities**

- Prepare appointment notes
- Send requests to the Groq API
- Store AI-generated summaries

---

### userController.js

Handles user management.

**Responsibilities**

- User registration
- User login
- User profile management
- Password validation

---

## Middlewares

### authMiddleware.js

Provides authentication and authorization.

**Responsibilities**

- Verify user authentication
- Protect private routes
- Validate access tokens

---

## Models

### appointmentModel.js

Defines the Appointment schema.

Stores:

- Patient Name
- Doctor Name
- Appointment Date
- Appointment Time
- Visit Notes
- Status

---

### medicationModel.js

Defines the Medication schema.

Stores:

- Medicine Name
- Dosage
- Reminder Time
- Phone Number
- Status

---

### reportModel.js

Defines the Health Report schema.

Stores:

- Patient Details
- Appointment History
- Medication Records
- AI Summary
- Report Date

---

### userModel.js

Defines the User schema.

Stores:

- Name
- Email
- Password
- Phone Number
- Role

---

## Routes

### appointmentRoute.js

API endpoints for appointment management.

---

### medicationRoute.js

API endpoints for medication management.

---

### reportRoute.js

API endpoints for health report generation.

---

### summaryRoute.js

API endpoints for AI health summary generation.

---

### userRoute.js

API endpoints for user authentication and profile management.

---

## Root Files

### index.js

Main server entry point.

Responsibilities:

- Initialize Express
- Configure middleware
- Connect database
- Register API routes
- Start server

---

### package.json

Contains:

- Project information
- Dependencies
- Scripts
- Version information

---

### package-lock.json

Automatically generated file that locks dependency versions for consistent installations.

---

### schemas.js

Exports all application schema definitions from a single location for easier imports and maintenance.

---

# Backend Folder Structure

```text
Server/
│
├── config/
│   └── db.js
│
├── controllers/
│   ├── appointmentController.js
│   ├── medicationController.js
│   ├── reportController.js
│   ├── summaryController.js
│   └── userController.js
│
├── middlewares/
│   └── authMiddleware.js
│
├── models/
│   ├── appointmentModel.js
│   ├── medicationModel.js
│   ├── reportModel.js
│   └── userModel.js
│
├── routes/
│   ├── appointmentRoute.js
│   ├── medicationRoute.js
│   ├── reportRoute.js
│   ├── summaryRoute.js
│   └── userRoute.js
│
├── index.js
├── schemas.js
├── package.json
└── package-lock.json
```

---

# Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- Groq API
- Twilio API

---

# Benefits

- Modular architecture
- Easy maintenance
- Scalable backend
- Secure authentication
- Organized API structure
- Clear separation of concerns
- Cloud-ready deployment
