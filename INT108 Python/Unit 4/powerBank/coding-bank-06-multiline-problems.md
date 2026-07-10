# Strings Coding Bank — Batch 6: Multi-Line Input (101–120)

*The judge-realistic pattern: first line n, then n lines — processed as a stream with counters and trackers, never stored.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-06-multiline-solutions.md`.*

---

## 101 — Longest of N Words  [M]

Read `n` words, one per line, and print the longest (the first one if there is a tie).

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The longest word.

**Sample Input:**
```
3
cat
mouse
dog
```
**Sample Output:**
```
mouse
```
---

## 102 — Total Characters  [E]

Read `n` lines and print the total number of characters across all of them.

**Input Format:** First line — `n`. Then `n` lines.
**Output Format:** The combined length.

**Sample Input:**
```
2
hi
there
```
**Sample Output:**
```
7
```
---

## 103 — Acronym From Lines  [E]

Read `n` words and print the acronym: each word's first letter, uppercased, joined together.

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The acronym.

**Sample Input:**
```
3
red
green
blue
```
**Sample Output:**
```
RGB
```
---

## 104 — Vowel-Start Words  [M]

Read `n` words and print how many begin with a vowel (ignore case).

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The count.

**Sample Input:**
```
4
apple
sky
egg
ice
```
**Sample Output:**
```
3
```
---

## 105 — Average Word Length  [M]

Read `n` words and print their average length, to two decimals.

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The average to 2 decimals.

**Sample Input:**
```
2
hi
there
```
**Sample Output:**
```
3.50
```
---

## 106 — All-Digit Lines  [M]

Read `n` lines and print how many consist only of digits.

**Input Format:** First line — `n`. Then `n` lines.
**Output Format:** The count.

**Sample Input:**
```
3
123
a1
77
```
**Sample Output:**
```
2
```
---

## 107 — Join With Dashes  [E]

Read `n` words and print them joined by `-` in the order given.

**Input Format:** First line — `n` (n ≥ 1). Then `n` lines, one word each.
**Output Format:** The dashed string.

**Sample Input:**
```
3
a
b
c
```
**Sample Output:**
```
a-b-c
```
---

## 108 — The Kth Line  [M]

Read `n` and `k`, then `n` lines; print the `k`-th line (counting from 1).

**Input Format:** First line — `n`. Second line — `k`. Then `n` lines.
**Output Format:** The `k`-th line.

**Sample Input:**
```
3
2
alpha
beta
gamma
```
**Sample Output:**
```
beta
```
---

## 109 — Lines Longer Than L  [M]

Read `n` and a limit `L`, then `n` lines; print how many lines are **longer** than `L` characters.

**Input Format:** First line — `n`. Second line — `L`. Then `n` lines.
**Output Format:** The count.

**Sample Input:**
```
3
2
hi
hello
hey
```
**Sample Output:**
```
2
```
---

## 110 — Vote Counter  [M]

An election reads the candidate's name first, then `n` votes (one name per line). Print how many votes the candidate received.

**Input Format:** First line — `n`. Second line — the candidate. Then `n` lines of votes.
**Output Format:** The candidate's vote count.

**Sample Input:**
```
4
ravi
ravi
meena
ravi
meena
```
**Sample Output:**
```
2
```
---

## 111 — Palindromic Words  [H]

Read `n` words and print how many read the same forwards and backwards.

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The palindrome count.

**Sample Input:**
```
4
noon
cat
anna
dog
```
**Sample Output:**
```
2
```
---

## 112 — Adjacent Duplicates  [H]

Read `n` lines and print how many lines are identical to the line **immediately before** them.

**Input Format:** First line — `n` (n ≥ 1). Then `n` lines.
**Output Format:** The count of adjacent repeats.

**Sample Input:**
```
4
a
a
b
b
```
**Sample Output:**
```
2
```
---

## 113 — Alphabetically First  [M]

Read `n` words and print the one that comes first in dictionary order (first on ties).

**Input Format:** First line — `n`. Then `n` lines of lowercase words.
**Output Format:** The alphabetically smallest word.

**Sample Input:**
```
3
pear
apple
plum
```
**Sample Output:**
```
apple
```
---

## 114 — Total Vowels  [M]

Read `n` lines and print the total number of vowels across all of them (lowercase input).

**Input Format:** First line — `n`. Then `n` lines.
**Output Format:** The vowel total.

**Sample Input:**
```
2
hello
sky
```
**Sample Output:**
```
2
```
---

## 115 — Distinct First Letters  [H]

Read `n` words and print how many **different** first letters appear among them.

**Input Format:** First line — `n`. Then `n` lines, one word each.
**Output Format:** The count of distinct initials.

**Sample Input:**
```
4
cat
cow
dog
duck
```
**Sample Output:**
```
2
```
---

## 116 — Digit-Sum Total  [M]

Read `n` lines and print the sum of every digit character across all of them.

**Input Format:** First line — `n`. Then `n` lines.
**Output Format:** The total of all digits.

**Sample Input:**
```
2
a1b2
34
```
**Sample Output:**
```
10
```
---

## 117 — Find the Line  [M]

Read a target word, then `n` lines. Print the line number (from 1) of the **first** line equal to the target (it is guaranteed to appear).

**Input Format:** First line — `n`. Second line — the target. Then `n` lines.
**Output Format:** The 1-based line number of the first match.

**Sample Input:**
```
3
go
stop
go
go
```
**Sample Output:**
```
2
```
---

## 118 — Longest and Shortest  [M]

Read `n` words and print two numbers separated by a space: the longest length and the shortest length.

**Input Format:** First line — `n` (n ≥ 1). Then `n` lines, one word each.
**Output Format:** `longest shortest`.

**Sample Input:**
```
3
hi
hello
hey
```
**Sample Output:**
```
5 2
```
---

## 119 — Uppercase Starters  [E]

Read `n` lines and print how many begin with an uppercase letter.

**Input Format:** First line — `n`. Then `n` lines.
**Output Format:** The count.

**Sample Input:**
```
3
Cat
dog
Bird
```
**Sample Output:**
```
2
```
---

## 120 — Stream Checksum  [H]

Read a modulus `m`, then `n` lines. Print the sum of the character codes of **every** character across all lines, mod `m`.

**Input Format:** First line — `n`. Second line — `m`. Then `n` lines.
**Output Format:** The checksum.

**Sample Input:**
```
2
100
ab
c
```
**Sample Output:**
```
94
```
---

*End of Batch 6 — 20 problems. Difficulty: 4 [E] · 12 [M] · 4 [H]. All reference solutions verified by execution.*