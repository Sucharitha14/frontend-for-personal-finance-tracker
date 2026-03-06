# Personal Finance Tracker REST API

A backend REST API built with Flask that allows users to manage personal financial transactions securely using JWT authentication.

## Features

- User Registration
- User Login with JWT Authentication
- Protected API Routes
- Add Income / Expense Transactions
- View User Transactions
- Delete Transactions
- Financial Summary (Balance, Income, Expense)

## Tech Stack

- Python
- Flask
- Flask-JWT-Extended
- Flask-SQLAlchemy
- SQLite
- REST API

## Project Structure

finance_tracker/
│
├── app.py
├── config.py
├── extensions.py
├── models.py
├── init_db.py
│
├── routes/
│   ├── auth_routes.py
│   └── transaction_routes.py
│
├── requirements.txt
└── README.md

## API Endpoints

### Authentication

POST /api/register  
Register a new user.

POST /api/login  
Login and receive JWT token.

### Transactions

POST /api/transactions  
Add a new transaction.

GET /api/transactions  
Get all user transactions.

DELETE /api/transactions/<id>  
Delete a transaction.

### Financial Summary

GET /api/summary  
Get balance, income, and expense summary.

## Installation

Clone the repository:

git clone <repo_link>

Install dependencies:

pip install -r requirements.txt

Run the application:

python app.py

Server will start at:

http://127.0.0.1:5000