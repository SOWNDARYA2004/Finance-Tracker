# Personal Expense Tracker

A simple command-line-based **Personal Expense Tracker** application that allows users to record and analyze their income and expenses using a CSV file.

## Features
- Add transactions with date, amount, category (Income/Expense), and description.
- View transactions within a date range.
- Get a summary of total income, total expenses, and net savings.
- Visualize transactions using a **plot graph**.
- Stores all data in `expense_data.csv` for easy tracking.

## Installation
Ensure you have **Python 3.x** installed on your system.

1. Clone this repository:
   ```sh
   git clone https://github.com/SOWNDARYA2004/personal-expense-tracker.git
   cd personal-expense-tracker
   ```

2. Install required dependencies:
   ```sh
   pip install pandas matplotlib
   ```

## Usage
Run the main script to start tracking expenses:
```sh
python main.py
```

### Options:
1. **Add a New Transaction**
   - Enter date (`dd-mm-yyyy`) or press **Enter** for today's date.
   - Enter the amount.
   - Choose a category: **I** (Income) or **E** (Expense).
   - Provide an optional description.

2. **View Transactions and Summary**
   - Enter a **start date** and **end date**.
   - View transactions and a financial summary.
   - Optionally, generate a plot of income vs. expenses.

3. **Exit the program**

## File Structure
```
📂 expense-tracker
├── 📄 main.py            # Entry point for the application
├── 📄 data_entry.py      # Functions for user input (amount, date, category, etc.)
├── 📄 csv_handler.py     # Handles CSV operations (reading, writing transactions)
├── 📄 finance_data.csv   # Stores transaction records
└── 📄 README.md          # Documentation
```

## Example
```
1. Add a new transaction
Enter the date of the transaction (dd-mm-yyyy) or enter for today's date: 10-02-2025
Enter the amount: 500
Enter the category ('I' for Income or 'E' for Expense): E
Enter a description (optional): Grocery Shopping
Entry added successfully.

2. View transactions and summary within a date range
Enter the start date (dd-mm-yyyy): 01-02-2025
Enter the end date (dd-mm-yyyy): 10-02-2025
Transactions from 01-02-2025 to 10-02-2025:
date        amount  category  description
10-02-2025  500.00  Expense   Grocery Shopping

Summary:
Total Income: $0.00
Total Expense: $500.00
Net Savings: -$500.00
Do you want to see a plot? (y/n) : y
```
This is a line chart visualizing income and expenses over time.
<img>![Screenshot 2025-02-13 155837](https://github.com/user-attachments/assets/bf4f6e5a-5d1d-4f55-9148-7dee88d1f9a4)</img>

