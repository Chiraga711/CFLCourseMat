# Test: Nested Loops

*Loops in Python series · Test for Lesson 4*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use **nested `for` loops** with `range()`. You won't need `break` or `continue`.
- Remember: the **inner loop runs completely for every pass of the outer loop**, and `range()` stops before its stop value.
- Read whole-number input with `int(input(...))`.
- The answer key is in a separate file: `answer-keys/answers-04-nested-loops.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** How many times does the innermost line run?
```python
for i in range(4):
    for j in range(5):
        print(i + j)
```
- A) 9
- B) 20
- C) 4
- D) 25

**Q2.** What is the **last** thing this prints?
```python
for i in range(1, 4):
    for j in range(1, 4):
        print(i + j)
```
- A) `6`
- B) `9`
- C) `3`
- D) `4`

**Q3.** What does this print?
```python
for i in range(1, 4):
    for j in range(i):
        print(i, end=" ")
    print()
```
- A)
  ```
  1 1
  2 2
  3 3
  ```
- B) `1 2 3`
- C)
  ```
  1
  2 2
  3 3 3
  ```
- D) An error

**Q4.** In a nested loop, when the outer loop variable changes to its next value, the inner loop:
- A) Continues from where it left off
- B) Starts over and runs completely again
- C) Runs only once
- D) Stops

**Q5.** How many numbers does this print in total?
```python
for i in range(1, 4):
    for j in range(1, i + 1):
        print(j)
```
- A) `6`
- B) `9`
- C) `3`
- D) `4`

---

## Part B — Coding Problems (5)

**P1 — Seating Chart.**
A small theatre has 4 rows, each with 5 seats. Using nested loops, print every seat as `Row R Seat S` (so `Row 1 Seat 1`, `Row 1 Seat 2`, … up to `Row 4 Seat 5`).

**P2 — Addition Table.**
Print a 5×5 addition table: a grid where the value in each cell is `i + j` for `i` from 1 to 5 and `j` from 1 to 5. Each row should be on its own line.

**P3 — Number Square.**
Ask the user for a whole number `n`, then print an `n × n` square in which every row contains the numbers 1 to `n`. For example, if `n` is 4, each of the four rows reads `1 2 3 4`.

**P4 — Tables for a Range.**
Ask the user for a start number and an end number. Using nested loops, print the multiplication table from 1 to 10 for **every** number from start to end (each line like `3 x 1 = 3`).

**P5 — Bakery Price Grid.**
A bakery sells cakes in 3 sizes. A cake's price is its size number times ₹50.00 (size 1 is ₹50.00, size 2 is ₹100.00, size 3 is ₹150.00). For each size (1 to 3) and each quantity (1 to 4), print the total cost (price × quantity), for example `Size 2 Qty 3 = 300.0`.

---

*End of test. Check your work against the separate answer key.*
