# Recursion — Coding Problems (1–5)

*Unit 3 · Topic 08. Platform-judge format: exact-match output. Every solution must be **recursive** — the function calls itself, with a **base condition** that stops it. **No loops are allowed** (a `for` or `while` solution will not be accepted even if its output is correct — this is checked when your code is reviewed). Each names a **Required function** you must define with the exact name and parameters given.*

---

## Problem 1 — Factorial (Recursive)

**Task:** Read an integer `n` and print `n!` — computed recursively.

**Required function:** Define `factorial(n)` that **returns** 1 when `n` is 0 (the base case), and otherwise **returns** `n * factorial(n - 1)`. Call it and print the result. No loop.

**Input Format:** A single integer `n` (0 ≤ n ≤ 12).

**Output Format:** A single integer — the factorial of `n`.

**Sample Input:**
```
5
```
**Sample Output:**
```
120
```

---

## Problem 2 — Sum to N (Recursive)

**Task:** Read an integer `n` and print the sum 1 + 2 + … + n — computed recursively.

**Required function:** Define `sum_to(n)` that **returns** 0 when `n` is 0 (base case), and otherwise **returns** `n + sum_to(n - 1)`. Call it and print the result. No loop.

**Input Format:** A single integer `n` (0 ≤ n ≤ 10000).

**Output Format:** A single integer — the sum from 1 to `n`.

**Sample Input:**
```
10
```
**Sample Output:**
```
55
```

---

## Problem 3 — Nth Fibonacci (Recursive)

**Task:** Read an integer `n` and print the `n`-th Fibonacci number, where `fib(0) = 0`, `fib(1) = 1`, and each later value is the sum of the two before it.

**Required function:** Define `fib(n)` that **returns** `n` when `n < 2` (base cases), and otherwise **returns** `fib(n - 1) + fib(n - 2)`. Call it and print the result.

**Input Format:** A single integer `n` (0 ≤ n ≤ 30).

**Output Format:** A single integer — the `n`-th Fibonacci number.

**Sample Input:**
```
7
```
**Sample Output:**
```
13
```

---

## Problem 4 — Power (Recursive)

**Task:** Read a base and an exponent and print `base` raised to `exp` — computed recursively, without `**` or `math.pow`.

**Required function:** Define `power(base, exp)` that **returns** 1 when `exp` is 0 (base case), and otherwise **returns** `base * power(base, exp - 1)`. Call it and print the result.

**Input Format:** Two integers, each on its own line — `base` then `exp` (1 ≤ base ≤ 100, 0 ≤ exp ≤ 15).

**Output Format:** A single integer — `base` raised to the power `exp`.

**Sample Input:**
```
2
10
```
**Sample Output:**
```
1024
```

---

## Problem 5 — Digit Sum (Recursive)

**Task:** Read an integer `n` and print the sum of its digits — computed recursively.

**Required function:** Define `digit_sum(n)` that **returns** 0 when `n` is 0 (base case), and otherwise **returns** `n % 10 + digit_sum(n // 10)` (the last digit plus the digit sum of the rest). Call it and print the result.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the sum of the digits of `n`.

**Sample Input:**
```
472
```
**Sample Output:**
```
13
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases (including base-case inputs like 0 and 1).*
