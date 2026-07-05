# Lesson 4a: Pattern Making with Loops

*Part of the **Loops in Python** series · companion to Lesson 4*

> **Before you start:** This lesson puts **Lesson 4 (nested loops)** to work, so make sure you're comfortable with a loop inside a loop first. Type every example and run it — patterns are best understood by watching them appear.
>
> **A note on printing characters:** the patterns below print the `*` character and spaces. That's just `print("*")` — printing text in quotes, exactly like your very first program. No new string skills are needed.

---

## What You'll Learn

- The mental model behind every pattern: **outer loop = rows, inner loop = what's in each row**
- How to print squares, triangles, and pyramids made of `*`
- How to print **number patterns** like number triangles and Floyd's triangle
- How to **indent** rows with spaces to make a centred pyramid
- The one line that beginners always forget: the row-ending `print()`

---

## 1. The Big Idea: Rows and Columns

Every pattern is a grid of rows. To build one, you use two loops:

- The **outer loop** runs once per **row**.
- The **inner loop** prints the **items in that row** (stars, numbers, or spaces).
- A bare **`print()`** after the inner loop ends the row and drops to the next line.

That's the whole recipe. What changes from pattern to pattern is **how many items each row has** and **what those items are**. Master that, and every pattern becomes a small variation on the same idea.

---

## 2. A Solid Square

The simplest pattern: every row has the same number of stars.

```python
n = 4
for i in range(n):          # 4 rows
    for j in range(n):      # 4 stars per row
        print("*", end=" ")
    print()                 # end the row
```

**Output:**
```
* * * * 
* * * * 
* * * * 
* * * * 
```

`end=" "` keeps the stars on the same line with a space between them; the bare `print()` starts the next row.

---

## 3. A Right-Angled Triangle (Growing)

Now make each row a little longer than the last. The trick is that the inner loop's length **depends on the row number `i`**.

```python
n = 4
for i in range(1, n + 1):   # i = 1, 2, 3, 4
    for j in range(i):      # row i has i stars
        print("*", end=" ")
    print()
```

**Output:**
```
* 
* * 
* * * 
* * * * 
```

Row 1 prints one star, row 2 prints two, and so on. This dependency between the loops is the heart of triangle patterns.

---

## 4. An Upside-Down Triangle (Shrinking)

To shrink the rows instead, count the outer loop **downwards** with a negative step:

```python
n = 4
for i in range(n, 0, -1):   # i = 4, 3, 2, 1
    for j in range(i):
        print("*", end=" ")
    print()
```

**Output:**
```
* * * * 
* * * 
* * 
* 
```

Same inner loop as before — only the outer loop changed direction.

---

## 5. A Number Triangle

Patterns don't have to be stars. Print the loop variable instead of `*` and you get a number triangle:

```python
n = 4
for i in range(1, n + 1):
    for j in range(1, i + 1):   # numbers 1 up to i
        print(j, end=" ")
    print()
```

**Output:**
```
1 
1 2 
1 2 3 
1 2 3 4 
```

Each row counts from 1 up to its row number.

---

## 6. Floyd's Triangle (a Running Counter)

What if the numbers should keep climbing across the whole shape? Keep a **counter** that lives *outside* both loops and increases every time you print:

```python
n = 4
count = 1
for i in range(1, n + 1):
    for j in range(i):
        print(count, end=" ")
        count = count + 1      # increase after each number
    print()
```

**Output:**
```
1 
2 3 
4 5 6 
7 8 9 10 
```

Because `count` is never reset, the numbers flow continuously from one row to the next. This is the classic **Floyd's triangle**.

---

## 7. A Centred Pyramid (Two Inner Loops)

To centre a triangle into a pyramid, each row needs some **spaces** before the stars. That means **two inner loops** per row: one for the spaces, then one for the stars.

```python
n = 4
for i in range(1, n + 1):
    for s in range(n - i):      # spaces: more at the top, fewer lower down
        print(" ", end=" ")
    for j in range(i):          # then the stars
        print("*", end=" ")
    print()
```

**Output:**
```
      * 
    * * 
  * * * 
* * * * 
```

The top row gets the most spaces (`n - i` is largest when `i` is small), so the stars are pushed toward the centre. Stacking two inner loops like this is how most "fancy" patterns are built.

---

## 8. Common Mistakes to Avoid

### Mistake 1: Forgetting the row-ending `print()`

```python
# WRONG - no print() to end the row, so everything lands on one line
for i in range(1, 4):
    for j in range(i):
        print("*", end=" ")

# CORRECT - print() after the inner loop, lined up with it
for i in range(1, 4):
    for j in range(i):
        print("*", end=" ")
    print()
```

### Mistake 2: Putting `print()` at the wrong indentation

If the `print()` is indented under the **inner** loop, it runs after every star and you get one star per line. It must line up with the **inner loop**, so it runs once per row.

### Mistake 3: Wrong inner range for triangles

For a growing triangle, the inner loop must depend on `i` (`range(i)` or `range(1, i + 1)`). Using a fixed range like `range(n)` gives a square instead.

---

## 9. Quick Reference

```python
# Solid square (n x n)
for i in range(n):
    for j in range(n):
        print("*", end=" ")
    print()

# Growing right triangle
for i in range(1, n + 1):
    for j in range(i):
        print("*", end=" ")
    print()

# Shrinking right triangle
for i in range(n, 0, -1):
    for j in range(i):
        print("*", end=" ")
    print()

# Centred pyramid (spaces, then stars)
for i in range(1, n + 1):
    for s in range(n - i):
        print(" ", end=" ")
    for j in range(i):
        print("*", end=" ")
    print()
```

---

## 10. Check Your Understanding (5 MCQs)

**Q1.** What shape does this make?
```python
for i in range(1, 4):
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) A square
- B) A shrinking triangle
- C) A growing right triangle (1, then 2, then 3 stars)
- D) A single row of stars

**Q2.** How many stars are printed in total?
```python
for i in range(1, 5):
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) 4
- B) 10
- C) 16
- D) 8

**Q3.** In a pattern, which loop controls the number of **rows**?
- A) The outer loop
- B) The inner loop
- C) Neither
- D) Both equally

**Q4.** What does the bare `print()` after the inner loop do?
- A) Prints a star
- B) Ends the current row and starts a new line
- C) Skips a row
- D) Does nothing

**Q5.** What is the **last** row of this pattern?
```python
for i in range(4, 0, -1):
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) 4 stars
- B) 3 stars
- C) 2 stars
- D) 1 star

<details>
<summary><strong>Answer Key (tap to reveal)</strong></summary>

**Q1 — C.** The inner range is `range(i)`, so row 1 has 1 star, row 2 has 2, row 3 has 3 — a growing right triangle.

**Q2 — B (10).** The rows have 1 + 2 + 3 + 4 = 10 stars in total.

**Q3 — A.** The outer loop runs once per row, so it controls how many rows there are.

**Q4 — B.** It ends the current row and moves to the next line, so the next row starts fresh.

**Q5 — D (1 star).** The outer loop counts down 4, 3, 2, 1, so the final row has just 1 star.

</details>

---

## 11. Coding Challenges (5 Problems)

Write and **run** each one. Solutions follow — try first!

**Problem 1 — Star Square.**
Print a solid 5×5 square of stars (five rows, five stars each).

**Problem 2 — Growing Triangle.**
Ask the user for a number `n`, then print a right-angled triangle of stars where row 1 has 1 star, up to row `n` having `n` stars.

**Problem 3 — Shrinking Triangle.**
Ask the user for a number `n`, then print an upside-down triangle of stars: the first row has `n` stars and each row below has one fewer.

**Problem 4 — Number Triangle.**
Ask the user for a number `n`, then print a number triangle where each row counts from 1 up to its row number (row 3 reads `1 2 3`).

**Problem 5 — Floyd's Triangle.**
Ask the user for a number `n`, then print Floyd's triangle for `n` rows — the numbers count up continuously across the whole shape (`1` / `2 3` / `4 5 6` / …).

<details>
<summary><strong>Solutions (tap to reveal)</strong></summary>

**Solution 1**
```python
for i in range(5):
    for j in range(5):
        print("*", end=" ")
    print()
```

**Solution 2**
```python
n = int(input("Enter a number: "))
for i in range(1, n + 1):
    for j in range(i):
        print("*", end=" ")
    print()
```

**Solution 3**
```python
n = int(input("Enter a number: "))
for i in range(n, 0, -1):
    for j in range(i):
        print("*", end=" ")
    print()
```

**Solution 4**
```python
n = int(input("Enter a number: "))
for i in range(1, n + 1):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
```

**Solution 5**
```python
n = int(input("Enter a number: "))
count = 1
for i in range(1, n + 1):
    for j in range(i):
        print(count, end=" ")
        count = count + 1
    print()
```

</details>

---

## Summary

- Every pattern follows one recipe: **outer loop = rows, inner loop = items in the row**, and a bare **`print()`** ends each row.
- Make the inner loop **depend on the row number** to grow or shrink a triangle.
- Print the loop variable (or a running **counter**) instead of `*` to make **number patterns**.
- Counting the outer loop **downwards** flips a triangle upside down.
- Add a **second inner loop for spaces** to indent rows into a centred pyramid.

Next up — **Lesson 5: Common Loop Patterns** (the programming kind: accumulator, counting, finding the largest or smallest, and the flag pattern).
