# Parameters & Arguments — Coding Problems (1–5)

*Unit 3 · Topic 04. Platform-judge format: exact-match output. These problems pass values **into** functions through parameters; the function **prints** its result inside the body (handing values back with `return` is the next topic). Each names a **Required function** you must define with the exact name and parameters given, then call.*

---

## Problem 1 — Rectangle Area

**Task:** Read a length and a width and print the area of the rectangle.

**Required function:** Define `rectangle_area(length, width)` that computes the area and **prints** it. Read the two values and call the function.

**Input Format:** Two integers, each on its own line — `length` then `width` (1 ≤ each ≤ 10000).

**Output Format:** A single integer — the area.

**Sample Input:**
```
5
3
```
**Sample Output:**
```
15
```

---

## Problem 2 — Larger of Two

**Task:** Read two integers and print the larger one — without using the built-in `max()`.

**Required function:** Define `max_of_two(a, b)` that compares its two parameters with an `if` and **prints** the larger. Call it with the two values read from input.

**Input Format:** Two integers, each on its own line (−10000 ≤ each ≤ 10000).

**Output Format:** A single integer — the larger value. (If they are equal, print that value.)

**Sample Input:**
```
8
3
```
**Sample Output:**
```
8
```

---

## Problem 3 — Power With a Default

**Task:** Read a base and an exponent and print `base` raised to `exp`, computed with a loop (do **not** use `**` or `math.pow`).

**Required function:** Define `power(base, exp=2)` — note the **default** exponent of 2 — that multiplies `base` by itself `exp` times and **prints** the result. Read both values and call `power(base, exp)`.

**Input Format:** Two integers, each on its own line — `base` then `exp` (1 ≤ base ≤ 100, 0 ≤ exp ≤ 10).

**Output Format:** A single integer — `base` raised to the power `exp`. (Any number to the power 0 is 1.)

**Sample Input:**
```
2
5
```
**Sample Output:**
```
32
```

---

## Problem 4 — Describe a Person

**Task:** Read a name and an age, then print a sentence describing the person, in the exact form `NAME is AGE years old`.

**Required function:** Define `describe(name, age)` that takes two parameters and **prints** the sentence. Read the name (a word) and the age (an integer), then call the function with both — notice the two arguments fill the two parameters **in order**.

**Input Format:** A name on the first line (a single word), then an integer `age` on the second line (1 ≤ age ≤ 120).

**Output Format:** One line in the form `NAME is AGE years old`.

**Sample Input:**
```
Sam
12
```
**Sample Output:**
```
Sam is 12 years old
```

---

## Problem 5 — Discounted Bill

**Task:** A purchase has a quantity, a unit price, and a discount percentage. Read all three and print the final amount after the discount.

**Required function:** Define `bill(qty, price, discount)` — three parameters — that computes quantity × price, reduces it by `discount` percent using `total - total * discount // 100`, and **prints** the result. Call it with the three values read from input.

**Input Format:** Three integers, each on its own line — `qty`, `price`, then `discount` (1 ≤ qty ≤ 1000, 1 ≤ price ≤ 100000, 0 ≤ discount ≤ 100).

**Output Format:** A single integer — the final amount after discount.

**Sample Input:**
```
5
100
10
```
**Sample Output:**
```
450
```

---

*End — 5 problems. Every reference solution verified against the sample and additional hidden cases. No `return` is used — functions print their results, keeping to Topic 04's scope.*
