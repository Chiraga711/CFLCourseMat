# Strings Coding Bank — Batch 5: Two-String Problems (81–100)

*Pair-wise string logic: prefixes, merges, comparisons, and cross-string builds.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-05-twostring-solutions.md`.*

---

## 81 — Common Prefix Length  [M]

Print how many characters two strings share at the **start** (stop at the first mismatch).

**Input Format:** Two lines — two strings.
**Output Format:** The shared-prefix length.

**Sample Input:**
```
abcde
abfde
```
**Sample Output:**
```
2
```
---

## 82 — Common Suffix Length  [H]

Print how many characters two strings share at the **end**.

**Input Format:** Two lines — two strings.
**Output Format:** The shared-suffix length.

**Sample Input:**
```
walking
running
```
**Sample Output:**
```
3
```
---

## 83 — Censored Diff  [M]

Two strings have equal length. Print the first string, but with `*` at every position where the two strings differ.

**Input Format:** Two lines — two equal-length strings.
**Output Format:** The masked first string.

**Sample Input:**
```
paste
taste
```
**Sample Output:**
```
*aste
```
---

## 84 — Merge Alternate (Unequal)  [H]

Merge two strings by alternating characters; when the shorter one runs out, append the rest of the longer one.

**Input Format:** Two lines — two strings (any lengths).
**Output Format:** The merged string.

**Sample Input:**
```
abc
xy
```
**Sample Output:**
```
axbyc
```
---

## 85 — Vowel Count Difference  [M]

Print the vowel count of the first string minus the vowel count of the second (can be negative).

**Input Format:** Two lines — two lowercase strings.
**Output Format:** The difference (may be negative).

**Sample Input:**
```
audio
sky
```
**Sample Output:**
```
4
```
---

## 86 — Lexicographically Smaller  [M]

Print whichever string comes first in dictionary order (print the first one if they are equal).

**Input Format:** Two lines — two lowercase strings.
**Output Format:** The smaller string.

**Sample Input:**
```
banana
apple
```
**Sample Output:**
```
apple
```
---

## 87 — Length Gap  [E]

Print the difference between the two strings' lengths as a positive number.

**Input Format:** Two lines — two strings.
**Output Format:** The absolute length difference.

**Sample Input:**
```
hello
hi
```
**Sample Output:**
```
3
```
---

## 88 — Word Match Positions  [M]

Two sentences have the same number of words. Print how many positions hold the **same word** in both.

**Input Format:** Two lines — two sentences with equal word counts.
**Output Format:** The matching-position count.

**Sample Input:**
```
the cat ran
the dog ran
```
**Sample Output:**
```
2
```
---

## 89 — Build an ID  [E]

Build an ID from two names: the first 3 characters of the first name + the last 3 of the second, all lowercase.

**Input Format:** Two lines — two names (each at least 3 characters).
**Output Format:** The 6-character ID.

**Sample Input:**
```
Ravinder
Kumar
```
**Sample Output:**
```
ravmar
```
---

## 90 — Missing Characters  [M]

Print how many characters of the second string do **not** appear anywhere in the first.

**Input Format:** Two lines — two strings.
**Output Format:** The count of missing characters.

**Sample Input:**
```
apple
plum
```
**Sample Output:**
```
2
```
---

## 91 — Alternating Word Merge  [M]

Two sentences have the same number of words. Print them merged word-by-word: first word of A, first of B, second of A, second of B, …

**Input Format:** Two lines — two sentences with equal word counts.
**Output Format:** The merged sentence.

**Sample Input:**
```
one two
1 2
```
**Sample Output:**
```
one 1 two 2
```
---

## 92 — Same-Ends Score  [E]

Score two strings 0–2: one point if their first characters match, one point if their last characters match.

**Input Format:** Two lines — two non-empty strings.
**Output Format:** An integer 0, 1 or 2.

**Sample Input:**
```
mango
music
```
**Sample Output:**
```
1
```
---

## 93 — Overlap Join  [M]

The last `k` characters of the first string equal the first `k` of the second. Join them **without repeating** the overlap.

**Input Format:** Three lines — string A, string B, then the overlap size `k`.
**Output Format:** The joined string.

**Sample Input:**
```
classroom
roomlight
4
```
**Sample Output:**
```
classroomlight
```
---

## 94 — Position-Sum Difference  [M]

For two lowercase words, print (alphabet-position sum of the first) minus (that of the second), where `a`=1 … `z`=26.

**Input Format:** Two lines — two lowercase words.
**Output Format:** The difference (may be negative).

**Sample Input:**
```
abc
aa
```
**Sample Output:**
```
4
```
---

## 95 — Rotation Detector  [H]

String B may be a *rotation* of string A (A's characters shifted around, like `abcde` → `cdeab`). Search for B inside A joined to itself (`A + A`) and print the position found — that position is the rotation amount. Print `-1` if B is not found there (not a rotation).

**Input Format:** Two lines — two equal-length strings.
**Output Format:** The rotation amount, or `-1`.

**Sample Input:**
```
abcde
cdeab
```
**Sample Output:**
```
2
```
---

## 96 — Cross-Swapped Halves  [H]

Two even-length strings swap second halves. Print two lines: A's first half + B's second half, then B's first half + A's second half.

**Input Format:** Two lines — two even-length strings.
**Output Format:** Two lines — the cross-joined strings.

**Sample Input:**
```
abcd
wxyz
```
**Sample Output:**
```
abyz
wxcd
```
---

## 97 — Zip Word Initials  [M]

Two sentences have the same number of words. Print the first letters alternating: A's word 1, B's word 1, A's word 2, …

**Input Format:** Two lines — two sentences with equal word counts.
**Output Format:** The zipped initials, no spaces.

**Sample Input:**
```
silver moon
gold star
```
**Sample Output:**
```
sgms
```
---

## 98 — Shared Characters  [M]

Print how many characters of the first string (counting repeats, position by position) appear **anywhere** in the second.

**Input Format:** Two lines — two strings.
**Output Format:** The count.

**Sample Input:**
```
apple
pel
```
**Sample Output:**
```
4
```
---

## 99 — Shared Words  [H]

Print how many words of the first sentence also appear (anywhere) as words of the second. Count repeats in the first sentence each time.

**Input Format:** Two lines — two sentences.
**Output Format:** The count.

**Sample Input:**
```
the cat sat
a cat sat here
```
**Sample Output:**
```
2
```
---

## 100 — Extra Tail  [E]

One string is longer than the other. Print the part of the longer string that extends beyond the shorter one's length.

**Input Format:** Two lines — two strings of different lengths.
**Output Format:** The tail of the longer string.

**Sample Input:**
```
weekend
week
```
**Sample Output:**
```
end
```
---

*End of Batch 5 — 20 problems. Difficulty: 4 [E] · 11 [M] · 5 [H]. All reference solutions verified by execution.*