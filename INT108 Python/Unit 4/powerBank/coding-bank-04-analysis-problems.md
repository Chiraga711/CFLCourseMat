# Strings Coding Bank — Batch 4: Text Analysis & Validation (61–80)

*Measuring, scoring, and checking text — every result a computed value.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-04-analysis-solutions.md`.*

---

## 61 — Password Strength 4  [M]

Score a password 0–4: one point each for containing an uppercase letter, a lowercase letter, a digit, and any other character (symbol/space). Print the score.

**Input Format:** One line — the password.
**Output Format:** An integer 0–4.

**Sample Input:**
```
Ab1!
```
**Sample Output:**
```
4
```
---

## 62 — Palindrome Distance  [M]

Print how many mirror pairs of a string **disagree** (0 means it is a palindrome).

**Input Format:** One line — a string.
**Output Format:** The number of mismatched pairs.

**Sample Input:**
```
level
```
**Sample Output:**
```
0
```
---

## 63 — Anagram Distance  [H]

For two lowercase words, print the total of absolute differences in each letter's count (0 means they are anagrams).

**Input Format:** Two lines — two lowercase words.
**Output Format:** The summed letter-count difference.

**Sample Input:**
```
listen
silent
```
**Sample Output:**
```
0
```
---

## 64 — Vowels and Consonants  [M]

Print two numbers separated by a space: the vowel count and the consonant count (letters only; ignore other characters). Treat input as lowercase.

**Input Format:** One line — a lowercase string.
**Output Format:** `vowels consonants`.

**Sample Input:**
```
stream
```
**Sample Output:**
```
2 4
```
---

## 65 — Average Word Length  [M]

Print the average word length of a sentence, to two decimals.

**Input Format:** One line — a sentence.
**Output Format:** The average to 2 decimals.

**Sample Input:**
```
the quick brown fox
```
**Sample Output:**
```
4.00
```
---

## 66 — Longest and Shortest  [M]

Print the lengths of the longest and shortest words, separated by a space.

**Input Format:** One line — a sentence.
**Output Format:** `longest shortest` lengths.

**Sample Input:**
```
we all win big
```
**Sample Output:**
```
3 2
```
---

## 67 — Unique Characters  [M]

Print how many **different** characters the string uses.

**Input Format:** One line — a string.
**Output Format:** The count of distinct characters.

**Sample Input:**
```
banana
```
**Sample Output:**
```
3
```
---

## 68 — Most Frequent Character  [H]

Print the most frequent character and its count, separated by a space (on ties, the one that appears **first** in the string).

**Input Format:** One line — a non-empty string.
**Output Format:** `char count`.

**Sample Input:**
```
banana
```
**Sample Output:**
```
a 3
```
---

## 69 — Character Classes  [M]

Print three numbers separated by spaces: how many characters are digits, letters, and anything else.

**Input Format:** One line — a string.
**Output Format:** `digits letters others`.

**Sample Input:**
```
a1 b2!
```
**Sample Output:**
```
2 2 2
```
---

## 70 — Capitalised Words  [M]

Print how many words start with an uppercase letter.

**Input Format:** One line — a sentence.
**Output Format:** The count.

**Sample Input:**
```
The Quick brown Fox
```
**Sample Output:**
```
3
```
---

## 71 — Sentence-Case Violations  [H]

In proper sentence case only the **first** word starts uppercase. Print how many words violate this (first word lowercase counts as one violation; any later word starting uppercase counts as one each).

**Input Format:** One line — a sentence.
**Output Format:** The violation count.

**Sample Input:**
```
The cat Sat down
```
**Sample Output:**
```
1
```
---

## 72 — Diversity Ratio  [H]

Print the ratio of distinct characters to total characters, to two decimals.

**Input Format:** One line — a non-empty string.
**Output Format:** `distinct / total` to 2 decimals.

**Sample Input:**
```
aabb
```
**Sample Output:**
```
0.50
```
---

## 73 — Repeated Words  [M]

Print how many words appear more than once in a sentence (each such word counted once).

**Input Format:** One line — a sentence.
**Output Format:** The number of distinct repeated words.

**Sample Input:**
```
the cat and the dog and
```
**Sample Output:**
```
2
```
---

## 74 — Acronym Match  [M]

Given a phrase and an acronym, print how many of the acronym's letters match the phrase's word-initials in order (position by position).

**Input Format:** Two lines — the phrase, then the acronym (same length as the word count).
**Output Format:** The number of matching positions.

**Sample Input:**
```
central processing unit
CPU
```
**Sample Output:**
```
3
```
---

## 75 — Quote Balance  [E]

Print the remainder when the number of `"` characters in a line is divided by 2 (0 means the quotes pair up).

**Input Format:** One line — text that may contain `"` characters.
**Output Format:** `0` or `1`.

**Sample Input:**
```
say "hi" now
```
**Sample Output:**
```
0
```
---

## 76 — Position Similarity  [H]

For two equal-length strings, print how many positions hold the same character.

**Input Format:** Two lines — two equal-length strings.
**Output Format:** The matching-position count.

**Sample Input:**
```
paste
taste
```
**Sample Output:**
```
4
```
---

## 77 — Rarest Vowel Present  [M]

Among the vowels that actually occur in the string, print the count of the least frequent one.

**Input Format:** One line — a lowercase string containing at least one vowel.
**Output Format:** The smallest nonzero vowel count.

**Sample Input:**
```
education
```
**Sample Output:**
```
1
```
---

## 78 — Space Runs  [M]

Print how many separate runs of one-or-more spaces the line contains.

**Input Format:** One line — text.
**Output Format:** The number of space runs.

**Sample Input:**
```
a  b c
```
**Sample Output:**
```
2
```
---

## 79 — Initial Letter Frequency  [M]

Print how many words begin with a given letter, ignoring case.

**Input Format:** Two lines — the sentence, then a single letter.
**Output Format:** The count.

**Sample Input:**
```
Big brown Bear ran
b
```
**Sample Output:**
```
3
```
---

## 80 — Readability Score  [H]

Print `words + average-word-length` as one number to two decimals (a toy readability measure).

**Input Format:** One line — a sentence.
**Output Format:** The combined score to 2 decimals.

**Sample Input:**
```
the quick brown fox
```
**Sample Output:**
```
8.00
```
---

*End of Batch 4 — 20 problems. Difficulty: 1 [E] · 13 [M] · 6 [H]. All reference solutions verified by execution.*