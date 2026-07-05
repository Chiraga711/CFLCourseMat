# Test: `while` Loops

*Loops in Python series · Test for Lesson 2*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use `while` loops controlled by a condition. You won't need `break` or `continue` yet — those come in Lesson 3.
- For decimal input, use `float(input(...))`; for whole-number input, use `int(input(...))`.
- Make sure every loop **updates** the variable in its condition so it eventually stops.
- The answer key is in a separate file: `answer-keys/answers-02-while-loops.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
balance = 50.0
while balance < 200.0:
    balance = balance + 50.0
print(balance)
```
- A) Forever
- B) `150.0`
- C) `200.0`
- D) `250.0`

**Q2.** How many times does the loop body run?
```python
i = 0
while i < 10:
    i = i + 2
```
- A) 4
- B) 5
- C) 10
- D) Forever

**Q3.** What does this code do?
```python
n = 5
while n > 0:
    print(n)
    n = n + 1
```
- A) It is an infinite loop, because `n` grows instead of shrinking
- B) It counts down from 5 to 1
- C) It prints nothing
- D) It causes an error

**Q4.** If the user enters `5`, then `3`, then `0`, what does this print?
```python
total = 0
n = int(input())
while n != 0:
    total = total + n
    n = int(input())
print(total)
```
- A) `5`
- B) `8`
- C) `0`
- D) An error

**Q5.** Which loop is the better choice when you **don't know in advance** how many times you need to repeat?
- A) A `while` loop
- B) A `for` loop
- C) They are identical
- D) Neither can do it

---

## Part B — Coding Problems (5)

**P1 — Savings Goal.**
You start with ₹500.00 in savings and add ₹250.00 every month. Using a `while` loop, keep adding until your savings reach at least ₹2000.00, printing the balance after each month.

**P2 — Seating the Audience.**
A theatre seats 20 people per show. Using a `while` loop, work out how many shows are needed to seat 150 people, and print that number of shows.

**P3 — Counting Scores.**
A teacher enters students' scores one at a time and types `-1` when finished. Using a `while` loop, count how many scores were entered (not counting the `-1`) and print the count.

**P4 — Loan Payoff.**
A loan of ₹1000.00 is paid off ₹200.00 every week. Using a `while` loop, print the remaining balance after each week, until the balance reaches 0.

**P5 — Bouncing Ball.**
A ball is dropped from a height of 100.0 metres, and each bounce reaches half the previous height. Using a `while` loop, print the height of each bounce until the height drops below 1.0 metre.

---

*End of test. Check your work against the separate answer key.*
