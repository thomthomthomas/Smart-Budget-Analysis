# Smart Budget Analysis

 # Budget Analysis and Reallocation Tool

## 📋 Overview
This project implements a **Budget Analysis and Reallocation Tool** using Python. The code is designed to help users track their monthly expenses, compare their spending to predefined budgets, and suggest reallocations to manage overspending effectively.

---

## 🚀 Features
1. **Expense Classification**:
   - Categorizes expenses into types: **Transport**, **Food**, **Entertainment**, **School Expenses**, and **Other**.
   - Reads expense data from a CSV file and organizes it into categories./ Access example csv file(November_Budget_Expenditure.csv) in assets folder

2. **Budget Analysis**:
   - Prompts users to input their **total budget** and individual category budgets.
   - Calculates whether each category is **over-budget** or **under-budget** based on actual spending.

3. **Daily Budget Averages**:
   - Computes the average daily spending for each category.
   - Provides insights into how well spending aligns with daily budget goals.

4. **Over-Budget and Under-Budget Detection**:
   - Identifies over-budget categories and calculates the total amount overspent.
   - Detects under-budget categories and determines the remaining budget available for reallocation.

5. **Reallocation Suggestions**:
   - Suggests reallocations from under-budget categories to cover overspending in other areas.
   - Displays reallocation recommendations or suggests reducing expenses if reallocation isn't feasible.

---

## 🛠️ How It Works
1. **Input Data**:
   - The user is prompted to input their **total monthly budget** and **individual category budgets**.
   - Expense data is loaded from a CSV file (`November_Budget_Expenditure.csv`).

2. **Data Analysis**:
   - The code filters expenses into categories based on their type.
   - Total spending for each category is compared to the user-defined budgets to classify as **Over-Budget** or **Under-Budget**.

3. **Reallocation Logic**:
   - For each date in the dataset:
     - Analyzes spending in over-budget categories.
     - Checks under-budget categories for remaining funds.
     - Suggests proportional reallocation of funds from under-budget categories to cover overspending.

4. **Output**:
   - Displays average daily budgets for all categories.
   - Provides reallocation suggestions or highlights the need to reduce spending.

---

## 📊 Example Output
- **Average Daily Budgets**:
  Transport: $5.50 Food: $4.25 Entertainment: $3.75 School Expenses: $2.90 Other: $1.80

- **Reallocation Suggestions**:
  Reallocate $3.25 from Food budget for 2023-11-12. Reallocate $2.50 from School Expenses budget for 2023-11-15.

- **Spending Reduction Alert**:
  Reduce spending by $4.00 on 2023-11-20 for over-budget categories.

## 💡 How to Use

1. Prepare a CSV file with your monthly expense data (`Spending`, `Type`, `Name`, `Date`).
2. Run the Python script in an environment with **Pandas** installed:
 ```bash
 pip install pandas

