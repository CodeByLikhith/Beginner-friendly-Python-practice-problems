# 🐍 Beginner Python Practical Problems – Set 1

This file contains **10 beginner-friendly problems** with **questions, algorithms, and Python solutions**.  
**Set 1 Questions:**

1. Write an algorithm to add three numbers.  
2. Write an algorithm to add 2 numbers and subtract from the 3rd number.  
3. Write an algorithm to add 2 numbers where a = 10 and b = 20.  
4. Write an algorithm to evaluate the following expressions:  
   - 10 + 20 - 30 + 5  
   - $5 + 10 Rs  
5. Evaluate `{a+b-10}/x` where a=10, x=2, b is given by the user.  
6. A man takes salary & saves some amount of it and spends double the savings. How much did he spend? (derive formula and implement)  
7. Harish works for 30 days & earns salary. He pays 30% as tax. How much tax does he pay?  
8. Harish has a worker; he pays 1/4 of the tax as salary. How much does he pay? (extension of previous question)  
9. Harish removes the worker and saves money previously given to worker & half of tax. What is total savings?  
10. Mythili rents a brush for 4 days and does not use it for 3 days. When not used, the website charges 30% of daily usage. Calculate total weekly charges.  

---

## 1️⃣ Add Three Numbers

**Question:** Write an algorithm to add three numbers.

**Algorithm:**  
1. Take three numbers as input from the user.  
2. Add the three numbers.  
3. Print the result.

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
sum_total = a + b + c
print("Sum of three numbers:", sum_total)
```

---

## 2️⃣ Add Two Numbers and Subtract from Third

**Question:** Write an algorithm to add 2 numbers and subtract from the 3rd number.

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
c = int(input("Enter third number: "))
result = c - (a + b)
print("Result:", result)
```

---

## 3️⃣ Add Two Numbers (a=10, b=20)

**Question:** Write an algorithm to add 2 numbers where a = 10 and b = 20.

```python
a = 10
b = 20
sum_ab = a + b
print("Sum of a and b:", sum_ab)
```

---

## 4️⃣ Evaluate Expressions

**Question:** Write an algorithm to evaluate:  
- 10 + 20 - 30 + 5  
- $5 + 10 Rs

```python
# Expression 1
expr1 = 10 + 20 - 30 + 5
print("10 + 20 - 30 + 5 =", expr1)

# Expression 2: $5 + 10 Rs (convert USD to INR first)
usd_to_inr = 82
amount_usd = 5
amount_rs = 10

amount_usd_in_rs = amount_usd * usd_to_inr
total_amount = amount_usd_in_rs + amount_rs
print("5 USD + 10 Rs =", total_amount, "Rs")
```

---

## 5️⃣ Evaluate {a+b-10}/x

**Question:** {a+b-10}/x where a=10, x=2, b is given by user

```python
a = 10
x = 2
b = int(input("Enter value for b: "))
result = (a + b - 10) / x
print("Result of (a+b-10)/x:", result)
```

---

## 6️⃣ Salary, Savings, and Spending

**Question:** A man takes salary & saves some amount. Spending = 2 × savings. Find spending.

```python
salary = float(input("Enter salary: "))
savings = float(input("Enter savings: "))
spending = 2 * savings
print("Amount spent:", spending)
```

---

## 7️⃣ Salary Tax Calculation

**Question:** Harish pays 30% tax on salary.

```python
salary = float(input("Enter salary: "))
tax = (30 / 100) * salary
print("Tax to pay:", tax)
```

---

## 8️⃣ Worker Salary from Tax

**Question:** Worker salary = 1/4 of tax.

```python
tax = float(input("Enter tax amount: "))
worker_salary = tax / 4
print("Worker salary:", worker_salary)
```

---

## 9️⃣ Total Savings after Removing Worker

**Question:** Savings = previous worker salary + half of tax.

```python
worker_salary = float(input("Enter previous worker salary: "))
tax = float(input("Enter previous tax: "))
tax_savings = tax / 2
total_savings = worker_salary + tax_savings
print("Total savings:", total_savings)
```

---

## 🔟 Rental Charges Calculation

**Question:** Mythili rents a brush 4 days, not used 3 days. Not-used charge = 30% of daily usage.

```python
daily_rent = float(input("Enter daily rent: "))
used_days = 4
not_used_days = 3

total_amount = (daily_rent * used_days) + (daily_rent * 0.3 * not_used_days)
print("Total amount to pay for the week:", total_amount)
```

---

# 🐍 Beginner Python Practical Problems – Set 2

This file contains **9 practical problems** with **questions, algorithms, formulas, and Python implementations**, focusing on real-life applications and beginner-friendly logic.

**Set 2 Questions:**

1. Nikhil, a movie fan, contributes to a rating system where votes are counted in multiples of 1,000. Represent votes as '1K', '1.5K', etc.  
2. Preeti buys oil from Russia at $50/10 liters. Calculate cost in INR. Part B: Russia gives $2 discount/10 liters. Calculate discount for 1 barrel (158.987 liters).  
3. Neha wants to play 170 minutes. Display in `xh : ym` format.  
4. Manya fills first name, last name, age, percentage. Display first name, last name, full name.  
5. Take salary as input. If >50,000 → "middle class", else "lower middle class".  
6. Take salary as input. If >50,000 → "upper middle class", else add 7% increment.  
7. Input character 'm' for male, 'f' for female (case-insensitive).  
8. Menu-driven addition: choice = 1 → add two numbers, else wrong choice.  
9. Salary >50,000 → Deduct 10% tax. If remaining salary >50,000 → Deduct 2% more.

---

## 1️⃣ Display Votes in 'K' Format

**Question:**  
Nikhil, a movie fan, contributes to a rating system where votes are counted in multiples of 1,000. To make displayed ratings easier, represent every 1,000 votes as '1K'. For example, 1,500 votes → '1.5K'.

**Algorithm:**
1. Take the number of votes as input.  
2. Check if votes > 0.  
3. Divide votes by 1000 → `votes_in_k`.  
4. Display as formatted string with `K`.

```python
votes = int(input("Enter number of votes: "))
if votes > 0:
    votes_in_k = votes / 1000
    print(f"Votes Display: {votes_in_k}K")
else:
    print("No votes yet")
```

**Example Output:**
```
Enter number of votes: 1500
Votes Display: 1.5K
```

---

## 2️⃣ Oil Purchase from Russia

**Question Part A:**  
Preeti buys oil from Russia at $50 for 10 liters. How much does she pay in INR?  

**Question Part B:**  
Russia gives $2 discount per 10 liters. How much discount for 1 barrel (1 barrel = 158.987 liters)?

**Algorithm Part A:**  
1. Take liters needed.  
2. Calculate cost in USD: `(liters / 10) * 50`.  
3. Convert USD to INR: `USD * 82`.  
4. Print total amount.

```python
# Part A
liters_needed = float(input("Enter liters to buy: "))
price_per_10_liters_usd = 50
usd_to_inr = 82
total_usd = (liters_needed / 10) * price_per_10_liters_usd
total_inr = total_usd * usd_to_inr
print("Total price to pay (INR):", total_inr)
```

**Algorithm Part B:**  
1. Barrel liters = 158.987  
2. Discount per 10 liters = $2  
3. Units = barrel_liters / 10  
4. Total discount = units * 2 USD → convert to INR

```python
barrel_liters = 158.987
discount_per_10_liters_usd = 2
usd_to_inr = 82
units = barrel_liters / 10
total_discount_usd = units * discount_per_10_liters_usd
total_discount_inr = total_discount_usd * usd_to_inr
print("Discount for 1 barrel (INR):", total_discount_inr)
```

---

## 3️⃣ Convert Minutes to Hours and Minutes

**Question:**  
Neha has 170 minutes to play. Show it in `xh : ym` format.

**Algorithm:**  
1. Hours = minutes // 60  
2. Remaining minutes = minutes % 60  
3. Print formatted string

```python
total_minutes = int(input("Enter total minutes: "))
hours = total_minutes // 60
minutes = total_minutes % 60
print(f"{hours}h : {minutes}m")
```

**Example Output:**  
```
Enter total minutes: 170
2h : 50m
```

---

## 4️⃣ Display Full Name

**Question:**  
Manya fills first name, last name, age, percentage. Display first name, last name, and full name.

**Algorithm:**  
1. Take first name, last name, age, percentage  
2. Concatenate first and last name → full name  
3. Print all

```python
first_name = input("Enter first name: ")
last_name = input("Enter last name: ")
age = int(input("Enter age: "))
percentage = float(input("Enter percentage: "))
full_name = first_name + " " + last_name
print("First Name:", first_name)
print("Last Name:", last_name)
print("Full Name:", full_name)
```

---

## 5️⃣ Salary Classification – Middle Class

**Question:**  
If salary > 50,000 → "middle class", else "lower middle class".

```python
salary = float(input("Enter salary: "))
if salary > 50000:
    print("Middle class")
else:
    print("Lower middle class")
```

---

## 6️⃣ Salary Increment if Below 50,000

**Question:**  
If salary > 50,000 → upper middle class. Else, add 7% and show new salary.

```python
salary = float(input("Enter salary: "))
if salary > 50000:
    print("Upper middle class")
else:
    salary = salary + (salary * 0.07)
    print("Updated Salary with 7% increment:", salary)
```

---

## 7️⃣ Character Input – Male or Female

**Question:**  
Input 'm' for male, 'f' for female, case-insensitive.

```python
gender = input("Enter gender (m/f): ")
if gender.lower() == 'm':
    print("Male")
elif gender.lower() == 'f':
    print("Female")
else:
    print("Invalid input")
```

---

## 8️⃣ Menu Driven – Add Two Numbers

**Question:**  
Choice = 1 → add two numbers, else wrong choice.

```python
choice = int(input("Enter your choice (1 to add): "))
if choice == 1:
    num1 = int(input("Enter first number: "))
    num2 = int(input("Enter second number: "))
    print("Sum =", num1 + num2)
else:
    print("Wrong choice")
```

---

## 9️⃣ Nested If – Salary Tax Deduction

**Question:**  
If salary > 50,000 → Deduct 10% tax. If remaining salary > 50,000 → Deduct 2% more.

```python
salary = float(input("Enter salary: "))

if salary > 50000:
    salary -= salary * 0.10  # Deduct 10%
    if salary > 50000:
        salary -= salary * 0.02  # Deduct 2% more
print("Final Salary after tax:", salary)
```

---

---

### ✅ Notes for Beginners:
- Always **break problems into steps (algorithm)** before coding.  
- Use **variables clearly** for each part of calculation.  
- Test with **different inputs** to ensure correctness.  
- These problems cover **basic arithmetic, percentage, loops, and user input**, which strengthens your core Python fundamentals.

