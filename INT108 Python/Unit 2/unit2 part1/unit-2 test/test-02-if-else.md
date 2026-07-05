# Test 2: The `if-else` Statement

*Conditional Statements series · Test for Lesson 2*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- Use the `if-else` statement for this test (a two-way choice) — but no `elif`, `and`/`or`/`not`, or nested `if`s yet.
- For decimal input, use `float(input(...))`; for whole-number input, use `int(input(...))`.
- Currency is shown as ₹, but you only need to print the numbers.
- The answer key is in a separate file: `answer-keys/answers-02-if-else.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
price = 250.0
if price > 200.0:
    price = price - 50.0
else:
    price = price + 50.0
print(price)
```
- A) `250.0`
- B) `200.0`
- C) `300.0`
- D) `50.0`

**Q2.** What does this print?
```python
temp = 36.5
if temp > 36.5:
    print("Fever")
else:
    print("Normal")
```
- A) `Fever`
- B) `Both`
- C) `Normal`
- D) An error

**Q3.** What is wrong with this code?
```python
if age >= 18:
    print("Adult")
print("Hello")
else:
    print("Minor")
```
- A) The statement between the `if` block and `else` isn't allowed
- B) `else` needs a condition
- C) It is missing a colon
- D) Nothing is wrong

**Q4.** What does this print if the user enters `100`?
```python
amount = int(input())
if amount >= 100:
    final = amount - amount / 10
    print(final)
else:
    print(amount)
```
- A) `100`
- B) `90`
- C) `110`
- D) `90.0`

**Q5.** What does this print?
```python
balance = 0.0
if balance != 0.0:
    print("You have money")
else:
    print("Account is empty")
```
- A) `You have money`
- B) `Account is empty`
- C) Both run
- D) An error

---

## Part B — Coding Problems (5)

**P1 — Exam Result.**
The pass mark is 40.0. Ask for a student's marks. If the marks are 40.0 or more, print `Pass`. Otherwise, calculate **how many marks short** of passing they were and print `Fail. You were short by X marks.` (where X is the difference).

**P2 — Personalised Greeting.**
Ask for a person's gender (`male` or `female`). If it is `male`, print `Hello, Mr. Smith!`. Otherwise, print `Hello, Ms. Smith!`.

**P3 — Recharge Bonus.**
A mobile recharge of ₹200.00 or more earns a 10% bonus added to it. Ask for the recharge amount. If it qualifies, calculate the **total balance** (recharge plus the 10% bonus) and print it. Otherwise, print the recharge amount as the balance (no bonus).

**P4 — Library Borrowing Limit.**
A member may hold up to 5 books at a time. Ask how many books the member currently has. If they have fewer than 5, calculate **how many more** they may borrow and print it. Otherwise, print `You've reached your borrowing limit.`.

**P5 — Toll by Vehicle.**
A toll plaza charges ₹75.50 for a car and ₹30.00 for a bike, and a ₹5.00 service charge is added to every toll. Ask for the vehicle type (`car` or `bike`), calculate the **total toll** (base fee + service charge), and print it.

---

*End of test. Check your work against the separate answer key.*
