Personal Expense Tracker API
1. Problem Statement

People often forget where their money goes. This application helps users record, manage and track their daily expenses.

2. Users

Normal users who want to track their daily spending.

3. Main Features (Must Have)
1. User registration and login.
2. Add a new expense.
3. Edit an existing expense.
4. Delete an expense.
5. View all expenses.
6. Filter expenses by date and category.
7. Calculate monthly expenses.

4. Future Features
- Export expenses to CSV.
- Display spending charts.
- Set monthly budgets and alerts.

5. Technology Stack
Technology	Purpose
Python	Programming language
FastAPI	Build backend APIs
SQLite	Store data
SQLAlchemy	Connect Python with database
Pytest	Test the application


6. Database Design

User Table
Column	Purpose
id	User ID
email	User email
password_hash	Encrypted password hash

Expense Table
Column	Purpose
id	Expense ID
user_id	Owner of expense
amount	Money spent
category	Food, travel, shopping
note	Expense description
date	Date of expense


7. API Endpoints
Method	Endpoint	Purpose
POST	/signup	Register user
POST	/login	Login user
POST	/expenses	Add expense
GET	/expenses	View expenses
PUT	/expenses/{id}	Update expense
DELETE	/expenses/{id}	Delete expense
GET	/expenses/summary	Monthly total