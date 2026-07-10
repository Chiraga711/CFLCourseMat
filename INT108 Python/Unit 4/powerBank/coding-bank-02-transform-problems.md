# Strings Coding Bank — Batch 2: Transform & Cipher (21–40)

*String-to-string mappings: ciphers, encodings, rotations, and character transforms.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-02-transform-solutions.md`.*

---

## 21 — Caesar Shift (with wrap)  [H]

Encode a lowercase word by shifting each letter forward `k` places, wrapping from `z` back to `a`.

**Input Format:** Two lines — the word (lowercase letters only), then the shift `k` (0 ≤ k ≤ 25).
**Output Format:** The encoded word.

**Sample Input:**
```
zap
1
```
**Sample Output:**
```
abq
```
---

## 22 — Caesar Decode  [H]

Decode a lowercase word that was shifted forward by `k` (wrap included).

**Input Format:** Two lines — the encoded word, then `k`.
**Output Format:** The original word.

**Sample Input:**
```
khoor
3
```
**Sample Output:**
```
hello
```
---

## 23 — Alphabet Position Sum  [M]

Print the sum of alphabet positions of a lowercase word (`a`=1 … `z`=26).

**Input Format:** One line — a lowercase word.
**Output Format:** The sum.

**Sample Input:**
```
abc
```
**Sample Output:**
```
6
```
---

## 24 — Swap Halves  [M]

Swap the two halves of an even-length string.

**Input Format:** One line — an even-length string.
**Output Format:** The string with halves swapped.

**Sample Input:**
```
abcd
```
**Sample Output:**
```
cdab
```
---

## 25 — Remove Duplicate Characters  [H]

Keep only the first occurrence of each character, preserving order.

**Input Format:** One line — a string.
**Output Format:** The string with later repeats removed.

**Sample Input:**
```
banana
```
**Sample Output:**
```
ban
```
---

## 26 — Run-Length Encode  [H]

Compress runs of repeated characters as `char + count` (count even when 1).

**Input Format:** One line — a string.
**Output Format:** The encoded form.

**Sample Input:**
```
aaabb
```
**Sample Output:**
```
a3b2
```
---

## 27 — Run-Length Decode  [H]

Expand `char digit` pairs back into the full string (counts are single digits 1–9).

**Input Format:** One line — an encoded string like `a3b2`.
**Output Format:** The expanded string.

**Sample Input:**
```
a3b2
```
**Sample Output:**
```
aaabb
```
---

## 28 — Duplicate the Vowels  [M]

Print the string with every vowel doubled.

**Input Format:** One line — a lowercase string.
**Output Format:** The transformed string.

**Sample Input:**
```
beam
```
**Sample Output:**
```
beeaam
```
---

## 29 — Interleave Two Strings  [M]

Merge two equal-length strings by alternating characters, starting with the first.

**Input Format:** Two lines — two equal-length strings.
**Output Format:** The interleaved string.

**Sample Input:**
```
ab
xy
```
**Sample Output:**
```
axby
```
---

## 30 — Mirror Append  [E]

Print the string followed by its reverse.

**Input Format:** One line — a string.
**Output Format:** `s` + reversed `s`.

**Sample Input:**
```
abc
```
**Sample Output:**
```
abccba
```
---

## 31 — Digit Shift  [H]

In a mixed string, replace each digit with the next one (`9` wraps to `0`); leave other characters alone.

**Input Format:** One line — a string.
**Output Format:** The transformed string.

**Sample Input:**
```
a9b1
```
**Sample Output:**
```
a0b2
```
---

## 32 — Reverse-Alphabet Map  [H]

Map each lowercase letter to its mirror (`a`↔`z`, `b`↔`y`, …) and print the result.

**Input Format:** One line — a lowercase word.
**Output Format:** The mapped word.

**Sample Input:**
```
abc
```
**Sample Output:**
```
zyx
```
---

## 33 — Collapse Spaces  [M]

Reduce every run of spaces inside a line to a single space (also trimming the ends).

**Input Format:** One line — text with messy spacing.
**Output Format:** The cleaned line.

**Sample Input:**
```
a   b  c
```
**Sample Output:**
```
a b c
```
---

## 34 — Rotate Left  [M]

Rotate a string left by `k` positions (characters wrap to the end).

**Input Format:** Two lines — the string, then `k` (0 ≤ k ≤ len).
**Output Format:** The rotated string.

**Sample Input:**
```
abcdef
2
```
**Sample Output:**
```
cdefab
```
---

## 35 — Rotate Right  [M]

Rotate a string right by `k` positions.

**Input Format:** Two lines — the string, then `k` (0 ≤ k ≤ len).
**Output Format:** The rotated string.

**Sample Input:**
```
abcdef
2
```
**Sample Output:**
```
efabcd
```
---

## 36 — Toggle Case Manually  [H]

Flip each letter's case **without** using `swapcase` (use `isupper`/`islower` with `upper`/`lower`).

**Input Format:** One line — a string.
**Output Format:** The case-flipped string.

**Sample Input:**
```
aBc
```
**Sample Output:**
```
AbC
```
---

## 37 — Ord Checksum  [M]

Print the sum of the character codes of the string, mod a given `n`.

**Input Format:** Two lines — the string, then `n`.
**Output Format:** The checksum.

**Sample Input:**
```
abc
100
```
**Sample Output:**
```
94
```
---

## 38 — Remove Every Kth  [M]

Remove every `k`-th character (positions k, 2k, … counting from 1) and print what remains.

**Input Format:** Two lines — the string, then `k` (k ≥ 1).
**Output Format:** The thinned string.

**Sample Input:**
```
abcdef
3
```
**Sample Output:**
```
abde
```
---

## 39 — Vowel Replace  [M]

Replace every vowel with a given character.

**Input Format:** Two lines — the string, then a single replacement character.
**Output Format:** The transformed string.

**Sample Input:**
```
education
_
```
**Sample Output:**
```
_d_c_t__n
```
---

## 40 — Repeat Pattern  [E]

Print a string repeated `k` times, separated by `-`.

**Input Format:** Two lines — the string, then `k` (k ≥ 1).
**Output Format:** `s-s-…-s` with k copies.

**Sample Input:**
```
ab
3
```
**Sample Output:**
```
ab-ab-ab
```
---

*End of Batch 2 — 20 problems. Difficulty: 2 [E] · 10 [M] · 8 [H]. All reference solutions verified by execution.*