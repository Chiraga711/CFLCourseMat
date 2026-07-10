# Strings Coding Bank — Batch 7: Number-String Hybrids & Formatting (121–140)

*Digits living inside text: extraction, clock times, percentages, and precise 2-decimal output.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-07-hybrid-solutions.md`.*

---

## 121 — Extract the Number  [H]

A string contains letters and exactly one contiguous group of digits. Print that number as an integer (leading zeros disappear).

**Input Format:** One line — the mixed string.
**Output Format:** The number as an integer.

**Sample Input:**
```
ab007cd
```
**Sample Output:**
```
7
```
---

## 122 — Paise by Slicing  [M]

A price is a digit string in paise (at least 3 digits). Print it in rupees by **slicing only** — insert a dot before the last two digits. No arithmetic allowed.

**Input Format:** One line — the digit string.
**Output Format:** The rupee form.

**Sample Input:**
```
4075
```
**Sample Output:**
```
40.75
```
---

## 123 — Minutes Since Midnight  [M]

Read a 24-hour time `HH:MM` and print how many minutes have passed since 00:00.

**Input Format:** One line — the time.
**Output Format:** The minute count.

**Sample Input:**
```
14:30
```
**Sample Output:**
```
870
```
---

## 124 — Time Difference  [H]

Read two times `HH:MM` on the same day (the second is later). Print the minutes between them.

**Input Format:** Two lines — the earlier time, then the later time.
**Output Format:** The difference in minutes.

**Sample Input:**
```
09:15
11:05
```
**Sample Output:**
```
110
```
---

## 125 — Vowel Percentage  [M]

Print what percentage of a string's characters are vowels, to two decimals.

**Input Format:** One line — a lowercase string.
**Output Format:** The percentage to 2 decimals.

**Sample Input:**
```
audio
```
**Sample Output:**
```
80.00
```
---

## 126 — Score Percent  [M]

A score is written `got/total`, like `45/60`. Print it as a percentage to two decimals.

**Input Format:** One line — the score string.
**Output Format:** The percentage to 2 decimals.

**Sample Input:**
```
45/60
```
**Sample Output:**
```
75.00
```
---

## 127 — Dash Every K  [H]

Insert a `-` after every `k` characters (never at the very start or end).

**Input Format:** Two lines — the string, then `k`.
**Output Format:** The dashed string.

**Sample Input:**
```
abcdef
2
```
**Sample Output:**
```
ab-cd-ef
```
---

## 128 — Zero-Pad Left  [E]

Pad a digit string with `0`s on the left to reach width `w` (build the padding yourself).

**Input Format:** Two lines — the digit string, then `w` (w ≥ its length).
**Output Format:** The padded string.

**Sample Input:**
```
42
5
```
**Sample Output:**
```
00042
```
---

## 129 — Grand Total  [E]

Read three item prices in paise and print the bill total in rupees, to two decimals.

**Input Format:** Three lines — three integers (paise).
**Output Format:** The total to 2 decimals.

**Sample Input:**
```
100
250
75
```
**Sample Output:**
```
4.25
```
---

## 130 — Largest Digit  [M]

Print the largest digit character appearing in a string (at least one digit is present).

**Input Format:** One line — the string.
**Output Format:** The largest digit.

**Sample Input:**
```
a3x9b1
```
**Sample Output:**
```
9
```
---

## 131 — Odd vs Even Digits  [M]

Print two numbers separated by a space: how many digits in the string are odd, and how many are even.

**Input Format:** One line — the string.
**Output Format:** `odd even` counts.

**Sample Input:**
```
a1b2c3
```
**Sample Output:**
```
2 1
```
---

## 132 — Weighted Checksum  [H]

Print the sum of each digit multiplied by its 1-based **position in the string** (non-digits contribute nothing but still occupy positions).

**Input Format:** One line — the string.
**Output Format:** The weighted sum.

**Sample Input:**
```
1a2
```
**Sample Output:**
```
7
```
---

## 133 — Uppercase Percentage  [M]

Print what percentage of the string's characters are uppercase letters, to two decimals.

**Input Format:** One line — the string.
**Output Format:** The percentage to 2 decimals.

**Sample Input:**
```
AbCd
```
**Sample Output:**
```
50.00
```
---

## 134 — Time Violations  [H]

A 5-character time string should satisfy three rules: the middle character is `:`; the first two characters are digits forming a number below 24; the last two are digits forming a number below 60. Print how many rules are broken (0–3).

**Input Format:** One line — a 5-character string.
**Output Format:** The violation count.

**Sample Input:**
```
25:70
```
**Sample Output:**
```
2
```
---

## 135 — Evaluate a Sum  [M]

A string holds a single addition like `12+30`. Print the result.

**Input Format:** One line — `a+b` with two non-negative integers.
**Output Format:** The sum.

**Sample Input:**
```
12+30
```
**Sample Output:**
```
42
```
---

## 136 — Max of a CSV  [M]

Print the largest of the comma-separated non-negative integers (via a loop, not `max`).

**Input Format:** One line — integers separated by commas.
**Output Format:** The largest value.

**Sample Input:**
```
4,17,9
```
**Sample Output:**
```
17
```
---

## 137 — Discount Line  [H]

A bill line reads `price qty discount` (integers, discount is a percent). Print the final amount: price × qty reduced by the discount, to two decimals.

**Input Format:** One line — three space-separated integers.
**Output Format:** The final amount to 2 decimals.

**Sample Input:**
```
50 3 10
```
**Sample Output:**
```
135.00
```
---

## 138 — Decimal Places  [E]

Print how many digits a decimal number string has after its dot.

**Input Format:** One line — a number string containing one `.`.
**Output Format:** The count of decimal places.

**Sample Input:**
```
3.1415
```
**Sample Output:**
```
4
```
---

## 139 — Average Character Code  [M]

Print the average of the character codes of a string, to two decimals.

**Input Format:** One line — a non-empty string.
**Output Format:** The average code to 2 decimals.

**Sample Input:**
```
ab
```
**Sample Output:**
```
97.50
```
---

## 140 — Digits Minus Letters  [M]

Print (the sum of the digit characters) minus (the count of letters). The answer may be negative.

**Input Format:** One line — the string.
**Output Format:** The difference.

**Sample Input:**
```
a5b3
```
**Sample Output:**
```
6
```
---

*End of Batch 7 — 20 problems. Difficulty: 3 [E] · 11 [M] · 6 [H]. All reference solutions verified by execution.*