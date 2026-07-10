# Topic 04 — String Methods II (Search & Test) · Coding

*Unit 4 · Strings. Six judge-format problems on searching, counting, replacing, and testing characters. Read input with `input()`, produce exact-match output. Each shows a verified reference solution. Outputs are computed values (counts, positions), never guessable labels. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Count a Character  [E]

Read a string and a single character, and print how many times the character appears in the string.

**Input Format:** Two lines — the string `s`, then a single character `c`.
**Output Format:** A single integer — the count.

**Sample Input:**
```
banana
a
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
c = input()
print(s.count(c))
```

---

## 2 — First Space Position  [M]

Print the index of the first space in a string. (You may assume there is at least one space.)

**Input Format:** A single line — a string `s` containing at least one space.
**Output Format:** A single integer — the position of the first space.

**Sample Input:**
```
hello world
```
**Sample Output:**
```
5
```

**Solution:**
```python
s = input()
print(s.find(' '))
```
`find` returns the index of the first match. (If there were no space, `find` would return −1 rather than raising an error — unlike `index`.)

---

## 3 — Underscore the Spaces  [E]

Print the string with every space replaced by an underscore.

**Input Format:** A single line — a string `s`.
**Output Format:** `s` with all spaces turned into `_`.

**Sample Input:**
```
a b c
```
**Sample Output:**
```
a_b_c
```

**Solution:**
```python
s = input()
print(s.replace(' ', '_'))
```
`replace` swaps **every** occurrence.

---

## 4 — Count Digits  [M]

Print how many characters of the string are digits.

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the number of digit characters.

**Sample Input:**
```
ab12cd3
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
c = 0
for ch in s:
    if ch.isdigit():
        c += 1
print(c)
```
`ch.isdigit()` is True only for digit characters. The output is a **count**, so it can't be guessed.

---

## 5 — Count a Word  [M]

Read a sentence and a word, and print how many times the word appears in the sentence.

**Input Format:** Two lines — the sentence `s`, then the word `w`.
**Output Format:** A single integer — how many times `w` appears.

**Sample Input:**
```
the cat and the dog
the
```
**Sample Output:**
```
2
```

**Solution:**
```python
s = input()
w = input()
print(s.count(w))
```
`count` works with multi-character substrings, not just single characters.

---

## 6 — Length After Removal  [H]

Read a string and a character. Remove every occurrence of that character and print the length of what remains.

**Input Format:** Two lines — the string `s`, then a single character `c`.
**Output Format:** A single integer — the length after removing all `c`.

**Sample Input:**
```
banana
a
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
c = input()
print(len(s.replace(c, '')))
```
Replacing `c` with the empty string deletes it; `banana` without its three `a`s is `bnn`, length 3.

---

*End of Topic 04 coding — 6 problems. Every reference solution verified by execution.*
