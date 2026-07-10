# Strings Coding Bank — Batch 3: Core Mechanics (41–60)

*Slicing precision, method pipelines, index arithmetic, and comparisons.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-03-core-solutions.md`.*

---

## 41 — Kth From the End  [M]

Print the `k`-th character from the end **without** using a negative index (use `len` arithmetic).

**Input Format:** Two lines — the string, then `k` (1 ≤ k ≤ len).
**Output Format:** The character.

**Sample Input:**
```
python
2
```
**Sample Output:**
```
o
```
---

## 42 — Middle Two  [M]

Print the middle two characters of an even-length string.

**Input Format:** One line — an even-length string.
**Output Format:** The two centre characters.

**Sample Input:**
```
abcdef
```
**Sample Output:**
```
cd
```
---

## 43 — Every Third  [E]

Print every third character, starting from the first.

**Input Format:** One line — a string.
**Output Format:** Characters at positions 0, 3, 6, …

**Sample Input:**
```
abcdefghij
```
**Sample Output:**
```
adgj
```
---

## 44 — Window Slice  [M]

Read a string and two indices `a` and `b`; print the slice from `a` up to (not including) `b`.

**Input Format:** Three lines — the string, `a`, then `b` (0 ≤ a ≤ b ≤ len).
**Output Format:** The slice `s[a:b]`.

**Sample Input:**
```
keyboard
2
5
```
**Sample Output:**
```
ybo
```
---

## 45 — Half Difference  [M]

Print the length difference between the first half and second half of a string (first half gets the extra character when the length is odd).

**Input Format:** One line — a string.
**Output Format:** first-half length − second-half length (0 or 1).

**Sample Input:**
```
abcde
```
**Sample Output:**
```
1
```
---

## 46 — Overlapping Count  [H]

Count occurrences of a 2-character pattern **allowing overlaps** (which `count` does not).

**Input Format:** Two lines — the string, then a 2-character pattern.
**Output Format:** The overlapping count.

**Sample Input:**
```
aaaa
aa
```
**Sample Output:**
```
3
```
---

## 47 — Second Occurrence  [M]

Print the index of the **second** occurrence of a character (it always appears at least twice).

**Input Format:** Two lines — the string, then a single character.
**Output Format:** The index of the second occurrence.

**Sample Input:**
```
banana
a
```
**Sample Output:**
```
3
```
---

## 48 — Clean Pipeline  [M]

Strip the string, title-case it, then replace spaces with underscores. Print the result.

**Input Format:** One line — messy text.
**Output Format:** The pipelined string.

**Sample Input:**
```
  data science  
```
**Sample Output:**
```
Data_Science
```
---

## 49 — Longest Run  [H]

Print the length of the longest run of the same character.

**Input Format:** One line — a string.
**Output Format:** The longest run length.

**Sample Input:**
```
aabbbcc
```
**Sample Output:**
```
3
```
---

## 50 — Two Middles  [M]

For a string of length `n`, print the characters at `n // 2` and `(n - 1) // 2`, separated by a space (they're the same character when `n` is odd).

**Input Format:** One line — a string (length ≥ 1).
**Output Format:** Two characters separated by a space.

**Sample Input:**
```
abcd
```
**Sample Output:**
```
c b
```
---

## 51 — Re-Delimit  [E]

Change a comma-separated record into a semicolon-separated one.

**Input Format:** One line — a comma-separated record.
**Output Format:** The record with `;` instead of `,`.

**Sample Input:**
```
a,b,c
```
**Sample Output:**
```
a;b;c
```
---

## 52 — Last Word Length  [E]

Print the length of the last word of a sentence.

**Input Format:** One line — a sentence.
**Output Format:** The last word's length.

**Sample Input:**
```
we are here
```
**Sample Output:**
```
4
```
---

## 53 — Words of Length K  [M]

Print how many words have exactly `k` characters.

**Input Format:** Two lines — the sentence, then `k`.
**Output Format:** The count.

**Sample Input:**
```
the cat ran far
3
```
**Sample Output:**
```
4
```
---

## 54 — Letters vs Length  [M]

Print two numbers separated by a space: the total length of the string, and the length excluding spaces.

**Input Format:** One line — a sentence.
**Output Format:** `total non-space` counts.

**Sample Input:**
```
a b c
```
**Sample Output:**
```
5 3
```
---

## 55 — Alphabetically First Word  [H]

Print the word that comes first alphabetically (the first such word if repeated), using `<` comparisons in a loop.

**Input Format:** One line — a sentence of lowercase words.
**Output Format:** The alphabetically smallest word.

**Sample Input:**
```
banana apple cherry
```
**Sample Output:**
```
apple
```
---

## 56 — Alphabetically Last Word  [H]

Print the word that comes last alphabetically (first such word on ties).

**Input Format:** One line — a sentence of lowercase words.
**Output Format:** The alphabetically largest word.

**Sample Input:**
```
banana apple cherry
```
**Sample Output:**
```
cherry
```
---

## 57 — Alternate First Letters  [M]

Print the first letters of the 1st, 3rd, 5th… words joined together.

**Input Format:** One line — a sentence.
**Output Format:** The collected letters.

**Sample Input:**
```
sun and moon and star
```
**Sample Output:**
```
sms
```
---

## 58 — A-to-A Distance  [H]

Print the index distance between the first and last occurrence of a given character (0 if it appears once).

**Input Format:** Two lines — the string, then the character (present at least once).
**Output Format:** last index − first index.

**Sample Input:**
```
banana
a
```
**Sample Output:**
```
4
```
---

## 59 — Reverse First Half  [H]

Reverse only the first half of the string (extra middle character of odd lengths stays with the second half). Print the result.

**Input Format:** One line — a string.
**Output Format:** The half-reversed string.

**Sample Input:**
```
abcdef
```
**Sample Output:**
```
cbadef
```
---

## 60 — Fit to Width  [M]

Print the string cut to exactly width `w`: truncate if longer, pad with `.` on the right if shorter.

**Input Format:** Two lines — the string, then `w`.
**Output Format:** A string of exactly `w` characters.

**Sample Input:**
```
hello
3
```
**Sample Output:**
```
hel
```
---

*End of Batch 3 — 20 problems. Difficulty: 3 [E] · 11 [M] · 6 [H]. All reference solutions verified by execution.*