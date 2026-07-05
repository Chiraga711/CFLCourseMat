# Test: Pattern Making with Loops

*Loops in Python series · Test for Lesson 4a*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use **nested `for` loops** to build patterns. Remember: outer loop = rows, inner loop = items in the row, and a bare `print()` ends each row.
- The patterns print the `*` character, numbers, and spaces — all with ordinary `print()`.
- Read whole-number input with `int(input(...))`.
- The answer key is in a separate file: `answer-keys/answers-04a-pattern-making.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What is the **first** row of this pattern?
```python
for i in range(4, 0, -1):
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) 1 star
- B) 4 stars
- C) 3 stars
- D) An empty row

**Q2.** How many numbers are printed in total?
```python
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```
- A) 5
- B) 25
- C) 15
- D) 10

**Q3.** In this centred pattern, what is the job of the **first** inner loop?
```python
for i in range(1, n + 1):
    for s in range(n - i):
        print(" ", end=" ")
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) It prints the stars
- B) It prints the spaces that indent each row
- C) It ends the row
- D) It counts the rows

**Q4.** Which loop decides **how many items** appear in each row?
- A) The inner loop
- B) The outer loop
- C) The `print()` statement
- D) The `range` start value

**Q5.** What pattern does this make?
```python
for i in range(1, 4):
    for j in range(i):
        print(i, end=" ")
    print()
```
- A)
  ```
  1
  1 2
  1 2 3
  ```
- B) All stars
- C) `1 2 3` on one line
- D)
  ```
  1
  2 2
  3 3 3
  ```

---

## Part B — Coding Problems (5)

**P1 — Inverted Number Triangle.**
Ask the user for a number `n`, then print a number triangle that *shrinks*: the first row reads `1 2 3 ... n`, the next `1 2 3 ... (n-1)`, and so on down to a row with just `1`.

**P2 — Square of Row Numbers.**
Ask the user for a number `n`, then print an `n × n` square where every item in row `i` is the number `i`. For `n` = 4, row 1 is `1 1 1 1`, row 2 is `2 2 2 2`, and so on.

**P3 — Repeated-Number Triangle.**
Ask the user for a number `n`, then print a triangle where row `i` contains the number `i` printed `i` times (`1` / `2 2` / `3 3 3` / …).

**P4 — Inverted Star Pyramid.**
Ask the user for a number `n`, then print a centred pyramid of stars that points downward: the top row has `n` stars and each row below has one fewer, indented so the pyramid stays centred.

**P5 — Centred Number Pyramid.**
Ask the user for a number `n`, then print a centred pyramid where each row counts from 1 up to its row number, indented with spaces so the shape is centred (the bottom row reads `1 2 3 ... n`).

---

*End of test. Check your work against the separate answer key.*
