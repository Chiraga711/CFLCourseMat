# Test: `for` Loops with `range()`

*Loops in Python series · Test for Lesson 1*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use `for` loops with `range()`. You won't need `break` or `continue` yet — those come in Lesson 3.
- Remember the golden rule: `range()` **stops before** the stop value.
- Read whole-number input with `int(input(...))`.
- The answer key is in a separate file: `answer-keys/answers-01-for-loops.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
for i in range(3, 12, 2):
    print(i, end=" ")
```
- A) `3 5 7 9`
- B) `3 5 7 9 11`
- C) `3 5 7 9 11 13`
- D) `4 6 8 10`

**Q2.** How many times does the body of this loop run?
```python
for i in range(0, 20, 4):
    print(i)
```
- A) 4
- B) 20
- C) 5
- D) 6

**Q3.** What does this print?
```python
for i in range(8, 3, -1):
    print(i, end=" ")
```
- A) `8 7 6 5 4`
- B) `8 7 6 5 4 3`
- C) `8 7 6 5`
- D) `3 4 5 6 7 8`

**Q4.** What does this print?
```python
for i in range(5, 5):
    print(i)
print("Done")
```
- A) `5` then `Done`
- B) `Done`
- C) Nothing
- D) An error

**Q5.** What does this print?
```python
total = 0
for i in range(2, 11, 2):
    total = total + i
print(total)
```
- A) `30`
- B) `20`
- C) `25`
- D) `55`

---

## Part B — Coding Problems (5)

**P1 — Multiplication Table.**
Ask the user for a whole number, then use a `for` loop to print its multiplication table from 1 to 10. Each line should look like `7 x 1 = 7`, `7 x 2 = 14`, and so on up to `7 x 10 = 70`.

**P2 — Year of Savings.**
You start with ₹1000.00 in savings and add ₹500.00 every month. Using a `for` loop over 12 months, print your balance after each month.

**P3 — Temperature Table.**
Print a conversion table from 0 °C to 100 °C in steps of 10. For each Celsius value, calculate the Fahrenheit value using `F = C × 9 / 5 + 32` and print both (for example, `20 C = 68.0 F`).

**P4 — Factorial.**
Ask the user for a whole number `n`, then use a `for` loop to calculate and print `n!` — the product `1 × 2 × 3 × ... × n`. (For example, the factorial of 5 is 120.)

**P5 — Average Score.**
Ask the user how many scores there are, then read that many scores one at a time, adding them up. After the loop, calculate and print the average (the total divided by how many scores there were).

---

*End of test. Check your work against the separate answer key.*
