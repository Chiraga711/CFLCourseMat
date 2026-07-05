# Math Module — Coding Problems (1–5)

*Unit 3 · Topic 07. Platform-judge format: exact-match output. Every program must `import math` and use its functions. Remember: `math.sqrt` and `math.pow` return **floats**, while `math.ceil` and `math.floor` return **ints**. Where a problem names a **Required function**, define it with the exact name and parameters given.*

---

## Problem 1 — Hypotenuse

**Task:** A right triangle has two perpendicular sides `a` and `b`. Print the length of the hypotenuse, √(a² + b²), to exactly 2 decimal places.

**Required function:** Define `hypotenuse(a, b)` that **returns** `math.sqrt(a * a + b * b)`. Read the two sides, call it, and print the result formatted with `f"{value:.2f}"`.

**Input Format:** Two integers, each on its own line — `a` then `b` (1 ≤ each ≤ 10000).

**Output Format:** The hypotenuse length, to exactly 2 decimal places.

**Sample Input:**
```
3
4
```
**Sample Output:**
```
5.00
```

---

## Problem 2 — Boxes Needed

**Task:** You have `items` objects and each box holds `cap` of them. Print the number of boxes needed so that every item fits (a partly filled box still counts as one).

**Required function:** Define `boxes_needed(items, cap)` that **returns** `math.ceil(items / cap)`. Read the two values, call it, and print the result. (Ceiling division is the natural tool: any leftover items force one more box.)

**Input Format:** Two integers, each on its own line — `items` then `cap` (1 ≤ items ≤ 1000000, 1 ≤ cap ≤ 1000).

**Output Format:** A single integer — the number of boxes.

**Sample Input:**
```
17
5
```
**Sample Output:**
```
4
```

---

## Problem 3 — Power as a Whole Number

**Task:** Read a base and an exponent and print `base` raised to `exp`, using `math.pow`. Because `math.pow` returns a float, convert the result to an integer before printing.

**Required function:** Define `int_power(base, exp)` that **returns** `int(math.pow(base, exp))`. Read both values, call it, and print the result.

**Input Format:** Two integers, each on its own line — `base` then `exp` (1 ≤ base ≤ 100, 0 ≤ exp ≤ 9).

**Output Format:** A single integer — `base` raised to the power `exp`.

**Sample Input:**
```
3
4
```
**Sample Output:**
```
81
```

---

## Problem 4 — Perfect Square Check

**Task:** Read an integer and print `Yes` if it is a perfect square (like 1, 4, 9, 16, 25…), otherwise `No`.

**Required function:** Define `is_perfect_square(n)` that takes the square root with `math.sqrt`, rounds it down with `math.floor`, and **returns** `True` if that whole number squared equals `n`. Use the returned value to print `Yes` or `No`.

**Input Format:** A single integer `n` (1 ≤ n ≤ 1000000).

**Output Format:** Either `Yes` or `No`.

**Sample Input:**
```
49
```
**Sample Output:**
```
Yes
```

---

## Problem 5 — Floor and Ceiling Together

**Task:** Read two integers `a` and `b` and print the floor and the ceiling of `a ÷ b`, separated by a space — showing how the two functions round the same division in opposite directions.

**Required function:** Define `floor_and_ceil(a, b)` that **returns two values**: `math.floor(a / b)` and `math.ceil(a / b)`. Unpack them and print both, separated by a space.

**Input Format:** Two integers, each on its own line — `a` then `b` (1 ≤ a ≤ 1000000, 1 ≤ b ≤ 1000).

**Output Format:** Two integers separated by a space: the floor, then the ceiling.

**Sample Input:**
```
23
4
```
**Sample Output:**
```
5 6
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases.*
