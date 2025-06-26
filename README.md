# PaymentTracker

A RESTful Node.js and Express API for managing vendor payments. This application uses **MongoDB** to store transaction data and supports CRUD operations such as creating, updating, retrieving, and deleting vendor payments.
------
# Features
- Create an express server and with API end points based on tracking payments use case
- Retrieve data, stored in the MongoDB, through API end points
- Add data through POST end points
- Update the data through UPDATE end points
- DELETE the data through DELETE end points
----
## Tech Stack
- Node.js
- Express.js
- MongoDB with Mongoose
- Body-parser
- REST API architecture
---

# setUP & Usage
### 1. Clone the Repository

```bash
  git clone https://github.com/sushmi-krish/PaymentTracker.git
  cd PaymentTracker
```
## 2. Install Dependencies
```bash
npm install
```
### 3. Start MongoDB (local) 
 - Ensure your MongoDB service is running. If using Docker or remote MongoDB, update the connection URI in server.js.
 
# 4. Run the Server
```bash
node server.js
```
Server will start at: http://localhost:3000
-----
## File Overview
 | File                | Purpose                             |
| ------------------- | ----------------------------------- |
| `vendorPayment.js`  | Mongoose schema for payment records |
| `vendor_payment.js` | API route handlers                  |
| `server.js`         | Main Express server configuration   |
| `package.json`      | Project metadata & dependencies     |

----
# API Endpoints
| Method | Endpoint           | Description                 |
| ------ | ------------------ | --------------------------- |
| POST   | `/`                | Create a new vendor payment |
| GET    | `/`                | Get all payments            |
| GET    | `/:payment_status` | Get payments by status      |
| GET    | `/:vendor_id`      | Get payments by vendor ID   |
| PUT    | `/:transaction_id` | Update a specific payment   |
| DELETE | `/:transaction_id` | Delete a specific payment   |
----
# Summary
 - The Payment Tracker Application has been successfully tested using Postman.
- All required screenshots have been captured and are included in the repository.
