
# 🐍 Beginner Python Practical Problems

This file contains **10 beginner-friendly problems** with **algorithms and Python implementations**, perfect for practice and learning basics like **arithmetic, percentage, input/output, and logic**.

---

## 1️⃣ Add Three Numbers

**Algorithm:**
1. Take three numbers as input from the user.
2. Add the three numbers.
3. Print the result.

```python
# Solution
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
sum_total = a + b + c
print("Sum of three numbers:", sum_total)
```

---

## 2️⃣ Add Two Numbers and Subtract from Third

**Algorithm:**
1. Take three numbers a, b, c.
2. Add a and b.
3. Subtract the sum from c.
4. Print the result.

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
result = c - (a + b)
print("Result:", result)
```

---

## 3️⃣ Add Two Numbers (a=10, b=20)

**Algorithm:**
1. Assign a = 10, b = 20.
2. Add a and b.
3. Print the sum.

```python
a = 10
b = 20
sum_ab = a + b
print("Sum of a and b:", sum_ab)
```

---

## 4️⃣ Evaluate Expressions

**Algorithm:**
1. Evaluate arithmetic expressions.
2. Print the results.

```python
# Expression 1
expr1 = 10 + 20 - 30 + 5
print("10 + 20 - 30 + 5 =", expr1)

# Expression 2
expr2 = 5 + 10  # Assuming $5 + 10 Rs
print("$5 + 10 Rs =", expr2)
```

---

## 5️⃣ Evaluate {a+b-10}/x

**Algorithm:**
1. Assign a = 10, x = 2.
2. Take b as input from user.
3. Evaluate (a + b - 10) / x
4. Print result.

```python
a = 10
x = 2
b = int(input("Enter value for b: "))
result = (a + b - 10) / x
print("Result of (a+b-10)/x:", result)
```

---

## 6️⃣ Salary, Savings, and Spending

**Algorithm:**
1. Take salary and savings from user.
2. Spending = 2 * savings
3. Print spending.

```python
salary = float(input("Enter salary: "))
savings = float(input("Enter savings: "))
spending = 2 * savings
print("Amount spent:", spending)
```

---

## 7️⃣ Salary Tax Calculation

**Algorithm:**
1. Take monthly salary as input.
2. Tax = 30% of salary
3. Print tax.

```python
salary = float(input("Enter salary: "))
tax = (30 / 100) * salary
print("Tax to pay:", tax)
```

---

## 8️⃣ Worker Salary from Tax

**Algorithm:**
1. Take tax from previous question.
2. Worker salary = 1/4 of tax
3. Print worker salary.

```python
tax = float(input("Enter tax amount: "))
worker_salary = tax / 4
print("Worker salary:", worker_salary)
```

---

## 9️⃣ Total Savings after Removing Worker

**Algorithm:**
1. Savings from removing worker = previous worker salary  
2. Savings from tax = half of tax  
3. Total savings = sum of above  
4. Print total savings

```python
worker_salary = float(input("Enter previous worker salary: "))
tax = float(input("Enter previous tax: "))
tax_savings = tax / 2
total_savings = worker_salary + tax_savings
print("Total savings:", total_savings)
```

---

## 🔟 Rental Charges Calculation

**Algorithm:**
1. Material is used for 4 days, not used for 3 days per week.  
2. Charge when not used = 30% of daily usage.  
3. Calculate total weekly charges.  

```python
daily_rent = float(input("Enter daily rent: "))
used_days = 4
not_used_days = 3

total_amount = (daily_rent * used_days) + (daily_rent * 0.3 * not_used_days)
print("Total amount to pay for the week:", total_amount)
```

---

### ✅ Notes for Beginners:
- Always **break problems into steps (algorithm)** before coding.  
- Use **variables clearly** for each part of calculation.  
- Test with **different inputs** to ensure correctness.  
- These problems cover **basic arithmetic, percentage, loops, and user input**, which strengthens your core Python fundamentals.

