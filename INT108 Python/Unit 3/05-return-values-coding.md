# Return Values — Coding Problems (1–5)

*Unit 3 · Topic 05. Platform-judge format: exact-match output. These functions **return** their results with `return`; the returned value is then printed (or used) at the call site. Each names a **Required function** you must define with the exact name and parameters given.*

---

## Problem 1 — Cube

**Task:** Read an integer and print its cube.

**Required function:** Define `cube(n)` that **returns** `n × n × n` (do not print inside the function). Read the value, call `cube(n)`, and print what it returns.

**Input Format:** A single integer `n` (−100 ≤ n ≤ 100).

**Output Format:** A single integer — the cube of `n`.

**Sample Input:**
```
4
```
**Sample Output:**
```
64
```

---

## Problem 2 — Even or Odd (via a Returned Answer)

**Task:** Read an integer and print `Even` or `Odd`.

**Required function:** Define `is_even(n)` that **returns** `True` when `n` is even and `False` otherwise. In the main program, call it and use the returned value in an `if` to decide which word to print — the printing happens **outside** the function.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** Either `Even` or `Odd`.

**Sample Input:**
```
10
```
**Sample Output:**
```
Even
```

---

## Problem 3 — Smallest and Largest

**Task:** Read three integers and print the smallest and the largest, separated by a space.

**Required function:** Define `min_max(a, b, c)` that **returns two values** — the smallest and the largest of its three parameters. Unpack them in the main program (`lo, hi = min_max(...)`) and print them separated by a space.

**Input Format:** Three integers, each on its own line.

**Output Format:** Two integers separated by a space: the smallest, then the largest.

**Sample Input:**
```
7
2
9
```
**Sample Output:**
```
2 9
```

---

## Problem 4 — Grade

**Task:** Read a marks value (0–100) and print the grade letter, using these bands: 90 and above → `A`; 75–89 → `B`; 50–74 → `C`; below 50 → `F`.

**Required function:** Define `grade(marks)` that **returns** the correct letter. Write it as a series of `if` checks that each `return` immediately when matched (so the first matching band wins). Call it and print the returned letter.

**Input Format:** A single integer `marks` (0 ≤ marks ≤ 100).

**Output Format:** A single letter — `A`, `B`, `C`, or `F`.

**Sample Input:**
```
85
```
**Sample Output:**
```
B
```

---

## Problem 5 — Sum and Even-Count

**Task:** Read an integer `n` and print two values: the sum 1 + 2 + … + n, and how many numbers from 1 to `n` are even — separated by a space.

**Required function:** Define `sum_and_count(n)` that loops once from 1 to `n`, and **returns two values**: the running total and the count of even numbers. Unpack and print them, separated by a space.

**Input Format:** A single integer `n` (1 ≤ n ≤ 10000).

**Output Format:** Two integers separated by a space: the sum, then the count of even numbers.

**Sample Input:**
```
6
```
**Sample Output:**
```
21 3
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases.*
