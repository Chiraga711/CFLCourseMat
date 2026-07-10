# Topic 03 — String Methods I (Case & Whitespace) · Coding

*Unit 4 · Strings. Six judge-format problems on case and whitespace methods. Read input with `input()`, produce exact-match output. Each shows a verified reference solution. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Shout It  [E]

Print the input string entirely in uppercase.

**Input Format:** A single line — a string `s`.
**Output Format:** `s` in uppercase.

**Sample Input:**
```
hello
```
**Sample Output:**
```
HELLO
```

**Solution:**
```python
s = input()
print(s.upper())
```

---

## 2 — Title Case a Heading  [M]

Print the string with the first letter of every word capitalised.

**Input Format:** A single line — a string `s`.
**Output Format:** `s` in title case.

**Sample Input:**
```
the lord of rings
```
**Sample Output:**
```
The Lord Of Rings
```

**Solution:**
```python
s = input()
print(s.title())
```
`title()` capitalises the first letter of each word and lowercases the rest.

---

## 3 — Trimmed Length  [M]

Print the length of the string **after** removing whitespace from both ends.

**Input Format:** A single line — a string `s` that may have leading/trailing spaces.
**Output Format:** A single integer — the length of the trimmed string.

**Sample Input:**
```
   hi there   
```
**Sample Output:**
```
8
```

**Solution:**
```python
s = input()
print(len(s.strip()))
```
`strip()` removes the outer spaces, leaving `hi there` (8 characters, including the space in the middle). Only the **outer** whitespace is removed.

---

## 4 — Flip the Case  [M]

Print the string with every letter's case swapped.

**Input Format:** A single line — a string `s`.
**Output Format:** `s` with upper↔lower case swapped.

**Sample Input:**
```
Hello World
```
**Sample Output:**
```
hELLO wORLD
```

**Solution:**
```python
s = input()
print(s.swapcase())
```

---

## 5 — Clean a Name  [H]

A name has been entered with stray spaces and inconsistent capitalisation. Print it tidied: no surrounding spaces, first letter uppercase, the rest lowercase.

**Input Format:** A single line — a name `s`, possibly padded with spaces and mis-cased.
**Output Format:** The cleaned name.

**Sample Input:**
```
  rAVI  
```
**Sample Output:**
```
Ravi
```

**Solution:**
```python
s = input()
print(s.strip().capitalize())
```
Chain the methods: `strip()` removes the spaces, then `capitalize()` fixes the case (first letter up, rest down).

---

## 6 — Count Lowercase Letters  [H]

Print how many characters of the string are lowercase letters. (A character is lowercase if changing it to uppercase would change it.)

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the number of lowercase letters.

**Sample Input:**
```
Hello World
```
**Sample Output:**
```
8
```

**Solution:**
```python
s = input()
count = 0
for ch in s:
    if ch != ch.upper():
        count += 1
print(count)
```
A lowercase letter differs from its uppercase form, so `ch != ch.upper()` detects it. In `Hello World`, `H` and `W` are the only uppercase letters and the space is unaffected, leaving 8 lowercase letters. (The output is a **count**, not a yes/no, so it can't be guessed.)

---

*End of Topic 03 coding — 6 problems. Every reference solution verified by execution.*
