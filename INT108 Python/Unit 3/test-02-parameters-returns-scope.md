# Test 2 — Parameters, Returns & Scope

**Unit 3 · Functions and Recursion — covers Topics 04–06 (Parameters & Arguments, Return Values, Scope of Variables)**

*Section A: 10 multiple-choice questions (1 mark each).*
*Section B: 10 coding problems (3 marks each).*
*Total: 40 marks. Answer key in the separate file `test-02-parameters-returns-scope-answers.md`.*

---

## Section A — Multiple Choice (10 × 1 = 10 marks)

**A1.** What does this print?
```python
def div(a, b):
    print(a // b)

div(b=8, a=2)
```
- A) `0`
- B) `4`
- C) `2`
- D) An error

**A2.** What happens when this runs?
```python
def show(n):
    print(n)

x = show(5)
print(x + 1)
```
- A) It prints `5` then `6`
- B) It prints `5` then `1`
- C) It prints `6`
- D) It prints `5`, then an error on `x + 1`

**A3.** What does this print?
```python
def f(a, b=10):
    return a + b

print(f(3, 20))
```
- A) `13`
- B) `33`
- C) `23`
- D) An error — `b` already has a default

**A4.** What does this print?
```python
def first_even(n):
    for i in range(1, n + 1):
        if i % 2 == 0:
            return i
    return -1

print(first_even(5))
```
- A) `4`
- B) `2`
- C) `2 4`
- D) `-1`

**A5.** What does this print?
```python
def f(a, b):
    return b, a

x, y = f(1, 2)
print(x, y)
```
- A) `1 2`
- B) `1 1`
- C) `2 1`
- D) `2 2`

**A6.** What does this print?
```python
v = 5

def bump(v):
    return v + 1

v = bump(v)
print(v)
```
- A) `5`
- B) `6`
- C) `1`
- D) An error

**A7.** What happens when this runs?
```python
s = 100

def f():
    s = s + 1
    return s

print(f())
```
- A) It prints `101`
- B) It prints `100`
- C) It prints `1`
- D) An error — `s` is treated as local but used before assignment

**A8.** What does this print?
```python
def dbl(n):
    return n * 2

def inc(n):
    return n + 1

print(dbl(inc(4)))
```
- A) `10`
- B) `9`
- C) `12`
- D) `8`

**A9.** What happens when this runs?
```python
def area(l, w):
    return l * w

print(area(5))
```
- A) It prints `5`
- B) It prints `25`
- C) It prints `0`
- D) An error — one argument is missing

**A10.** What does this print?
```python
k = 100

def f(k):
    return k * k

print(f(3))
print(k)
```
- A) `9` then `9`
- B) `9` then `100`
- C) `100` then `100`
- D) `9` then `10000`

---

## Section B — Coding (10 × 3 = 30 marks)

*Platform-judge format: exact-match output. Each problem names a **Required function** you must define with the exact name and parameters given, then call. Functions should `return` their results; printing happens at the call site unless stated otherwise.*

---

### B1 — Simple Interest

**Task:** Compute simple interest. For principal `P`, rate `R` percent per year, and time `T` years, the interest is `P × R × T ÷ 100` (use integer division).

**Required function:** Define `simple_interest(p, r, t)` that **returns** the interest. Read the three values, call it, and print the result.

**Input Format:** Three integers, each on its own line — `p`, `r`, then `t` (1 ≤ p ≤ 1000000, 0 ≤ r ≤ 100, 0 ≤ t ≤ 100).

**Output Format:** A single integer — the simple interest.

**Sample Input:**
```
1000
5
2
```
**Sample Output:**
```
100
```

---

### B2 — Primes in a Range

**Task:** Read two integers `a` and `b` and print how many prime numbers lie in the range `a` to `b` (inclusive).

**Required functions:** Define `is_prime(n)` returning `True`/`False`, and `count_in_range(a, b)` that uses it and **returns** the count. Print the result.

**Input Format:** Two integers, each on its own line — `a` then `b` (2 ≤ a ≤ b ≤ 5000).

**Output Format:** A single integer — the number of primes in the range.

**Sample Input:**
```
10
30
```
**Sample Output:**
```
6
```

---

### B3 — Harshad Number

**Task:** A **Harshad number** is divisible by the sum of its own digits. Read an integer and print `Yes` if it is a Harshad number, otherwise `No`.

**Required functions:** Define `digit_sum(n)` that **returns** the digit sum, and `is_harshad(n)` that uses it and **returns** a boolean. Use the boolean in the main program to print `Yes` or `No`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 1000000).

**Output Format:** Either `Yes` or `No`.

**Sample Input:**
```
18
```
**Sample Output:**
```
Yes
```

---

### B4 — LCM Through GCD

**Task:** Read two integers and print their lowest common multiple (LCM). Use the fact that `LCM(a, b) = a × b ÷ GCD(a, b)`.

**Required functions:** Define `gcd(a, b)` that **returns** the greatest common divisor (Euclid's method), and `lcm(a, b)` that calls it and **returns** the LCM. Print the result.

**Input Format:** Two integers, each on its own line (1 ≤ each ≤ 100000).

**Output Format:** A single integer — the LCM.

**Sample Input:**
```
12
18
```
**Sample Output:**
```
36
```

---

### B5 — Quotient and Remainder

**Task:** Read two integers `a` and `b` and print the quotient and remainder of `a ÷ b`, separated by a space.

**Required function:** Define `quotient_remainder(a, b)` that **returns two values** — the quotient and the remainder. Unpack them and print both, separated by a space.

**Input Format:** Two integers, each on its own line — `a` then `b` (0 ≤ a ≤ 1000000, 1 ≤ b ≤ 1000).

**Output Format:** Two integers separated by a space: the quotient, then the remainder.

**Sample Input:**
```
17
5
```
**Sample Output:**
```
3 2
```

---

### B6 — Combinations (nCr)

**Task:** Read `n` and `r` and print the number of ways to choose `r` items from `n`, which is `n! ÷ (r! × (n − r)!)`.

**Required functions:** Define `fact(n)` that **returns** the factorial, and `ncr(n, r)` that uses it and **returns** the result. Print it.

**Input Format:** Two integers, each on its own line — `n` then `r` (0 ≤ r ≤ n ≤ 12).

**Output Format:** A single integer — the value of nCr.

**Sample Input:**
```
5
2
```
**Sample Output:**
```
10
```

---

### B7 — Average Speed

**Task:** Read a distance (in km) and a time (in hours) and print the average speed in km/h, to exactly 2 decimal places.

**Required function:** Define `average_speed(d, t)` that **returns** distance ÷ time. Print the returned value formatted to 2 decimal places using `f"{value:.2f}"`.

**Input Format:** Two integers, each on its own line — `d` then `t` (1 ≤ d ≤ 100000, 1 ≤ t ≤ 1000).

**Output Format:** The average speed, to exactly 2 decimal places.

**Sample Input:**
```
150
4
```
**Sample Output:**
```
37.50
```

---

### B8 — Spread of Three

**Task:** Read three integers and print the difference between the largest and the smallest (the "spread").

**Required functions:** Define `max_of_three(a, b, c)` and `min_of_three(a, b, c)`, each **returning** its result using `if` comparisons (no built-in `max`/`min`). In the main program, print their difference.

**Input Format:** Three integers, each on its own line.

**Output Format:** A single integer — the largest minus the smallest.

**Sample Input:**
```
7
2
9
```
**Sample Output:**
```
7
```

---

### B9 — Yearly Growth

**Task:** An amount grows by 10% each year, with the growth rounded down each year using integer division (`amount = amount + amount // 10`). Read a starting amount and a number of years, and print the amount after that many years.

**Required function:** Define `grow(amount, years)` that applies the yearly growth in a loop and **returns** the final amount. Print it.

**Input Format:** Two integers, each on its own line — `amount` then `years` (1 ≤ amount ≤ 1000000, 0 ≤ years ≤ 50).

**Output Format:** A single integer — the amount after the given years.

**Sample Input:**
```
100
3
```
**Sample Output:**
```
133
```

---

### B10 — Perfect Number

**Task:** A **perfect number** equals the sum of its proper divisors (all divisors except itself) — for example, 28 = 1 + 2 + 4 + 7 + 14. Read an integer and print `Yes` if it is perfect, otherwise `No`.

**Required functions:** Define `divisor_sum(n)` that **returns** the sum of proper divisors, and `is_perfect(n)` that uses it and **returns** a boolean. Use the boolean to print `Yes` or `No`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 100000).

**Output Format:** Either `Yes` or `No`.

**Sample Input:**
```
28
```
**Sample Output:**
```
Yes
```

---

*End of Test 2. Section A: 10 marks · Section B: 30 marks · Total: 40 marks.*
