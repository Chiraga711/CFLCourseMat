# Coding Bank — Batch 2: Formula & Maths Problems (21–40)

*Unit 3 · Functions and Recursion. Judge-format: read input with `input()`/`int()` in the exact order given, produce exact-match output. Each names a **Required function**. Powers use `math.pow` or repeated multiplication (never `**`); squares are written `x * x`.*

*Every problem outputs a **computed value** — a number that only comes out right if your logic is right — never a guessable label. Money and real-valued answers use `f"{value:.2f}"` (note `round()` drops trailing zeros and will fail the judge).*

*Difficulty: [E] easy · [M] medium · [H] hard. Reference solutions in `coding-bank-02-formula-solutions.md`.*

---

## 21 — Compound Interest  [H]

Money grows by compound interest: after `t` years at `r` percent per year, a principal `p` becomes `p × (1 + r/100)^t`. Print the final amount to 2 decimals. Use `math.pow` for the power.

**Required function:** `amount(p, r, t)` returning the final amount.

**Input Format:** Three integers, each on its own line — principal, rate percent, years (1 ≤ p ≤ 10000000, 0 ≤ r ≤ 100, 0 ≤ t ≤ 30).

**Output Format:** The final amount, to 2 decimals.

**Sample Input:**
```
1000
10
2
```
**Sample Output:**
```
1210.00
```

---

## 22 — Simple Interest  [E]

Simple interest on principal `p` at `r` percent per year for `t` years is `p × r × t ÷ 100`. Print it as a whole number (use integer division).

**Required function:** `si(p, r, t)` returning the interest.

**Input Format:** Three integers, each on its own line — principal, rate, years (1 ≤ p ≤ 1000000, 0 ≤ r ≤ 100, 0 ≤ t ≤ 100).

**Output Format:** A single integer — the simple interest.

**Sample Input:**
```
25000
8
3
```
**Sample Output:**
```
6000
```

---

## 23 — Loan Instalment  [M]

A loan of `principal` is repaid over `months` months. Flat interest of `rate` percent is added to the whole principal, then the total is split into equal monthly instalments. Print the instalment amount and the leftover (the remainder that doesn't divide evenly), separated by a space.

**Required function:** `emi_total(principal, months, rate)` returning the total amount to repay (principal plus flat interest).

**Input Format:** Three integers, each on its own line — principal, months, rate percent (1 ≤ principal ≤ 10000000, 1 ≤ months ≤ 120, 0 ≤ rate ≤ 100).

**Output Format:** Two integers separated by a space: the whole monthly instalment, then the leftover.

**Sample Input:**
```
12000
12
10
```
**Sample Output:**
```
1100 0
```

---

## 24 — Profit Percent  [M]

Given the cost price and selling price of an item, print the profit percentage as a whole number (use integer division). A loss gives a negative value.

**Required function:** `profit_percent(cost, sell)` returning the percentage.

**Input Format:** Two integers, each on its own line — cost price, then selling price (1 ≤ cost ≤ 1000000, 0 ≤ sell ≤ 10000000).

**Output Format:** A single integer — the profit percent (negative for a loss).

**Sample Input:**
```
200
250
```
**Sample Output:**
```
25
```

---

## 25 — Washer Area  [M]

A flat ring (washer) has outer radius `R` and inner radius `r`. Its area is π(R² − r²). Print it to 2 decimals, using `math.pi`.

**Required function:** `ring_area(R, r)` returning the area.

**Input Format:** Two integers, each on its own line — outer radius `R`, then inner radius `r` (1 ≤ r < R ≤ 10000).

**Output Format:** The area, to 2 decimals.

**Sample Input:**
```
5
3
```
**Sample Output:**
```
50.27
```

---

## 26 — Triangle Area (Heron)  [H]

Given the three side lengths of a triangle, use Heron's formula to print its area to 2 decimals: let `s = (a+b+c)/2`, then area = √(s(s−a)(s−b)(s−c)). Use `math.sqrt`.

**Required function:** `tri_area(a, b, c)` returning the area.

**Input Format:** Three integers, each on its own line — the side lengths (they always form a valid triangle; 1 ≤ each ≤ 1000).

**Output Format:** The area, to 2 decimals.

**Sample Input:**
```
3
4
5
```
**Sample Output:**
```
6.00
```

---

## 27 — Distance Between Points  [M]

Given two points `(x1, y1)` and `(x2, y2)`, print the straight-line distance between them to 2 decimals. Write the squares as `dx * dx` (not `dx ** 2`) and use `math.sqrt`.

**Required function:** `dist(x1, y1, x2, y2)` returning the distance.

**Input Format:** Four integers, each on its own line — `x1`, `y1`, `x2`, `y2` (−10000 ≤ each ≤ 10000).

**Output Format:** The distance, to 2 decimals.

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

## 28 — Cone Volume  [H]

A cone has base radius `r` and height `h`. Its volume is `π r² h ÷ 3`. Print it to 2 decimals, using `math.pi`.

**Required function:** `cone_volume(r, h)` returning the volume.

**Input Format:** Two integers, each on its own line — radius, then height (1 ≤ each ≤ 1000).

**Output Format:** The volume, to 2 decimals.

**Sample Input:**
```
3
7
```
**Sample Output:**
```
65.97
```

---

## 29 — Cylinder Surface Area  [H]

A closed cylinder has radius `r` and height `h`. Its total surface area is `2π r (r + h)`. Print it to 2 decimals, using `math.pi`.

**Required function:** `cylinder_surface(r, h)` returning the surface area.

**Input Format:** Two integers, each on its own line — radius, then height (1 ≤ each ≤ 1000).

**Output Format:** The surface area, to 2 decimals.

**Sample Input:**
```
3
5
```
**Sample Output:**
```
150.80
```

---

## 30 — Sum of Cubed Digits  [M]

Print the sum of the cubes of the digits of `n`. (For example, 153 gives 1³ + 5³ + 3³ = 153.)

**Required function:** `cube_digit_sum(n)` returning the sum of the cubes of the digits.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the sum of the cubed digits.

**Sample Input:**
```
153
```
**Sample Output:**
```
153
```

---

## 31 — Sum of Proper Divisors  [M]

Print the sum of all proper divisors of `n` (every divisor except `n` itself). For example, 28 gives 1 + 2 + 4 + 7 + 14 = 28.

**Required function:** `divisor_sum(n)` returning the sum of proper divisors.

**Input Format:** A single integer `n` (1 ≤ n ≤ 100000).

**Output Format:** A single integer — the sum of proper divisors (0 for `n = 1`).

**Sample Input:**
```
28
```
**Sample Output:**
```
28
```

---

## 32 — GCD and LCM  [H]

Print the greatest common divisor and the lowest common multiple of two integers, separated by a space. Use `LCM(a, b) = a × b ÷ GCD(a, b)`.

**Required functions:** `gcd(a, b)` returning the GCD, and `lcm(a, b)` returning the LCM.

**Input Format:** Two integers, each on its own line (1 ≤ each ≤ 100000).

**Output Format:** Two integers separated by a space: the GCD, then the LCM.

**Sample Input:**
```
12
18
```
**Sample Output:**
```
6 36
```

---

## 33 — Planet C Leap Count  [H]

On planet C a year is a leap year if it is divisible by 7, **except** when it is also divisible by 35 or by 77. Print how many leap years there are from 1 to `n` inclusive.

**Required function:** `count_leaps(n)` returning the number of planet-C leap years up to `n`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 1000000).

**Output Format:** A single integer — the count of leap years.

**Sample Input:**
```
100
```
**Sample Output:**
```
11
```

---

## 34 — Product of Digits  [M]

Print the product of the digits of `n`. (If any digit is 0, the product is 0.)

**Required function:** `digit_product(n)` returning the product of the digits.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the product of the digits.

**Sample Input:**
```
234
```
**Sample Output:**
```
24
```

---

## 35 — Count Primes  [H]

Print how many prime numbers there are from 2 to `n` inclusive.

**Required functions:** `is_prime(n)` returning whether `n` is prime, and `prime_count(n)` returning how many primes are in the range.

**Input Format:** A single integer `n` (2 ≤ n ≤ 5000).

**Output Format:** A single integer — the number of primes.

**Sample Input:**
```
20
```
**Sample Output:**
```
8
```

---

## 36 — Average Speed  [M]

A journey covers `d` kilometres in `t` hours. Print the average speed in km/h, to 2 decimals.

**Required function:** `avg_speed(d, t)` returning the speed.

**Input Format:** Two integers, each on its own line — distance in km, then time in hours (1 ≤ each ≤ 100000).

**Output Format:** The average speed, to 2 decimals.

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

## 37 — Celsius to Fahrenheit  [M]

Convert a Celsius temperature to Fahrenheit using `F = C × 9 ÷ 5 + 32`. Print the result to 2 decimals.

**Required function:** `celsius_to_f(c)` returning the Fahrenheit value.

**Input Format:** A single integer `c` (−100 ≤ c ≤ 1000).

**Output Format:** The Fahrenheit temperature, to 2 decimals.

**Sample Input:**
```
37
```
**Sample Output:**
```
98.60
```

---

## 38 — Density  [M]

Density is mass divided by volume. Print the density to 2 decimals.

**Required function:** `density(m, v)` returning mass ÷ volume.

**Input Format:** Two integers, each on its own line — mass, then volume (1 ≤ each ≤ 1000000).

**Output Format:** The density, to 2 decimals.

**Sample Input:**
```
100
8
```
**Sample Output:**
```
12.50
```

---

## 39 — Kinetic Energy  [M]

The kinetic energy of a body is `½ m v²`. Print it to 2 decimals. Write `v²` as `v * v` (not `v ** 2`).

**Required function:** `kinetic_energy(m, v)` returning the energy.

**Input Format:** Two integers, each on its own line — mass, then velocity (1 ≤ each ≤ 10000).

**Output Format:** The kinetic energy, to 2 decimals.

**Sample Input:**
```
10
4
```
**Sample Output:**
```
80.00
```

---

## 40 — Projectile Range  [H]

A projectile launched horizontally-scaled has range `v² ÷ g` for launch speed `v` and gravity `g`. Print the range to 2 decimals, writing `v²` as `v * v`.

**Required function:** `projectile_range(v, g)` returning the range.

**Input Format:** Two integers, each on its own line — speed, then gravity (1 ≤ each ≤ 1000).

**Output Format:** The range, to 2 decimals.

**Sample Input:**
```
20
10
```
**Sample Output:**
```
40.00
```

---

*End of Batch 2 — 20 formula & maths problems. Every output is a computed value (no guessable labels). All reference solutions verified against the sample and extra cases.*
