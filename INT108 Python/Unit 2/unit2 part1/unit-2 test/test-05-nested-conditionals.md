# Test 5: Nested Conditionals

*Conditional Statements series · Test for Lesson 5*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- This test uses **nested** conditionals — an `if`/`if-else` inside another. You may use everything you've learned (comparisons, `if`/`elif`/`else`, and `and`/`or`/`not`).
- For decimal input, use `float(input(...))`; for whole-number input, use `int(input(...))`.
- Watch your **indentation** — it decides what is inside what, and which `else` pairs with which `if`.
- The answer key is in a separate file: `answer-keys/answers-05-nested-conditionals.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
temp = 80.0
if temp > 50.0:
    if temp > 75.0:
        print("Overheating!")
    else:
        print("Warm")
else:
    print("Cool")
```
- A) `Overheating!`
- B) `Warm`
- C) `Cool`
- D) Nothing

**Q2.** What does this print?
```python
score = 60
if score >= 50:
    if score >= 80:
        print("Distinction")
    print("Pass")
else:
    print("Fail")
```
- A) `Distinction` then `Pass`
- B) `Pass`
- C) `Fail`
- D) `Distinction`

**Q3.** What is the problem with this code?
```python
if logged_in == "yes":
print("Welcome")
    if admin == "yes":
        print("Admin")
```
- A) The first `print` isn't indented under the `if`
- B) Nothing is wrong
- C) `admin` should be a number
- D) It is missing an `else`

**Q4.** In this code, what must be true to print `VIP lounge`?
```python
if has_ticket == "yes":
    if seat_class == "business":
        print("VIP lounge")
    else:
        print("Regular seating")
else:
    print("No entry")
```
- A) `has_ticket` is `"yes"` and `seat_class` is **not** `"business"`
- B) `has_ticket` is `"no"`
- C) `has_ticket` is `"yes"` **and** `seat_class` is `"business"`
- D) `seat_class` is `"business"`, no matter the ticket

**Q5.** What does this print?
```python
x = 4
if x > 10:
    y = x * 2
else:
    if x > 2:
        y = x + 100
    else:
        y = 0
print(y)
```
- A) `8`
- B) `104`
- C) `0`
- D) `4`

---

## Part B — Coding Problems (5)

**P1 — Hospital Triage.**
Ask whether a patient is an emergency case (`yes`/`no`). If they are, ask the severity (`critical`/`stable`): print `Send to ER immediately.` for critical, or `Send to urgent care.` otherwise. If it isn't an emergency, print `Join the general queue.`.

**P2 — Vending Machine.**
A snack costs ₹25.00. Ask how much money was inserted. If it is at least ₹25.00, ask whether the snack is in stock (`yes`/`no`): if it is, **calculate the change** (money inserted − 25.00) and print `Dispensing snack. Change: X`; if not, print `Out of stock - refunding your money.`. If not enough money was inserted, print `Please insert more money.`.

**P3 — University Admission.**
The entrance cutoff is 60. Ask for a student's entrance score. If it is 60 or more, check for a scholarship: print `Admitted with a scholarship!` if the score is 90 or more, otherwise `Admitted.`. If the score is below 60, print `Not qualified for admission.`.

**P4 — Phone Data Bill.**
A postpaid plan includes 50.0 GB of data, and extra data costs ₹10.00 per GB. Ask whether the customer is postpaid (`yes`/`no`). If they are, ask how much data they used (in GB): if it is more than 50.0, **calculate the extra charge** ((used − 50.0) × 10.00) and print it; otherwise print `You are within your data limit.`. If the customer isn't postpaid, print `Prepaid plan: please recharge to continue.`.

**P5 — Restaurant Reservation.**
Ask whether a table is available (`yes`/`no`). If it is, ask the party size: print `Table reserved!` if the size is 6 or fewer, otherwise `Party too large - please book the private hall.`. If no table is available, print `Sorry, you have been added to the waitlist.`.

---

*End of test. Check your work against the separate answer key.*
