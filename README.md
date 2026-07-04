# Running the Application

Follow the steps below to run the **SB Stocks** application locally.

---

# Step 1: Set Up the Frontend (React Application)

## Open the Client Folder

Open a terminal and navigate to the client directory.

```bash
cd client
```

---

## Install Dependencies

Install all required packages.

```bash
npm install
```

---

## Start the React Development Server

Run the following command:

```bash
npm run dev
```

The frontend application will be available at:

```text
http://localhost:5173
```

---

# Step 2: Set Up the Backend (Express Server)

Open a new terminal window or split the existing terminal.

Navigate to the server directory.

```bash
cd ../server
```

---

## Install Backend Dependencies

```bash
npm install
```

---

# Step 3: Configure Environment Variables

Inside the **server** folder, create a file named:

```text
.env
```

Add the required environment variables.

Example:

```env
PORT=8000

MONGO_URI=mongodb://localhost:27017/sbstocks

JWT_SECRET=your_jwt_secret

API_KEY=your_api_key
```

If you are using MongoDB Atlas:

```env
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/sbstocks
```

---

# Step 4: Start the Backend Server

Run the backend using Nodemon:

```bash
nodemon index.js
```

or

```bash
npm run dev
```

The backend server will start at:

```text
http://localhost:8000
```

---

# Project Startup Workflow

```text
Open Terminal
      │
      ▼
cd client
      │
      ▼
npm install
      │
      ▼
npm run dev
      │
      ▼
Frontend Running
      │
      ▼
Open New Terminal
      │
      ▼
cd server
      │
      ▼
npm install
      │
      ▼
Configure .env
      │
      ▼
nodemon index.js
      │
      ▼
Backend Running
      │
      ▼
Connect MongoDB
      │
      ▼
Application Ready
```

---

# Verify the Setup

Ensure that:

- ✅ React application loads successfully.
- ✅ Express server starts without errors.
- ✅ MongoDB connection is established.
- ✅ Environment variables are loaded correctly.
- ✅ API endpoints are accessible.
- ✅ Frontend communicates with the backend.

---

# Technologies Used

- React
- Vite
- Node.js
- Express.js
- MongoDB
- Mongoose
- Nodemon

---

# Expected Outcome

After completing these steps:

- The frontend runs on **http://localhost:5173**.
- The backend runs on **http://localhost:8000**.
- MongoDB is connected successfully.
- The SB Stocks application is ready for development and testing.
