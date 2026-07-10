# Topic 05 — Splitting & Joining · Coding

*Unit 4 · Strings. Six judge-format problems on `split` and `join`. Read input with `input()`, produce exact-match output. Each shows a verified reference solution. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Word Count  [E]

Print how many words are in a sentence (words are separated by spaces).

**Input Format:** A single line — a sentence `s`.
**Output Format:** A single integer — the number of words.

**Sample Input:**
```
the quick brown fox
```
**Sample Output:**
```
4
```

**Solution:**
```python
s = input()
print(len(s.split()))
```
`split()` with no argument breaks the sentence into a list of words; `len` counts them.

---

## 2 — Hyphenate Words  [M]

Print the words of a sentence joined together with hyphens instead of spaces.

**Input Format:** A single line — a sentence `s`.
**Output Format:** The words joined by `-`.

**Sample Input:**
```
a b c
```
**Sample Output:**
```
a-b-c
```

**Solution:**
```python
s = input()
print('-'.join(s.split()))
```
Split into words, then `join` them back with `-` between each.

---

## 3 — First Word  [E]

Print the first word of a sentence.

**Input Format:** A single line — a sentence `s`.
**Output Format:** The first word.

**Sample Input:**
```
hello world foo
```
**Sample Output:**
```
hello
```

**Solution:**
```python
s = input()
print(s.split()[0])
```
`split()` gives a list; index 0 is the first word.

---

## 4 — Last Word  [M]

Print the last word of a sentence.

**Input Format:** A single line — a sentence `s`.
**Output Format:** The last word.

**Sample Input:**
```
hello world foo
```
**Sample Output:**
```
foo
```

**Solution:**
```python
s = input()
print(s.split()[-1])
```
Negative indexing on the word list gives the last word.

---

## 5 — Reverse Word Order  [H]

Print the words of a sentence in reverse order, separated by single spaces.

**Input Format:** A single line — a sentence `s`.
**Output Format:** The words in reverse order.

**Sample Input:**
```
one two three
```
**Sample Output:**
```
three two one
```

**Solution:**
```python
s = input()
w = s.split()
print(' '.join(w[::-1]))
```
Split into words, reverse the list with `[::-1]`, then join back with spaces.

---

## 6 — Sum a CSV Line  [H]

A line contains integers separated by commas. Print their sum.

**Input Format:** A single line — integers separated by commas, with no spaces.
**Output Format:** A single integer — the total.

**Sample Input:**
```
10,20,30,5
```
**Sample Output:**
```
65
```

**Solution:**
```python
s = input()
parts = s.split(',')
total = 0
for p in parts:
    total += int(p)
print(total)
```
`split(',')` gives the pieces as strings; convert each with `int` before adding.

---

*End of Topic 05 coding — 6 problems. Every reference solution verified by execution.*
