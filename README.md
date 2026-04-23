# Personal Expense Tracker

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Handling-green)
![CSV](https://img.shields.io/badge/Data%20Storage-CSV-lightgrey)
![Status](https://img.shields.io/badge/Status-Portfolio%20Project-brightgreen)

## Overview

The **Personal Expense Tracker** is a Python-based budgeting application built in Jupyter Notebook. It allows users to record expenses, view spending history, set a monthly budget, track spending progress, and save/load expense data using CSV files.

This project demonstrates foundational Python programming, structured application logic, data handling with Pandas, user input processing, and basic file persistence.

## Project Objectives

- Build a simple menu-driven personal finance tracker.
- Capture expense details including date, category, amount, and description.
- Display expenses in a clean tabular format.
- Allow users to set and monitor a monthly budget.
- Save and load expense data using CSV files.
- Practice organizing Python code with reusable functions.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | DataFrame creation and expense display |
| CSV Module | Save and load expense records |
| Jupyter Notebook | Development and testing environment |
| GitHub | Version control and portfolio presentation |

## Lab Environment

| Component | Details |
|---|---|
| Language | Python 3.x |
| Interface | Jupyter Notebook |
| Data Storage | CSV file |
| Main File | `personal_expense_tracker.ipynb` |
| Output File | `expenses.csv` |

## Application Workflow

```text
User Opens Program
        |
        v
Previous Expenses Load from CSV
        |
        v
Main Menu Displays Options
        |
        v
User Adds, Views, Budgets, Tracks, or Saves Expenses
        |
        v
Expense Data Saves Back to CSV
```

## Features

- Add new expense records.
- View all recorded expenses.
- Set a monthly budget.
- Track total spending against the budget.
- Save expenses to a CSV file.
- Load saved expenses when the program starts.
- Basic error handling for missing CSV files.

## Example Program Run

```text
Menu:
1. Add Expense
2. View Expenses
3. Set Budget
4. Track Budget
5. Save Expenses
6. Exit

Choose an option from the menu: 1
Enter the date (YYYY-MM-DD): 2026-04-23
Enter the category (e.g., Food, Travel): Food
Enter the amount spent: 18.75
Enter a brief description: Lunch

Expense added successfully!

Menu:
1. Add Expense
2. View Expenses
3. Set Budget
4. Track Budget
5. Save Expenses
6. Exit

Choose an option from the menu: 2

Current Expenses:
      date category  amount description
2026-04-23     Food   18.75       Lunch

Choose an option from the menu: 3
Enter your monthly budget: 500
Monthly budget set to $500.00

Choose an option from the menu: 4
Total spent so far: $18.75
You have $481.25 left for the month.

```

## Step-by-Step Walkthrough

### 1. Project Files

The repository contains the main Jupyter Notebook, README documentation, and local screenshot assets.

![Project Files](images/01-project-files.png)

### 2. Imports and Data Setup

The project imports `csv` and `pandas`, initializes an empty expense structure, converts the date field into a datetime format, and prepares the expense list for use in the program.

![Imports and Data Setup](images/02-imports-and-data-setup.png)

### 3. Add and View Expenses

The `add_expense()` function collects user input for date, category, amount, and description. The `view_expenses()` function converts the expense list into a Pandas DataFrame for cleaner table-style output.

![Add and View Expenses Functions](images/03-add-and-view-expenses-functions.png)

### 4. Budget Tracking

The `set_budget()` function stores the monthly budget, while `track_budget()` calculates total spending and compares it against the user-defined budget.

![Budget Tracking Functions](images/04-budget-tracking-functions.png)

### 5. Save and Load Expense Data

The project uses CSV file handling to save expense records and reload them later, giving the application basic data persistence.

![Save and Load Expenses CSV](images/05-save-and-load-expenses-csv.png)

### 6. Main Menu Program Flow

The `main_menu()` function ties the application together by providing a simple menu-driven interface for adding, viewing, budgeting, saving, and exiting the program.

![Main Menu Program Flow](images/06-main-menu-program-flow.png)

## Results

This project successfully demonstrates:

- A functional Python expense tracking application.
- Organized code using reusable functions.
- Basic data persistence using CSV files.
- Structured display of expense data with Pandas.
- Budget comparison logic using conditional statements.
- Clear documentation and screenshot-based project presentation.

## What Employers Should Notice

This project highlights several entry-level technical skills that are valuable in software, data, automation, and cybersecurity-adjacent roles:

- Ability to build a working Python application from scratch.
- Understanding of functions, lists, dictionaries, loops, and conditionals.
- Experience handling structured data with Pandas.
- Ability to save and reload application data using files.
- Clear project organization and GitHub documentation.
- Practical mindset: solving a real-world problem with code.

## Lessons Learned

- How to organize a Python program into reusable functions.
- How to collect and process user input.
- How to structure records using dictionaries and lists.
- How to use Pandas to present data clearly.
- How to save and reload records using CSV files.
- How to document a project for a professional portfolio.

## Future Improvements

- Add stronger input validation for dates, amounts, and categories.
- Add category-based spending summaries.
- Add monthly spending reports.
- Add charts for visual expense analysis.
- Convert the notebook into a standalone Python script.
- Build a simple GUI or web dashboard.
- Add unit tests for the core functions.
- Add support for recurring expenses.

## Disclaimer

This project is for educational and portfolio purposes only. It is not intended to replace professional financial software or financial advice.
