# Connect MongoDB Before Backend Operations

Before performing any backend operations such as creating appointments, managing medications, generating reports, or handling user authentication, ensure that the application is successfully connected to the MongoDB database.

---

## Step 1: Create the Database Connection

Create a file named **db.js** inside the **config** folder.

Project structure:

```text
Server/
│
├── config/
│   └── db.js
│
├── controllers/
├── models/
├── routes/
├── index.js
└── package.json
```

---

## Step 2: Configure the Database Connection

Example connection code:

```javascript
const mongoose = require("mongoose");

const connectDB = async () => {
    try {
        await mongoose.connect(process.env.MONGODB_URI);

        console.log("MongoDB Connected Successfully");
    } catch (error) {
        console.error("Database Connection Failed:", error.message);
        process.exit(1);
    }
};

module.exports = connectDB;
```

---

## Step 3: Connect the Database in index.js

Import the database connection before defining routes or starting the server.

Example:

```javascript
const express = require("express");
const dotenv = require("dotenv");
const connectDB = require("./config/db");

dotenv.config();

connectDB();

const app = express();

app.use(express.json());

// Register Routes Here

const PORT = process.env.PORT || 5000;

app.listen(PORT, () => {
    console.log(`Server running on port ${PORT}`);
});
```

---

## Step 4: Configure Environment Variables

Create a `.env` file inside the **Server** folder.

Example:

```env
PORT=5000

MONGODB_URI=mongodb://localhost:27017/rk_health
```

For MongoDB Atlas:

```env
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/rk_health
```

---

## Backend Startup Flow

```text
Start Server
      │
      ▼
Load Environment Variables
      │
      ▼
Connect MongoDB
      │
      ▼
Connection Successful
      │
      ▼
Initialize Express Server
      │
      ▼
Register Middleware
      │
      ▼
Register Routes
      │
      ▼
Server Ready
```

---

## Why Connect First?

Connecting to MongoDB before handling requests ensures that:

- Database operations execute successfully.
- Data is stored and retrieved reliably.
- Backend routes have access to the database.
- Errors are detected early during server startup.
- The application remains stable and consistent.

---

## Verification Checklist

- Mongoose installed successfully.
- `.env` file configured.
- MongoDB connection established.
- Server starts without errors.
- Database models are accessible.
- Backend APIs are ready for CRUD operations.

---

## Expected Outcome

After completing these steps:

- MongoDB is connected before the server starts.
- Backend APIs can safely perform database operations.
- RK Health is ready to manage patient records, appointments, medications, AI summaries, and health reports.
