# Test: Controlling Loops — `break`, `continue`, `pass`, loop `else`

*Loops in Python series · Test for Lesson 3*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use `break`, `continue`, `pass`, and the loop `else` clause, in both `for` and `while` loops.
- Remember: `break` stops the loop, `continue` skips one pass, and a loop `else` runs only if **no** `break` happened.
- Read whole-number input with `int(input(...))`.
- The answer key is in a separate file: `answer-keys/answers-03-controlling-loops.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
n = 1
while n <= 10:
    if n == 4:
        break
    print(n)
    n = n + 1
```
- A) `1 2 3 4`
- B) `1 2 3`
- C) `1` through `10`
- D) `4 5 6`

**Q2.** What happens when this runs?
```python
n = 0
while n < 5:
    if n == 2:
        continue
    print(n)
    n = n + 1
```
- A) It prints `0` and `1`, then loops forever
- B) It prints `0 1 2 3 4`
- C) It prints `0 1 3 4`
- D) It causes an error

**Q3.** What does this print?
```python
n = 1
while n <= 3:
    print(n)
    n = n + 1
else:
    print("Loop done")
```
- A) `1 2 3`
- B) `Loop done`
- C) `1 2 3` then `Loop done`
- D) `1 2 3`, with no `Loop done`

**Q4.** Which statement does **nothing** and lets the rest of the loop body run normally?
- A) `break`
- B) `continue`
- C) `else`
- D) `pass`

**Q5.** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 4):
        if j == 2:
            break
        print(i, j)
```
- A) `1 1` only
- B) `1 1`, `2 1`, `3 1`
- C) `1 1`, `1 2`, `1 3`, `2 1`, …
- D) Nothing

---

## Part B — Coding Problems (5)

**P1 — ATM Withdrawals.**
An account starts with ₹2000.00, and each withdrawal takes out ₹500.00. Using a `while True` loop, withdraw ₹500.00 at a time and print the balance after each withdrawal, using `break` to stop once the balance reaches 0.

**P2 — Skipping a Floor.**
A building's lift visits floors 1 to 10, but this building has no 4th floor. Using a `for` loop with `continue`, print every floor from 1 to 10 except floor 4.

**P3 — Ticket Lookup.**
A cinema has ticket numbers 1 to 50. Ask the customer for a ticket number, then search 1 to 50: if the number is found, print `Ticket N is available` and `break`; if the loop finishes without finding it, use the loop `else` to print `Ticket not available`.

**P4 — Shopping on a Budget.**
You have a budget of ₹100.00, and each item costs ₹15.00. Using a `while True` loop, keep buying items (adding ₹15.00 to the amount spent) and printing the running total, but use `break` to stop *before* the total would go over the budget. At the end, print how many items you bought.

**P5 — Game Rounds.**
A game has rounds 1 to 20. Round 10 is a rest round that should be skipped (`continue`), and the game ends if you reach round 15 (`break`). Using a `for` loop, print the number of every round you actually play.

---

*End of test. Check your work against the separate answer key.*
