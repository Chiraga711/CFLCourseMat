# Coding Bank — Batch 3: Core Function Mechanics (41–60)

*Unit 3 · Functions and Recursion. Judge-format: read input with `input()`/`int()` in the exact order given, produce exact-match output. Each names a **Required function** you must define with the exact name and signature. Powers use loops or `math.pow` (never `**`); augmented operators (`+=`, `*=`) are allowed.*

*Every problem outputs a **computed value** — never a guessable label like `Yes`/`True`/`Pass`. Where a check is needed, the program prints the resulting count or number, so the answer can't be hardcoded.*

*Covers user-defined functions, parameters & arguments (including defaults), return values (including multiple returns), and scope. Difficulty: [E] easy · [M] medium · [H] hard. Reference solutions in `coding-bank-03-core-solutions.md`.*

---

## 41 — List Divisors  [E]

Read an integer `n` and print all its divisors (the numbers that divide it exactly) in increasing order on one line, separated by single spaces.

**Required function:** `divisors(n)` that prints the divisors.

**Input Format:** A single integer `n` (1 ≤ n ≤ 100000).

**Output Format:** The divisors of `n` in increasing order, separated by single spaces.

**Sample Input:**
```
12
```
**Sample Output:**
```
1 2 3 4 6 12
```

---

## 42 — Range Sum  [E]

Print the sum of all integers from `a` to `b` inclusive.

**Required function:** `range_sum(a, b)` returning the sum.

**Input Format:** Two integers, each on its own line — `a` then `b` (−10000 ≤ a ≤ b ≤ 10000).

**Output Format:** A single integer — the sum.

**Sample Input:**
```
3
7
```
**Sample Output:**
```
25
```

---

## 43 — Count Large Digits  [M]

Read a number `n` and a threshold `t`, and print how many digits of `n` are greater than or equal to `t`.

**Required function:** `count_big_digits(n, t)` returning the count.

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

## 44 — Arithmetic Sequence Term  [M]

An arithmetic sequence starts at `a` and increases by `d` each step. Print its `n`-th term, which is `a + (n−1)×d`.

**Required function:** `nth_term(a, d, n)` returning the term.

**Input Format:** Three integers, each on its own line — first term `a`, common difference `d`, position `n` (−1000 ≤ a,d ≤ 1000, 1 ≤ n ≤ 10000).

**Output Format:** A single integer — the `n`-th term.

**Sample Input:**
```
2
3
5
```
**Sample Output:**
```
14
```

---

## 45 — Largest of Three  [M]

Print the largest of three integers, without using the built-in `max()`.

**Required function:** `max3(a, b, c)` returning the largest, using `if` comparisons.

**Input Format:** Three integers, each on its own line.

**Output Format:** A single integer — the largest value.

**Sample Input:**
```
3
9
5
```
**Sample Output:**
```
9
```

---

## 46 — Weighted Score  [M]

A score is multiplied by a weight. Read a score and a weight, and print two values: the score with the given weight, and the score with the **default** weight of 2 — separated by a space.

**Required function:** `weighted(marks, weight=2)` returning the weighted score.

**Input Format:** Two integers, each on its own line — score, then weight (0 ≤ each ≤ 10000).

**Output Format:** Two integers separated by a space: weighted by the given weight, then by the default 2.

**Sample Input:**
```
10
5
```
**Sample Output:**
```
50 20
```

---

## 47 — Rectangle Perimeter and Area  [M]

Read a rectangle's length and width. Print its perimeter and area, separated by a space.

**Required function:** `rect(l, w)` returning **two values** — the perimeter `2(l+w)` and the area `l×w`.

**Input Format:** Two integers, each on its own line — length, then width (1 ≤ each ≤ 10000).

**Output Format:** Two integers separated by a space: perimeter, then area.

**Sample Input:**
```
4
3
```
**Sample Output:**
```
14 12
```

---

## 48 — Clamp a Value  [M]

"Clamping" forces a value to stay within a range: below the low bound it becomes the low bound, above the high bound it becomes the high bound, otherwise it stays. Print the clamped value.

**Required function:** `clamp(x, lo, hi)` returning the clamped value.

**Input Format:** Three integers, each on its own line — `x`, `lo`, `hi` (lo ≤ hi).

**Output Format:** A single integer — the clamped value.

**Sample Input:**
```
15
1
10
```
**Sample Output:**
```
10
```

---

## 49 — Net Price After Discount  [M]

A price may have a discount percentage applied. Read a price and a discount, and print two values: the net price with the given discount, and the net price with the **default** discount of 0 (i.e. the full price) — separated by a space.

**Required function:** `net_price(price, discount=0)` returning `price − price × discount ÷ 100` (integer division).

**Input Format:** Two integers, each on its own line — price, then discount percent (1 ≤ price ≤ 1000000, 0 ≤ discount ≤ 100).

**Output Format:** Two integers separated by a space: net with the given discount, then with the default 0.

**Sample Input:**
```
1000
20
```
**Sample Output:**
```
800 1000
```

---

## 50 — Power with Default Exponent  [H]

Raise a base to an exponent, computed with a loop (no `**`). Read a base and an exponent, and print two values: the base raised to the given exponent, and the base raised to the **default** exponent of 2 — separated by a space.

**Required function:** `power(base, exp=2)` returning `base` raised to `exp`.

**Input Format:** Two integers, each on its own line — base, then exponent (1 ≤ base ≤ 100, 0 ≤ exp ≤ 10).

**Output Format:** Two integers separated by a space: base^exp, then base².

**Sample Input:**
```
3
4
```
**Sample Output:**
```
81 9
```

---

## 51 — Sum and Product  [M]

Read three integers. Print their sum and their product, separated by a space.

**Required function:** `sum_prod(a, b, c)` returning **two values** — the sum and the product.

**Input Format:** Three integers, each on its own line.

**Output Format:** Two integers separated by a space: the sum, then the product.

**Sample Input:**
```
2
3
4
```
**Sample Output:**
```
9 24
```

---

## 52 — Sum and Count of Evens  [M]

Read an integer `n`. Print two values: the sum of the even numbers from 1 to `n`, and how many even numbers there are — separated by a space.

**Required function:** `sum_count_even(n)` returning **two values** — the sum and the count.

**Input Format:** A single integer `n` (1 ≤ n ≤ 100000).

**Output Format:** Two integers separated by a space: sum of evens, then count of evens.

**Sample Input:**
```
10
```
**Sample Output:**
```
30 5
```

---

## 53 — Quotient and Remainder  [E]

Read two integers `a` and `b`. Print the quotient and remainder of `a ÷ b`, separated by a space.

**Required function:** `divmod2(a, b)` returning **two values** — the quotient and the remainder.

**Input Format:** Two integers, each on its own line — `a` then `b` (0 ≤ a ≤ 1000000, 1 ≤ b ≤ 1000).

**Output Format:** Two integers separated by a space: quotient, then remainder.

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

## 54 — Grade Points  [M]

Convert a marks value to grade points: 90 and above → 10; 75–89 → 8; 50–74 → 5; below 50 → 0. Print the grade points (a number, not a letter).

**Required function:** `grade_point(marks)` returning the grade points.

**Input Format:** A single integer `marks` (0 ≤ marks ≤ 100).

**Output Format:** A single integer — the grade points.

**Sample Input:**
```
85
```
**Sample Output:**
```
8
```

---

## 55 — Fibonacci Pair  [H]

Read `n` and print the `n`-th and `(n+1)`-th Fibonacci numbers, separated by a space, where `fib(0) = 0` and `fib(1) = 1`.

**Required function:** `fib_pair(n)` returning **two values** — the `n`-th and `(n+1)`-th Fibonacci numbers.

**Input Format:** A single integer `n` (0 ≤ n ≤ 40).

**Output Format:** Two integers separated by a space: the `n`-th, then the `(n+1)`-th Fibonacci number.

**Sample Input:**
```
5
```
**Sample Output:**
```
5 8
```

---

## 56 — Running Maximum (No Globals)  [M]

Four integers are read one at a time. The largest-so-far must be tracked using a helper that keeps **no global state** — it takes the current maximum and the new value and returns whichever is larger. Print the final maximum.

**Required function:** `bigger(current, value)` returning the larger of the two.

**Input Format:** Four integers, each on its own line.

**Output Format:** A single integer — the largest of the four.

**Sample Input:**
```
3
9
5
7
```
**Sample Output:**
```
9
```

---

## 57 — Local Stays Local  [M]

A function triples its parameter inside its own body. Read `x`, print the tripled value returned by the function **and** the original `x` afterward — showing the caller's variable is unchanged.

**Required function:** `triple(n)` that sets `n = n * 3` inside and returns `n`.

**Input Format:** A single integer `x` (−100000 ≤ x ≤ 100000).

**Output Format:** Two integers separated by a space: the tripled value, then the original `x`.

**Sample Input:**
```
5
```
**Sample Output:**
```
15 5
```

---

## 58 — Primes in a Range  [H]

Read two integers `a` and `b`, and print how many prime numbers lie between them inclusive.

**Required functions:** `is_prime(n)` returning whether `n` is prime, and `count_primes(a, b)` returning the count of primes in the range.

**Input Format:** Two integers, each on its own line — `a` then `b` (2 ≤ a ≤ b ≤ 5000).

**Output Format:** A single integer — the number of primes.

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

## 59 — Factorial by Accumulation  [M]

Compute `n!` by repeatedly multiplying, where the multiply step is done by a helper that takes the running product and the next value and returns their product (keeping no global state). Print `n!`.

**Required function:** `multiply(acc, x)` returning `acc × x`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 12).

**Output Format:** A single integer — `n!`.

**Sample Input:**
```
5
```
**Sample Output:**
```
120
```

---

## 60 — Count Multiples of Two Numbers  [M]

Read an integer `n`. Using one function that counts multiples of a given divisor up to `n`, print how many numbers from 1 to `n` are multiples of 3, and how many are multiples of 5 — separated by a space. (Each call keeps its own local counter.)

**Required function:** `count_multiples(n, k)` returning how many numbers from 1 to `n` are multiples of `k`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 100000).

**Output Format:** Two integers separated by a space: multiples of 3, then multiples of 5.

**Sample Input:**
```
15
```
**Sample Output:**
```
5 3
```

---

*End of Batch 3 — 20 core-mechanics problems. Every output is a computed value. All reference solutions verified against the sample and extra cases.*
