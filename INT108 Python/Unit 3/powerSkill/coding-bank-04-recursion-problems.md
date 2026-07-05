# Coding Bank — Batch 4: Recursion (61–80)

*Unit 3 · Functions and Recursion. Judge-format: read input with `input()`/`int()` in the exact order given, produce exact-match output. Each names a **Required function** you must define.*

***Every solution must be recursive*** — the function calls itself with a base condition that stops it. **No loops (`for`/`while`) are allowed** — a loop solution will not be accepted even if its output is correct (checked at code review).

*Every problem outputs a **computed value** (a count, sum, or number) — never a guessable label. Difficulty: [E] easy · [M] medium · [H] hard. Reference solutions in `coding-bank-04-recursion-solutions.md`.*

---

## 61 — Factorial  [E]

Print `n!` computed recursively.

**Required function:** `fact(n)` — returns 1 when `n` is 0, else `n * fact(n - 1)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 12).

**Output Format:** A single integer — the factorial.

**Sample Input:**
```
5
```
**Sample Output:**
```
120
```

---

## 62 — Sum to N  [E]

Print the sum 1 + 2 + … + n computed recursively.

**Required function:** `sum_to(n)` — returns 0 when `n` is 0, else `n + sum_to(n - 1)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 10000).

**Output Format:** A single integer — the sum.

**Sample Input:**
```
10
```
**Sample Output:**
```
55
```

---

## 63 — Nth Fibonacci  [M]

Print the `n`-th Fibonacci number recursively, where `fib(0) = 0` and `fib(1) = 1`.

**Required function:** `fib(n)` — returns `n` when `n < 2`, else `fib(n - 1) + fib(n - 2)`.

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

## 64 — Power  [M]

Print `base` raised to `exp`, computed recursively (no `**`, no loops).

**Required function:** `power(base, exp)` — returns 1 when `exp` is 0, else `base * power(base, exp - 1)`.

**Input Format:** Two integers, each on its own line — base, then exponent (1 ≤ base ≤ 100, 0 ≤ exp ≤ 15).

**Output Format:** A single integer — `base` raised to `exp`.

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

## 65 — Digit Sum  [M]

Print the sum of the digits of `n`, computed recursively.

**Required function:** `dsum(n)` — returns 0 when `n` is 0, else `n % 10 + dsum(n // 10)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the digit sum.

**Sample Input:**
```
472
```
**Sample Output:**
```
13
```

---

## 66 — Count Digits  [M]

Print how many digits `n` has, computed recursively.

**Required function:** `ndigits(n)` — returns 1 when `n < 10`, else `1 + ndigits(n // 10)`.

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

## 67 — GCD  [M]

Print the greatest common divisor of two integers, computed recursively with Euclid's rule.

**Required function:** `gcd(a, b)` — returns `a` when `b` is 0, else `gcd(b, a % b)`.

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

## 68 — Sum of Squares  [M]

Print 1² + 2² + … + n², computed recursively.

**Required function:** `sumsq(n)` — returns 0 when `n` is 0, else `n * n + sumsq(n - 1)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000).

**Output Format:** A single integer — the sum of squares.

**Sample Input:**
```
3
```
**Sample Output:**
```
14
```

---

## 69 — Product of a Range  [M]

Read two integers `a` and `b` (with `a ≤ b`) and print the product a × (a+1) × … × b, computed recursively.

**Required function:** `product(a, b)` — returns 1 when `a > b`, else `a * product(a + 1, b)`.

**Input Format:** Two integers, each on its own line — `a` then `b` (1 ≤ a ≤ b ≤ 12).

**Output Format:** A single integer — the product.

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

## 70 — Count Odd Digits  [M]

Print how many digits of `n` are odd, computed recursively.

**Required function:** `odd_count(n)` — returns 0 when `n` is 0, else `(n % 10) % 2 + odd_count(n // 10)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the count of odd digits.

**Sample Input:**
```
13579
```
**Sample Output:**
```
5
```

---

## 71 — Reverse a Number  [H]

Print the digits of `n` in reverse order, computed recursively using an accumulator.

**Required function:** `rev(n, acc)` — returns `acc` when `n` is 0, else `rev(n // 10, acc * 10 + n % 10)`. Call it as `rev(n, 0)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the digits of `n` reversed (leading zeros naturally disappear).

**Sample Input:**
```
1234
```
**Sample Output:**
```
4321
```

---

## 72 — Digital Root  [H]

The digital root is found by summing digits repeatedly until one digit remains. Print it, using two recursive functions.

**Required functions:** `dsum(n)` returning the recursive digit sum, and `droot(n)` returning `n` when `n < 10`, else `droot(dsum(n))`.

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

## 73 — Sum of First N Even Numbers  [M]

Print 2 + 4 + … + 2n (the first `n` even numbers), computed recursively.

**Required function:** `even_sum(n)` — returns 0 when `n` is 0, else `2 * n + even_sum(n - 1)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 10000).

**Output Format:** A single integer — the sum of the first `n` even numbers.

**Sample Input:**
```
4
```
**Sample Output:**
```
20
```

---

## 74 — Count a Digit  [H]

Read a number `n` and a digit `d`, and print how many times `d` appears in `n`, computed recursively.

**Required function:** `count_digit(n, d)` — returns 0 when `n` is 0, else adds 1 when the last digit equals `d` and recurses on `n // 10`.

**Input Format:** Two integers, each on its own line — `n` then `d` (0 ≤ n ≤ 10000000, 0 ≤ d ≤ 9).

**Output Format:** A single integer — how many times `d` appears in `n`.

**Sample Input:**
```
1213121
1
```
**Sample Output:**
```
4
```

---

## 75 — Geometric Term  [H]

A geometric sequence starts at `a` and multiplies by `r` each step. Print its `n`-th term, `a × r^(n−1)`, computed recursively (no `**`, no loops).

**Required function:** `geo(a, r, n)` — returns `a` when `n` is 1, else `r * geo(a, r, n - 1)`.

**Input Format:** Three integers, each on its own line — first term `a`, ratio `r`, position `n` (1 ≤ a,r ≤ 100, 1 ≤ n ≤ 10).

**Output Format:** A single integer — the `n`-th term.

**Sample Input:**
```
2
3
4
```
**Sample Output:**
```
54
```

---

## 76 — Steps to a Single Digit  [H]

Repeatedly replacing `n` by its digit sum eventually leaves one digit. Print how many such steps it takes (0 if `n` is already a single digit), using two recursive functions.

**Required functions:** `dsum(n)` returning the recursive digit sum, and `steps(n)` returning 0 when `n < 10`, else `1 + steps(dsum(n))`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the number of steps.

**Sample Input:**
```
9875
```
**Sample Output:**
```
3
```

---

## 77 — Sum of Multiples of Three  [M]

Print the sum of all multiples of 3 from 1 to `n`, computed recursively.

**Required function:** `mult3_sum(n)` — returns 0 when `n` is 0; when `n` is a multiple of 3, adds `n` and recurses on `n − 1`; otherwise just recurses on `n − 1`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 10000).

**Output Format:** A single integer — the sum of multiples of 3 up to `n`.

**Sample Input:**
```
10
```
**Sample Output:**
```
18
```

---

## 78 — Count Ones in Binary  [H]

Print how many 1-bits are in the binary representation of `n`, computed recursively (by repeatedly taking `n % 2` and recursing on `n // 2`).

**Required function:** `ones(n)` — returns 0 when `n` is 0, else `n % 2 + ones(n // 2)`.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the number of 1-bits.

**Sample Input:**
```
13
```
**Sample Output:**
```
3
```

---

## 79 — Triangular of Triangular  [H]

The `k`-th triangular number is 1 + 2 + … + k. Read `k`, compute its triangular number `t`, then print the `t`-th triangular number — using one recursive triangular function applied twice.

**Required function:** `tri(n)` — returns 0 when `n` is 0, else `n + tri(n - 1)`. Print `tri(tri(k))`.

**Input Format:** A single integer `k` (0 ≤ k ≤ 20).

**Output Format:** A single integer — the triangular number of the triangular number of `k`.

**Sample Input:**
```
3
```
**Sample Output:**
```
21
```

---

## 80 — Count Large Digits  [H]

Read a number `n` and a threshold `t`, and print how many digits of `n` are greater than or equal to `t`, computed recursively.

**Required function:** `big_count(n, t)` — returns 0 when `n` is 0, else adds 1 when the last digit is ≥ `t` and recurses on `n // 10`.

**Input Format:** Two integers, each on its own line — `n` then `t` (0 ≤ n ≤ 1000000, 0 ≤ t ≤ 9).

**Output Format:** A single integer — how many digits are ≥ `t`.

**Sample Input:**
```
58317
5
```
**Sample Output:**
```
3
```

---

*End of Batch 4 — 20 recursion problems. Every solution is strictly recursive with a base case; every output is a computed value. All reference solutions verified against the sample and base-case edges.*
