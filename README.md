# Project-CLI-Expense-Tracker

A command-line expense tracker built using Python and SQLite.

## Features

- Add expenses
- View expenses
- Search expenses
- Update expenses
- Delete expenses
- Expense summary
- Category-wise spending report

## Technologies Used

- Python
- SQLite
- Tabulate

## Concepts Practiced

- CRUD Operations
- Database Integration
- SQL Queries
- Aggregation Functions
- Command Line Interface (CLI)

## How to Run

1. Install tabulate

```bash
pip install tabulate
```

2. Run

```bash
python main.py
```

## FIRST UNDERTAND THIS BEFORE GOING TO THE PROGRAM 👇👇👇:

Command Line Interface : You control a program by typing commands/instructions in a terminal instead of clicking buttons in a graphical interface.

## Workflow

### 1️⃣ Add Expense
User enters something like:
Amount: 250
Category: Food
Description: Dinner
Date: 2026-09-20
Python takes the information and stores it in SQL.

### 2️⃣ View Expenses

Display all stored expenses
- Something like:

| ID | Amount | Category  | Description | Date |
|----|---------|-----------|-------------|------------|
| 1  | 50      | Food      | Coffee      | 2026-09-18 |
| 2  | 200     | Transport | Bus         | 2026-09-19 |
| 3  | 500     | Shopping  | Shoes       | 2026-09-20 |

### 3️⃣ Search Expenses
This is where the project starts becoming more interesting.
You could search by:
- Category
- Date
- Amount
- Description
For example:
- Search by category:
- Food
- And SQL finds the matching records.

### 4️⃣ update Expense
Suppose you accidentally entered 
₹500
instead of 
₹50
You can select the expense ID and modify it.
Enter expense ID: 3
What do you want to update?
1. Amount
2. Category
3. Description
4. Date
  - Python takes the new value and SQL updates the database.


### 5️⃣ Delete Expense
- Select an expense ID:
- Enter expense ID: 3
- The record gets removed from the database.

### 6️⃣ View Summary 📊
This is where SQL becomes really useful.
Instead of simply displaying rows, your program can ask the database questions like:
- Total spent: ₹4,850
- Food:          ₹1,250
- Transport:     ₹800
- Shopping:      ₹2,000
- Entertainment: ₹800
