# MongoDB Schemas

This section defines the MongoDB schemas used in the **SB Stocks** application. The schemas are designed based on the Entity Relationship (ER) Diagram and provide a structured way to store and manage application data.

---

# User Schema

The **User Schema** stores user account information and authentication details.

### Fields

- Username
- Email
- Password
- Contact Number
- Balance
- Role
- Created At
- Updated At

### Purpose

- Register new users
- Authenticate users
- Store account balance
- Manage user profiles

---

# Transactions Schema

The **Transactions Schema** stores all buy and sell transactions performed by users.

### Fields

- User ID
- Stock ID
- Transaction Type (Buy/Sell)
- Quantity
- Stock Price
- Total Amount
- Transaction Time
- Status

### Purpose

- Record every stock transaction
- Maintain transaction history
- Track trading activity
- Generate reports

---

# Stocks Schema

The **Stocks Schema** stores stock market information.

### Fields

- Stock Symbol
- Company Name
- Stock Exchange
- Current Price
- Market Sector
- Market Capitalization
- Daily Change
- Historical Prices
- Last Updated

### Purpose

- Store stock details
- Display market information
- Provide real-time stock prices
- Support historical trend analysis

---

# Orders Schema

The **Orders Schema** stores user stock orders.

### Fields

- User ID
- Stock ID
- Order Type (Buy/Sell)
- Quantity
- Price
- Total Amount
- Order Status
- Created Time

### Purpose

- Manage stock orders
- Process buy and sell requests
- Track order status
- Link orders with transactions

---

# Database Relationships

```text
User
 │
 ├──────────────┐
 ▼              ▼
Transactions   Orders
 │              │
 └──────┬───────┘
        ▼
      Stocks
```

---

# Database Collections

The MongoDB database contains the following collections:

- Users
- Transactions
- Stocks
- Orders

---

# Benefits

- Organized data storage
- Easy querying
- Efficient relationship management
- Scalable database design
- Secure user information
- Fast transaction processing

---

# Technologies Used

- MongoDB
- Mongoose
- Node.js
- Express.js

---

# Expected Outcome

After implementing these schemas:

- User information is stored securely.
- Stock data is organized efficiently.
- Transactions are recorded accurately.
- Orders are managed effectively.
- The database supports real-time stock trading operations.
