# MongoDB Configuration

This section explains how to configure MongoDB using Mongoose for the **RK Health – Smart Patient Appointment & Medication Reminder System**.

---

## Step 1: Install Mongoose

Open the **Server** folder in Visual Studio Code and install Mongoose by running the following command:

```bash
npm install mongoose
```

This installs the Mongoose library, which provides an Object Data Modeling (ODM) layer for MongoDB.

---

## Step 2: Create Database Connection

Create a folder named **config** inside the Server directory.

```text
Server/
│
├── config/
│   └── db.js
```

The `db.js` file is responsible for:

- Connecting to the MongoDB database.
- Handling successful database connections.
- Reporting connection errors.
- Exporting the database connection.

---

## Step 3: Configure Environment Variables

Create a `.env` file in the Server folder.

Example:

```env
PORT=5000

MONGODB_URI=mongodb://localhost:27017/rk_health

JWT_SECRET=your_jwt_secret
```

For MongoDB Atlas:

```env
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/rk_health
```

---

## Step 4: Create Schemas and Models

Create a folder named **models**.

```text
Server/
│
├── models/
│   ├── userModel.js
│   ├── appointmentModel.js
│   ├── medicationModel.js
│   ├── reportModel.js
│   └── summaryModel.js
```

### User Model

Stores:

- Name
- Email
- Password
- Phone Number
- Role

---

### Appointment Model

Stores:

- Patient Name
- Doctor Name
- Appointment Date
- Appointment Time
- Visit Notes
- Status

---

### Medication Model

Stores:

- Medicine Name
- Dosage
- Reminder Time
- Phone Number
- Reminder Status

---

### Report Model

Stores:

- Patient Information
- Appointment History
- Medication Records
- AI Summary
- Report Date

---

### Summary Model

Stores:

- Appointment Details
- AI Health Summary
- Follow-up Recommendations
- Generated Timestamp

---

## Step 5: Verify the Database Connection

After starting the server, verify that:

- MongoDB connection is successful.
- Collections are created automatically.
- Schemas are registered correctly.
- Models are available throughout the application.

---

# Project Structure

```text
Server/
│
├── config/
│   └── db.js
│
├── models/
│   ├── userModel.js
│   ├── appointmentModel.js
│   ├── medicationModel.js
│   ├── reportModel.js
│   └── summaryModel.js
│
├── controllers/
├── routes/
├── middlewares/
├── index.js
├── package.json
└── .env
```

---

# Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- dotenv

---

# Expected Outcome

After completing these steps:

- Mongoose is installed successfully.
- MongoDB is connected to the application.
- Environment variables are configured securely.
- Database schemas and models are created.
- The RK Health backend is ready to store and manage healthcare data.
