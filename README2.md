# Personal Finance Tracker REST API

A backend REST API built using Flask that allows users to manage their personal finances by tracking income and expenses securely using JWT authentication.

## Features

User Authentication
- Register new users
- Login with JWT token authentication
- Secure protected routes

Transaction Management
- Add income or expense transactions
- View all user-specific transactions
- Delete transactions

Financial Summary
- Calculate total income
- Calculate total expenses
- Show current balance

## Technologies Used

- Python
- Flask
- Flask-JWT-Extended
- Flask-SQLAlchemy
- SQLite
- REST API
- Git & GitHub

## Project Structure

finance_tracker
│
├── app.py
├── config.py
├── extensions.py
├── models.py
├── init_db.py
│
├── routes
│   ├── auth_routes.py
│   └── transaction_routes.py
│
└── instance
    └── finance.db

## API Endpoints

Authentication
- POST /api/register
- POST /api/login

Transactions
- POST /api/transactions
- GET /api/transactions
- DELETE /api/transactions/<id>

Summary
- GET /api/summary

## How to Run the Project

1. Clone the repository

git clone https://github.com/Sucharitha14/personal-finance-tracker-api.git

2. Navigate into the project

cd personal-finance-tracker-api

3. Create virtual environment

python -m venv venv

4. Activate environment

Windows:
venv\Scripts\activate

5. Install dependencies

pip install -r requirements.txt

6. Run the application

python app.py

Server will start at:
http://127.0.0.1:5000
