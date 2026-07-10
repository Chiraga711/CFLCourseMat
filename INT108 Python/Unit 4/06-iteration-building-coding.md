# Topic 06 — Iteration & Building · Coding

*Unit 4 · Strings. Six judge-format problems on looping over characters and building results. Read input with `input()`, produce exact-match output. Each shows a verified reference solution. These use explicit loops (not shortcut methods) so you practise the character-by-character pattern. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Count Consonants  [E]

Loop over the string and print how many consonants it contains (letters that are not vowels), ignoring case. Non-letters do not count.

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the consonant count.

**Sample Input:**
```
Programming
```
**Sample Output:**
```
8
```

**Solution:**
```python
s = input()
c = 0
for ch in s.lower():
    if ch.isalpha() and ch not in 'aeiou':
        c += 1
print(c)
```
A consonant is a letter (`isalpha()`) that is not a vowel — both conditions must hold, so spaces and digits are excluded.

---

## 2 — Keep Only Digits  [M]

Build and print a new string containing only the digit characters of the input, in their original order.

**Input Format:** A single line — a string `s`.
**Output Format:** The digits of `s`, joined together.

**Sample Input:**
```
a1b2c3d4
```
**Sample Output:**
```
1234
```

**Solution:**
```python
s = input()
r = ''
for ch in s:
    if ch.isdigit():
        r = r + ch
print(r)
```
Start with an empty string and append each digit as it is found — the accumulator pattern.

---

## 3 — Count a Character  [M]

Read a string and a target character, and print how many times the character appears — by looping (not using `count`).

**Input Format:** Two lines — the string `s`, then a single character.
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
target = input()
c = 0
for ch in s:
    if ch == target:
        c += 1
print(c)
```
Compare each character to the target and tally the matches.

---

## 4 — Reverse by Building  [H]

Reverse the string by building the result one character at a time (not using slicing).

**Input Format:** A single line — a string `s`.
**Output Format:** `s` reversed.

**Sample Input:**
```
hello
```
**Sample Output:**
```
olleh
```

**Solution:**
```python
s = input()
r = ''
for ch in s:
    r = ch + r
print(r)
```
Placing each new character in **front** of the accumulator (`ch + r`) reverses the order.

---

## 5 — Count Uppercase Letters  [M]

Loop over the string and print how many characters are uppercase letters.

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the number of uppercase letters.

**Sample Input:**
```
HeLLo WoRLD
```
**Sample Output:**
```
7
```

**Solution:**
```python
s = input()
c = 0
for ch in s:
    if ch.isupper():
        c += 1
print(c)
```
`isupper()` is True only for uppercase letters (the space is ignored).

---

## 6 — Remove Vowels  [H]

Build and print the string with all vowels removed (both uppercase and lowercase).

**Input Format:** A single line — a string `s`.
**Output Format:** `s` with every vowel taken out.

**Sample Input:**
```
education
```
**Sample Output:**
```
dctn
```

**Solution:**
```python
s = input()
r = ''
for ch in s:
    if ch not in 'aeiouAEIOU':
        r = r + ch
print(r)
```
Keep a character only when it is **not** a vowel — checking against both cases in one test.

---

*End of Topic 06 coding — 6 problems. Every reference solution verified by execution.*
