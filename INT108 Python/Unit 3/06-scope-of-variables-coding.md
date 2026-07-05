# Scope of Variables — Coding Problems (1–5)

*Unit 3 · Topic 06. Platform-judge format: exact-match output. These problems reinforce that parameters and variables created inside a function are **local**, that values come back through `return`, and that the clean way to share data is passing arguments and returning results — not relying on globals. Each names a **Required function**.*

---

## Problem 1 — Local Stays Local

**Task:** Read an integer `x`. Print the result of doubling it, and then print `x` itself — showing that doubling inside a function did **not** change the original.

**Required function:** Define `double_it(n)` that sets `n = n * 2` inside the function and **returns** `n`. In the main program read `x`, print `double_it(x)`, then print `x` on the next line. (Because `n` is local, the original `x` is unchanged.)

**Input Format:** A single integer `x` (−100000 ≤ x ≤ 100000).

**Output Format:** Two lines — the doubled value, then the original `x`.

**Sample Input:**
```
6
```
**Sample Output:**
```
12
6
```

---

## Problem 2 — Celsius to Fahrenheit

**Task:** Read a temperature in Celsius (a whole number) and print it in Fahrenheit, using `F = C × 9 ÷ 5 + 32` with integer division.

**Required function:** Define `to_fahrenheit(c)` that computes the Fahrenheit value in a **local** variable and **returns** it. Call it and print the result.

**Input Format:** A single integer `c` (−100 ≤ c ≤ 1000).

**Output Format:** A single integer — the temperature in Fahrenheit.

**Sample Input:**
```
30
```
**Sample Output:**
```
86
```

---

## Problem 3 — Running Total Without Globals

**Task:** You are given three numbers on three lines. Print their running total after adding all three — but the adding must be done by a helper function that keeps **no global state**.

**Required function:** Define `add_to(total, value)` that **returns** `total + value`. In the main program keep your own `total` variable, read three integers, and update `total = add_to(total, v)` for each. Print the final total.

**Input Format:** Three integers, each on its own line.

**Output Format:** A single integer — the sum of the three.

**Sample Input:**
```
10
20
30
```
**Sample Output:**
```
60
```

---

## Problem 4 — Count Primes (Check + Wrapper)

**Task:** Read an integer `limit` and print how many prime numbers lie in the range 2 to `limit` (inclusive).

**Required functions:** Define **two** functions. `is_prime(n)` **returns** `True`/`False` by counting divisors. `count_primes(limit)` calls `is_prime` inside its own loop and **returns** the count. Each function has its **own local** loop variable — they do not interfere. Print the result of `count_primes(limit)`.

**Input Format:** A single integer `limit` (2 ≤ limit ≤ 5000).

**Output Format:** A single integer — the number of primes from 2 to `limit`.

**Sample Input:**
```
20
```
**Sample Output:**
```
8
```

---

## Problem 5 — Swap Two Values

**Task:** Read two integers `x` and `y`, then print them in swapped order.

**Required function:** Define `swap(a, b)` that **returns the two values in reversed order** (`return b, a`). In the main program call it as `x, y = swap(x, y)` and print `x` and `y` separated by a space. (The swap works through returned values — the function's own `a` and `b` are local.)

**Input Format:** Two integers, each on its own line.

**Output Format:** The two values in swapped order, separated by a space.

**Sample Input:**
```
3
8
```
**Sample Output:**
```
8 3
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases.*
