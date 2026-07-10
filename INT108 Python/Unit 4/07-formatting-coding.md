# Topic 07 — Formatting · Coding

*Unit 4 · Strings. Six judge-format problems on f-strings, two-decimal formatting, and `ord`/`chr`. Read input with `input()`, produce exact-match output. Each shows a verified reference solution. Note: money and averages use `f"{value:.2f}"` — `round()` would drop trailing zeros and fail the judge. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Format a Price  [E]

A price is given in paise. Print it in rupees with exactly two decimal places (100 paise = 1 rupee).

**Input Format:** A single line — an integer `p`, the price in paise.
**Output Format:** The price in rupees, to 2 decimals.

**Sample Input:**
```
1550
```
**Sample Output:**
```
15.50
```

**Solution:**
```python
p = int(input())
print(f'{p / 100:.2f}')
```
`:.2f` keeps both decimals, so 15.5 prints as `15.50`. Using `round(p/100, 2)` would print `15.5` and fail.

---

## 2 — Build a Greeting  [E]

Read a name and an age, and print a sentence using them.

**Input Format:** Two lines — the name, then an integer age.
**Output Format:** `NAME is AGE years old`.

**Sample Input:**
```
Ravi
25
```
**Sample Output:**
```
Ravi is 25 years old
```

**Solution:**
```python
name = input()
age = int(input())
print(f'{name} is {age} years old')
```
An f-string slots both values straight into the sentence.

---

## 3 — Character Code  [M]

Print the ASCII code of the first character of a string.

**Input Format:** A single line — a non-empty string `s`.
**Output Format:** A single integer — the code of the first character.

**Sample Input:**
```
Apple
```
**Sample Output:**
```
65
```

**Solution:**
```python
s = input()
print(ord(s[0]))
```
`ord` gives the numeric code of a character; `A` is 65.

---

## 4 — Code to Character  [M]

Print the character that has the given ASCII code.

**Input Format:** A single line — an integer `n` (32 ≤ n ≤ 126).
**Output Format:** The single character with that code.

**Sample Input:**
```
72
```
**Sample Output:**
```
H
```

**Solution:**
```python
n = int(input())
print(chr(n))
```
`chr` is the inverse of `ord`: code 72 is `H`.

---

## 5 — Average to Two Decimals  [M]

Read three integers and print their average with exactly two decimal places.

**Input Format:** Three lines — three integers.
**Output Format:** The average, to 2 decimals.

**Sample Input:**
```
10
20
30
```
**Sample Output:**
```
20.00
```

**Solution:**
```python
a = int(input())
b = int(input())
c = int(input())
print(f'{(a + b + c) / 3:.2f}')
```
The average of 10, 20, 30 is 20.0, shown as `20.00` — the two decimals matter for exact matching.

---

## 6 — Shift a Character  [H]

Read a lowercase letter and a shift amount `n`, and print the letter that comes `n` places later in the alphabet (assume the result stays within the letters, no wrap-around needed).

**Input Format:** Two lines — a single lowercase letter, then an integer `n`.
**Output Format:** The shifted letter.

**Sample Input:**
```
a
3
```
**Sample Output:**
```
d
```

**Solution:**
```python
c = input()
n = int(input())
print(chr(ord(c) + n))
```
Convert the letter to its code with `ord`, add the shift, and convert back with `chr`. This is the core idea behind a Caesar cipher.

---

*End of Topic 07 coding — 6 problems. Every reference solution verified by execution.*
