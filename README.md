# React Frontend Setup

This section explains how to set up the React frontend for the **RK Health – Smart Patient Appointment & Medication Reminder System** using Vite.

---

## Step 1: Open the Client Folder

Open the **Client** folder in Visual Studio Code.

Open the integrated terminal by selecting:

```text
Terminal → New Terminal
```

---

## Step 2: Create a React Project Using Vite

Run the following command inside the **Client** folder:

```bash
npm create vite@latest . -- --template react
```

---

## Step 3: Select the Framework

When prompted, select:

```text
Framework:
React
```

---

## Step 4: Select the Variant

Choose the JavaScript variant:

```text
Variant:
JavaScript
```

---

## Step 5: Install Project Dependencies

Install all required packages:

```bash
npm install
```

---

## Step 6: Start the Development Server

Run the following command:

```bash
npm run dev
```

---

## Step 7: Open the Application

After the server starts successfully, Vite will display a local development URL similar to:

```text
Local: http://localhost:5173/
```

Open the URL in your web browser to view the application.

---

# Project Structure

```text
RK-Health/
│
├── Client/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   │
│   ├── package.json
│   ├── vite.config.js
│   └── index.html
│
├── Server/
│
├── README.md
└── .gitignore
```

---

# Verify the Setup

Ensure that:

- ✅ React project is created successfully.
- ✅ All npm packages are installed.
- ✅ Vite development server starts without errors.
- ✅ The application loads in the browser.
- ✅ Hot Module Replacement (HMR) works correctly.

---

# Technologies Used

- React
- Vite
- JavaScript (ES6+)
- Node.js
- npm

---

# Expected Outcome

After completing these steps:

- A React application is created using Vite.
- All dependencies are installed.
- The development server is running successfully.
- The RK Health frontend is ready for further development.
