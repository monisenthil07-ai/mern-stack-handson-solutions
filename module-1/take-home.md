# Take-Home Assignment
Personal Expense Calculator Students develop a simple program that: ● Accepts income and expense details ● Calculates savings ● Categorizes expenses ● Displays a summary report AI-Assisted Activity ● Use AI to generate pseudocode and flowcharts from problem statements. ● Compare human vs AI-generated solutions.

Expected Outcome Students demonstrate understanding of variables, loops, conditions, and functions.
## Personal Expense Calculator – Solution

### 1. Aim

To develop a simple Personal Expense Calculator that accepts income and expense details, calculates savings, categorizes expenses, and displays a summary report.

### 2. Algorithm

1. Start the program.
2. Get the user's monthly income.
3. Ask the user to enter the number of expenses.
4. Accept each expense amount and its category.
5. Calculate the total expenses.
6. Categorize expenses such as Food, Travel, Education, and Shopping.
7. Calculate savings using the formula:

   **Savings = Total Income − Total Expenses**
8. Display the total income, total expenses, category-wise expenses, and savings.
9. Stop the program.

### 3. Python Program

```python
# Personal Expense Calculator

def expense_calculator():
    income = float(input("Enter your monthly income: ₹"))

    expenses = {}
    total_expenses = 0

    n = int(input("Enter the number of expenses: "))

    for i in range(n):
        category = input(f"Enter expense category {i + 1}: ")
        amount = float(input("Enter expense amount: ₹"))

        expenses[category] = expenses.get(category, 0) + amount
        total_expenses += amount

    savings = income - total_expenses

    print("\n===== MONTHLY EXPENSE REPORT =====")
    print(f"Total Income: ₹{income:.2f}")
    print(f"Total Expenses: ₹{total_expenses:.2f}")

    print("\nCategory-wise Expenses:")
    for category, amount in expenses.items():
        print(f"{category}: ₹{amount:.2f}")

    print(f"\nRemaining Savings: ₹{savings:.2f}")

    if savings > 0:
        print("Status: You have savings.")
    elif savings == 0:
        print("Status: Your income is fully spent.")
    else:
        print("Status: Your expenses exceed your income.")

expense_calculator()
```

### 4. Sample Output

```text
Enter your monthly income: ₹20000
Enter the number of expenses: 4

Enter expense category 1: Food
Enter expense amount: ₹3000

Enter expense category 2: Travel
Enter expense amount: ₹2000

Enter expense category 3: Education
Enter expense amount: ₹4000

Enter expense category 4: Shopping
Enter expense amount: ₹1000

===== MONTHLY EXPENSE REPORT =====
Total Income: ₹20000.00
Total Expenses: ₹10000.00

Category-wise Expenses:
Food: ₹3000.00
Travel: ₹2000.00
Education: ₹4000.00
Shopping: ₹1000.00

Remaining Savings: ₹10000.00
Status: You have savings.
```

### 5. Pseudocode

```text
START

INPUT income
INPUT number_of_expenses

SET total_expenses = 0

FOR each expense:
    INPUT category
    INPUT amount
    ADD amount to category total
    ADD amount to total_expenses
END FOR

savings = income - total_expenses

DISPLAY income
DISPLAY total_expenses
DISPLAY category-wise expenses
DISPLAY savings

IF savings > 0:
    DISPLAY "You have savings"
ELSE IF savings == 0:
    DISPLAY "Income fully spent"
ELSE:
    DISPLAY "Expenses exceed income"
END IF

STOP
```

### 6. Flowchart

```text
       ┌─────────────┐
       │    START    │
       └──────┬──────┘
              │
              ▼
       ┌─────────────┐
       │ Input Income│
       └──────┬──────┘
              │
              ▼
       ┌─────────────────┐
       │ Input Expenses  │
       │ and Categories  │
       └────────┬────────┘
                │
                ▼
       ┌─────────────────┐
       │ Calculate Total │
       │    Expenses     │
       └────────┬────────┘
                │
                ▼
       ┌─────────────────┐
       │ Calculate       │
       │ Savings         │
       └────────┬────────┘
                │
                ▼
       ┌─────────────────┐
       │ Display Summary │
       │     Report      │
       └────────┬────────┘
                │
                ▼
       ┌─────────────┐
       │     STOP    │
       └─────────────┘
```

### 7. AI-Assisted Activity

**Objective:** Use AI to generate pseudocode and flowcharts and compare the AI-generated solution with a human-designed solution.

| Human-Generated Solution                          | AI-Generated Solution                              |
| ------------------------------------------------- | -------------------------------------------------- |
| Created manually using logical thinking.          | Generated using an AI tool.                        |
| May take more time to develop.                    | Can be generated quickly.                          |
| Helps improve independent problem-solving skills. | Helps understand alternative approaches.           |
| May contain logical errors.                       | May also contain logical errors and needs testing. |

**Conclusion:** Both human reasoning and AI assistance can help develop a Personal Expense Calculator. AI can speed up development, while human verification ensures the program works correctly.

### 8. Expected Outcome

Students will learn to:

* Use variables to store income and expenses.
* Use loops to accept multiple expenses.
* Use conditional statements to check savings.
* Use functions to organize the program.
* Use dictionaries to categorize expenses.
* Generate pseudocode and flowcharts with AI assistance.
* Compare human-generated and AI-generated solutions.

