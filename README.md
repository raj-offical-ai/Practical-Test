# SMART EXPENSE TRACKER

## Project Overview

**Smart Expense Tracker** is a Python-based personal finance analysis project. It allows users to add, view, filter, analyze, and visualize their daily expenses.

The project is designed as a **Jupyter Notebook / Google Colab compatible** program and uses Python, NumPy, Pandas, Matplotlib, Seaborn, CSV file handling, Object-Oriented Programming, and Data Validation.

---

## Technologies Used

1. Python
2. NumPy
3. Pandas
4. Matplotlib
5. Seaborn
6. CSV File Handling
7. Object-Oriented Programming (OOP)
8. Data Validation
9. Control Structures
10. Lists / Arrays

---

## Main Features

### 1. Add Expense

Users can enter:

* Date
* Amount
* Category
* Description

The program validates all entered information before saving it.

### 2. View All Expenses

Displays all saved expenses in a tabular format and shows total spending.

### 3. Generate Summary Report

The report displays:

* Number of expenses
* Total spending
* Average expense
* Highest expense
* Lowest expense
* Category-wise spending
* Monthly spending
* Spending percentage by category

### 4. Filter Expenses

Expenses can be filtered using:

* Category
* Start date
* End date
* Minimum amount
* Maximum amount

### 5. Data Visualization

The project generates a dashboard containing:

* Category-wise spending bar chart
* Daily spending trend
* Spending distribution pie chart
* Expense amount frequency histogram

### 6. CSV File Handling

All expense records are stored in:

`expenses.csv`

The CSV file is automatically created if it does not exist.

---

## Expense Categories

The program supports the following categories:

* Food
* Transport
* Utilities
* Entertainment
* Shopping
* Healthcare
* Education
* Other

---

## Data Validation

The program checks:

* Date must follow `YYYY-MM-DD`
* Amount must be numeric
* Amount must be greater than zero
* Category must be one of the valid categories
* Description cannot be empty
* Invalid CSV data is removed during loading
* CSV columns must match the required format

---

## CSV File Format

The `expenses.csv` file contains four columns:

```text
Date,Amount,Category,Description
```

Example:

```text
2026-09-10,250,Food,Lunch
2026-09-11,100,Transport,Bus
2026-09-12,500,Shopping,Clothes
```

---

## Project Structure

```text
Smart Expense Tracker/
│
├── Smart_Expense_Tracker.ipynb
├── expenses.csv
└── README.md
```

In Google Colab or Jupyter Notebook, the CSV file is created automatically when the program starts.

---

## How to Run the Project

### Step 1: Open Jupyter Notebook or Google Colab

Create a new Python notebook.

### Step 2: Install Required Libraries

Usually NumPy, Pandas, Matplotlib and Seaborn are already available.

If required, run:

```python
!pip install numpy pandas matplotlib seaborn
```

### Step 3: Paste the Program

Paste the complete Smart Expense Tracker program into a notebook cell.

### Step 4: Run the Cell

Execute the cell.

The program starts with:

```text
Smart Expense Tracker started successfully!
```

### Step 5: Select a Menu Option

The main menu contains:

```text
1. Add Expense
2. View All Expenses
3. Generate Summary Report
4. Filter Expenses
5. Show Visualizations
6. Exit
```

Enter the required option number.

---

## Example: Adding an Expense

Example input:

```text
Date (YYYY-MM-DD): 2026-09-10
Amount: 250
Category: Food
Description: Lunch
```

Output:

```text
Expense added successfully!
```

---

## Example Summary Report

After adding expenses, selecting option `3` generates a report similar to:

```text
=================================================================
          SMART EXPENSE TRACKER REPORT
=================================================================
Number of expenses : 3
Total spending     : ₹850.00
Average expense    : ₹283.33
Highest expense    : ₹500.00
Lowest expense     : ₹100.00

Category-wise Spending:
----------------------------------------
Shopping            ₹500.00
Food                ₹250.00
Transport           ₹100.00

Monthly Spending:
   Month    Total    Average
2026-09    ₹850.00   ₹283.33
=================================================================
```

The exact values depend on the expenses entered by the user.

---

## Visualization Dashboard

Selecting option `5` displays a four-chart dashboard:

### 1. Category-wise Spending

A bar chart compares spending between different categories.

### 2. Daily Spending Trend

A line chart shows spending over different dates.

### 3. Spending Distribution by Category

A pie chart displays the percentage of total spending for each category.

### 4. Expense Amount Frequency

A histogram shows the frequency distribution of expense amounts.

---

## Important Note

The current `main()` function calls:

```python
create_fresh_csv()
```

at the beginning of every program run.

This means the existing `expenses.csv` is intentionally replaced with a new empty CSV whenever the program starts.

**Therefore, if you want previous expenses to remain available between program runs, remove or comment out this line:**

```python
create_fresh_csv()
```

After doing that, the `ExpenseTracker` class will load the existing `expenses.csv` file.

---

## Project Objective

The objective of this project is to demonstrate practical use of Python programming concepts for personal expense management and data analysis.

The project combines:

* Programming fundamentals
* Functions
* Classes and Objects
* Lists
* NumPy calculations
* Pandas data processing
* CSV file handling
* Data validation
* Data filtering
* Statistical summaries
* Data visualization

---

## Learning Outcomes

After completing this project, the following concepts are demonstrated:

* Working with CSV files
* Creating and using Python classes
* Performing data validation
* Processing data using Pandas
* Performing numerical calculations using NumPy
* Creating charts using Matplotlib and Seaborn
* Applying conditional statements and loops
* Building a menu-driven Python application
* Analyzing personal expense data
* Presenting analytical results visually

---

## Conclusion

The **Smart Expense Tracker** is a beginner-friendly Python data analysis project for managing and analyzing personal expenses.

It provides a menu-driven interface, validates user input, stores data in CSV format, calculates useful financial statistics, supports filtering, and creates a visual analytics dashboard.

This project is suitable for a **Python / Data Analysis academic submission** and can be extended in the future with features such as:

* Monthly budgets
* Expense editing
* Expense deletion
* Automatic spending insights
* Login functionality
* Database storage

---

## Author
Raj Dabhade

