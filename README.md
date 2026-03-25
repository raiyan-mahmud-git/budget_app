# Description
This project implements a simple budget management system using Python. It allows users to track deposits, withdrawals, transfers between categories, and visualize spending through a text-based chart.

# Features
Create budget categories (e.g., Food, Clothing, Entertainment)
Deposit and withdraw money with descriptions
Transfer funds between categories
Check available balance
Generate a formatted ledger output
Display a percentage-based spending chart

# How It Works
Category Class
Each category stores transactions in a ledger.

# Methods:
deposit(amount, description="")
Adds money to the category.
withdraw(amount, description="")
Removes money if sufficient funds exist.
transfer(amount, category)
Moves money from one category to another.
get_balance()
Returns current balance.
check_funds(amount)
Verifies if enough balance is available.
__str__()
Returns a formatted string of the ledger.
create_spend_chart(categories)
Takes a list of categories
Calculates total withdrawals per category
Converts them into percentages (rounded down to nearest 10)
Displays a vertical bar chart using o markers

# Example Usage
Python
food = Category("Food")
clothing = Category("Clothing")

food.deposit(1000, "initial deposit")
food.withdraw(200, "groceries")

clothing.deposit(500, "initial deposit")
clothing.withdraw(100, "shirt")

print(create_spend_chart([food, clothing]))

# Notes
Only withdrawals (negative amounts) are used for the chart
Percentages are rounded down to the nearest 10
Output is text-based (no external libraries required)

# Project Difficulty
This is a beginner-to-intermediate level project. It focuses on:
Object-Oriented Programming (OOP)
String formatting
Basic data handling
