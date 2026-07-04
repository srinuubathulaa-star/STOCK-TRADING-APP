# Backend Setup

This section explains how to initialize the backend for the **RK Health – Smart Patient Appointment & Medication Reminder System** using Node.js.

---

## Step 1: Open the Server Folder

Open the **Server** folder in Visual Studio Code.

Open the integrated terminal by selecting:

```text
Terminal → New Terminal
```

---

## Step 2: Initialize the Node.js Project

Run the following command to create a `package.json` file:

```bash
npm init -y
```

This command initializes the backend project with default settings.

---

## Step 3: Create the Main Server File

Create a file named:

```text
server.js
```

This file serves as the entry point for the backend application.

---

## Step 4: Create Project Folders

Create the following folders inside the **Server** directory:

```text
models
controllers
routes
```

### Folder Purpose

**models/**

Contains database models and schema definitions.

**controllers/**

Contains business logic and request handling functions.

**routes/**

Contains API route definitions and endpoint mappings.

---

## Step 5: Backend Project Structure

Your backend directory should look like:

```text
Server/
│
├── controllers/
│
├── models/
│
├── routes/
│
├── server.js
│
├── package.json
│
└── package-lock.json
```

---

## Step 6: Verify the Setup

Ensure that:

- ✅ `package.json` is created successfully.
- ✅ `server.js` exists.
- ✅ `models` folder is created.
- ✅ `controllers` folder is created.
- ✅ `routes` folder is created.
- ✅ Backend project structure is organized correctly.

---

## Technologies Used

- Node.js
- npm
- JavaScript (ES6)

---

## Expected Outcome

After completing these steps:

- The backend project is initialized.
- `package.json` is created.
- The main server entry file (`server.js`) is ready.
- Project folders are organized for scalable backend development.
- The RK Health backend is prepared for implementing APIs and business logic.
