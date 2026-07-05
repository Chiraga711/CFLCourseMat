# Test 3 — Math Module & Recursion

**Unit 3 · Functions and Recursion — covers Topics 07–08 (Math Module, Recursion)**

*Section A: 10 multiple-choice questions (1 mark each).*
*Section B: 10 coding problems (3 marks each).*
*Total: 40 marks. Answer key in the separate file `test-03-math-module-recursion-answers.md`.*

---

## Section A — Multiple Choice (10 × 1 = 10 marks)

**A1.** What does this print?
```python
import math
print(math.floor(math.sqrt(30)))
```
- A) `6`
- B) `5.4`
- C) `5`
- D) `5.0`

**A2.** What does this print?
```python
import math
print(int(math.pow(2, 3)) + math.sqrt(16))
```
- A) `12`
- B) `8.0`
- C) An error
- D) `12.0`

**A3.** What does this print?
```python
def m(n):
    if n == 0:
        return
    m(n - 1)
    print(n * n)

m(3)
```
- A) `1 4 9`
- B) `9 4 1`
- C) `1 2 3`
- D) `9 4 1 0`

**A4.** What does this print?
```python
import math
print(math.ceil(12 / 4))
```
- A) `4`
- B) `3.0`
- C) `12`
- D) `3`

**A5.** What does this print?
```python
def g(n):
    if n <= 1:
        return 1
    return n * g(n - 2)

print(g(4))
```
- A) `24`
- B) `6`
- C) `8`
- D) `4`

**A6.** What does this print?
```python
import math
print(math.sqrt(25) == 5)
```
- A) `True`
- B) `False`
- C) `5.0`
- D) An error

**A7.** What does this print?
```python
def h(n):
    if n == 0:
        return
    print(n)
    h(n - 1)
    print(n)

h(2)
```
- A) `2 1 2`
- B) `2 1 1 2`
- C) `1 2 2 1`
- D) `2 1`

**A8.** What does this print?
```python
def mystery(n):
    if n == 0:
        return 0
    return 1 + mystery(n // 2)

print(mystery(20))
```
- A) `4`
- B) `5`
- C) `20`
- D) `10`

**A9.** What does this print?
```python
import math
print(math.floor(-1.5))
```
- A) `-2`
- B) `-1`
- C) `2`
- D) `-1.5`

**A10.** What does this print?
```python
def p(b, e):
    if e == 0:
        return 1
    return b * p(b, e - 1)

print(p(3, 0))
```
- A) `3`
- B) `0`
- C) `9`
- D) `1`

---

## Section B — Coding (10 × 3 = 30 marks)

*Platform-judge format: exact-match output. Each problem names a **Required function**. Problems marked **(recursive)** must use recursion with a base case and **no loops** — checked on review. Problems marked **(math module)** must `import math`. The `**` operator is not used anywhere in this course; use multiplication or `math.pow`.*

---

### B1 — Digital Root (recursive)

**Task:** The *digital root* of a number is found by summing its digits, then summing the digits of that result, and so on until a single digit remains. For 9875 → 9+8+7+5 = 29 → 2+9 = 11 → 1+1 = 2. Read an integer and print its digital root.

**Required functions:** Define `dsum(n)` that **returns** the digit sum **recursively**, and `digital_root(n)` that **returns** `n` when `n < 10`, otherwise **returns** `digital_root(dsum(n))`. Both recursive, no loops.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the digital root (0–9).

**Sample Input:**
```
9875
```
**Sample Output:**
```
2
```

---

### B2 — Circle Area (math module)

**Task:** Read a radius and print the area of the circle, π r², to exactly 2 decimal places. Use `math.pi`.

**Required function:** Define `circle_area(r)` that **returns** `math.pi * r * r`. Print the result with `f"{value:.2f}"`.

**Input Format:** A single integer `r` (1 ≤ r ≤ 10000).

**Output Format:** The area, to exactly 2 decimal places.

**Sample Input:**
```
5
```
**Sample Output:**
```
78.54
```

---

### B3 — GCD (recursive)

**Task:** Read two integers and print their greatest common divisor, computed recursively with Euclid's rule: `gcd(a, b) = gcd(b, a mod b)`, and `gcd(a, 0) = a`.

**Required function:** Define `gcd(a, b)` that **returns** `a` when `b` is 0 (base case), otherwise **returns** `gcd(b, a % b)`. No loops.

**Input Format:** Two integers, each on its own line (1 ≤ each ≤ 1000000).

**Output Format:** A single integer — the GCD.

**Sample Input:**
```
48
36
```
**Sample Output:**
```
12
```

---

### B4 — Distance Between Two Points (math module)

**Task:** Read the coordinates of two points — `x1, y1, x2, y2`, one per line — and print the straight-line distance between them, √((x2−x1)² + (y2−y1)²), to exactly 2 decimal places.

**Required function:** Define `distance(x1, y1, x2, y2)` that computes the differences, uses `math.sqrt` (write the squares as `dx * dx`, not `dx ** 2`), and **returns** the distance. Print it with `f"{value:.2f}"`.

**Input Format:** Four integers, each on its own line — `x1`, `y1`, `x2`, `y2` (−10000 ≤ each ≤ 10000).

**Output Format:** The distance, to exactly 2 decimal places.

**Sample Input:**
```
0
0
3
4
```
**Sample Output:**
```
5.00
```

---

### B5 — Sum of Squares (recursive)

**Task:** Read an integer `n` and print 1² + 2² + … + n², computed recursively.

**Required function:** Define `sum_squares(n)` that **returns** 0 when `n` is 0 (base case), otherwise **returns** `n * n + sum_squares(n - 1)`. No loops.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000).

**Output Format:** A single integer — the sum of squares from 1 to `n`.

**Sample Input:**
```
3
```
**Sample Output:**
```
14
```

---

### B6 — Buses Needed (math module)

**Task:** `p` people must travel, and each bus holds `cap` people. Print the number of buses needed so everyone travels (a partly filled bus still counts).

**Required function:** Define `buses_needed(p, cap)` that **returns** `math.ceil(p / cap)`. Print the result.

**Input Format:** Two integers, each on its own line — `p` then `cap` (1 ≤ p ≤ 1000000, 1 ≤ cap ≤ 1000).

**Output Format:** A single integer — the number of buses.

**Sample Input:**
```
130
40
```
**Sample Output:**
```
4
```

---

### B7 — Product of a Range (recursive)

**Task:** Read two integers `a` and `b` (with `a ≤ b`) and print the product a × (a+1) × … × b, computed recursively.

**Required function:** Define `product(a, b)` that **returns** 1 when `a > b` (base case), otherwise **returns** `a * product(a + 1, b)`. No loops.

**Input Format:** Two integers, each on its own line — `a` then `b` (1 ≤ a ≤ b ≤ 12).

**Output Format:** A single integer — the product of all integers from `a` to `b`.

**Sample Input:**
```
2
5
```
**Sample Output:**
```
120
```

---

### B8 — Integer Square Root (math module)

**Task:** Read an integer and print the largest whole number whose square is not greater than it — that is, ⌊√n⌋. For 50, the answer is 7 (because 7² = 49 ≤ 50 < 64 = 8²).

**Required function:** Define `int_sqrt(n)` that **returns** `math.floor(math.sqrt(n))`. Print the result.

**Input Format:** A single integer `n` (1 ≤ n ≤ 1000000).

**Output Format:** A single integer — the floor of the square root of `n`.

**Sample Input:**
```
50
```
**Sample Output:**
```
7
```

---

### B9 — Count Digits (recursive)

**Task:** Read an integer and print how many digits it has, computed recursively.

**Required function:** Define `num_digits(n)` that **returns** 1 when `n < 10` (base case), otherwise **returns** `1 + num_digits(n // 10)`. No loops.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the number of digits.

**Sample Input:**
```
40725
```
**Sample Output:**
```
5
```

---

### B10 — Compound Interest (math module)

**Task:** Money grows by compound interest. For principal `P`, rate `R` percent per year, and `T` years, the final amount is `P × (1 + R/100)^T`. Read the three values and print the final amount as a whole number (use `int()` to drop any fraction).

**Required function:** Define `compound(p, r, t)` that uses `math.pow` for the `(1 + r/100)` raised to `t` part and **returns** `p * math.pow(1 + r / 100, t)`. Print `int()` of the returned value.

**Input Format:** Three integers, each on its own line — `p`, `r`, then `t` (1 ≤ p ≤ 1000000, 0 ≤ r ≤ 100, 0 ≤ t ≤ 30).

**Output Format:** A single integer — the final amount, with any fraction dropped.

**Sample Input:**
```
1000
10
2
```
**Sample Output:**
```
1210
```

---

*End of Test 3. Section A: 10 marks · Section B: 30 marks · Total: 40 marks.*
