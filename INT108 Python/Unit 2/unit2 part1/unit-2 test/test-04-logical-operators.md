# Test 4: Logical Operators (`and`, `or`, `not`)

*Conditional Statements series · Test for Lesson 4*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- This test combines conditions with `and`, `or`, and `not` (used inside `if` / `if-else`). No nested `if`s yet.
- For decimal input, use `float(input(...))`; for whole-number input, use `int(input(...))`.
- Remember the order of precedence: **`not` first, then `and`, then `or`** — and use parentheses when mixing `and` with `or`.
- The answer key is in a separate file: `answer-keys/answers-04-logical-operators.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
age = 25
income = 18000
if age > 18 and income > 20000:
    print("Approved")
else:
    print("Rejected")
```
- A) `Approved`
- B) `Both`
- C) `Rejected`
- D) An error

**Q2.** What does this print?
```python
temp = -5.0
if temp < 0.0 or temp > 40.0:
    print("Extreme")
else:
    print("Normal")
```
- A) `Extreme`
- B) `Normal`
- C) `Both`
- D) An error

**Q3.** What does this print?
```python
print(not True and False)
```
- A) `True`
- B) `False`
- C) An error
- D) `None`

**Q4.** Which condition is true exactly when a number `n` is **outside** the range 1 to 10?
- A) `n < 1 and n > 10`
- B) `n < 1 or n > 10`
- C) `n > 1 or n < 10`
- D) `n >= 1 and n <= 10`

**Q5.** What does this print?
```python
raining = True
have_umbrella = True
if not raining or have_umbrella:
    print("Go outside")
else:
    print("Stay in")
```
- A) `Stay in`
- B) `Go outside`
- C) An error
- D) Both

---

## Part B — Coding Problems (5)

**P1 — Blood Donation Eligibility.**
A person can donate blood only if their age is between 18 and 65 (inclusive) **and** they weigh at least 50.0 kg. Ask for the person's age and weight, then print whether they are eligible (`You are eligible to donate blood.`) or not (`Sorry, you are not eligible.`).

**P2 — Loan Approval.**
A bank approves a loan if the applicant is at least 21 **and** earns a monthly salary of at least ₹25000.00. For approved applicants, the maximum loan is **20 times the salary**. Ask for the applicant's age and salary; if they qualify, calculate and print the maximum loan, otherwise print `Not eligible for a loan.`.

**P3 — Fire Alarm.**
A fire alarm should sound if smoke is detected **or** the room temperature is above 60.0 °C. Ask whether smoke is detected (`yes`/`no`) and the room temperature. Print `FIRE ALARM! Evacuate now.` if either condition is met, otherwise `All clear.`.

**P4 — Gym Equipment.**
A treadmill is free to use as long as it is **not** occupied. Ask whether the treadmill is occupied (`yes`/`no`). Using `not`, print `Go ahead, it is free!` when it isn't occupied, and `It is occupied - please wait.` when it is.

**P5 — Airport Boarding (capstone).**
A passenger may board only if they have a ticket **and** (a passport **or** a national ID) **and** are **not** on the no-fly list. Ask four `yes`/`no` questions — ticket, passport, national ID, and no-fly list — then print `Boarding approved. Have a nice flight!` or `Boarding denied.`. (Use parentheses to group the `or` correctly.)

---

*End of test. Check your work against the separate answer key.*
