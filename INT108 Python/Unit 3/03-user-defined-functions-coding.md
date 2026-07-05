# User-Defined Functions — Coding Problems (1–5)

*Unit 3 · Topic 03. Platform-judge format: exact-match output. The natural solution to each defines a function and calls it, using only `def`, calling, loops, conditionals, and `input()` — no `return` yet (that comes in Topic 05). Values are passed into the function through its parentheses; results are printed inside the body.*

---

## Problem 1 — Repeat a Banner

Define a function that prints a three-line banner, then call it once for each repeat requested.

**Task:** Print the banner below `n` times, one immediately after another.
```
=====
MENU
=====
```

**Required function:** Define `banner()` (no parameters) that prints the three banner lines, and call it once per repeat.

**Input Format:** A single integer `n` (1 ≤ n ≤ 20).

**Output Format:** The 3-line banner printed `n` times — `3 × n` lines in total, no blank lines between repeats.

**Sample Input:**
```
2
```
**Sample Output:**
```
=====
MENU
=====
=====
MENU
=====
```

---

## Problem 2 — Times Table

Define a function that prints one number's multiplication table.

**Task:** Read an integer `k` and print its table from `k × 1` to `k × 10` on a single line, values separated by single spaces.

**Required function:** Define `table(k)` that prints the ten products, and call it with the value read from input.

**Input Format:** A single integer `k` (1 ≤ k ≤ 100).

**Output Format:** One line with the ten products `k×1 k×2 … k×10`, separated by single spaces.

**Sample Input:**
```
7
```
**Sample Output:**
```
7 14 21 28 35 42 49 56 63 70
```

---

## Problem 3 — Digit Sum

Define a function that prints the sum of a number's digits.

**Task:** Read an integer `n` and print the sum of its digits.

**Required function:** Define `digit_sum(n)` that computes and prints the digit sum, and call it with the value read from input.

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

## Problem 4 — Even Numbers Up To N

Define a function that prints the even numbers up to a limit.

**Task:** Read an integer `n` and print every even number from 2 up to and including `n` (if `n` is even) on a single line, separated by single spaces. If `n` is odd, stop at the largest even number below it.

**Required function:** Define `evens(n)` that prints the even numbers, and call it with the value read from input.

**Input Format:** A single integer `n` (2 ≤ n ≤ 100).

**Output Format:** One line of even numbers from 2 upward, separated by single spaces.

**Sample Input:**
```
10
```
**Sample Output:**
```
2 4 6 8 10
```

---

## Problem 5 — Star Triangle

Define a function that prints a left-aligned triangle of stars.

**Task:** Read an integer `n` and print a triangle with `n` rows, where row `i` contains `i` stars (no spaces between stars).

**Required function:** Define `triangle(n)` that prints the triangle, and call it with the value read from input.

**Input Format:** A single integer `n` (1 ≤ n ≤ 50).

**Output Format:** `n` lines; the i-th line contains `i` star characters.

**Sample Input:**
```
4
```
**Sample Output:**
```
*
**
***
****
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases.*
