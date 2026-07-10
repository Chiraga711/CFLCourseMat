# Topic 02 — Indexing & Slicing · Coding

*Unit 4 · Strings. Six judge-format problems on indexing and slicing. Read input with `input()`, produce exact-match output. Each problem shows a verified reference solution below it. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — First and Last  [E]

Print the first and last characters of a string, separated by a space.

**Input Format:** A single line — a non-empty string `s`.
**Output Format:** The first character and the last character, separated by a space.

**Sample Input:**
```
mango
```
**Sample Output:**
```
m o
```

**Solution:**
```python
s = input()
print(s[0], s[-1])
```
`s[0]` is the first character, `s[-1]` the last (negative indexing counts from the end).

---

## 2 — Middle Character  [M]

Print the middle character of an odd-length string.

**Input Format:** A single line — a string `s` with an odd number of characters.
**Output Format:** The single middle character.

**Sample Input:**
```
hello
```
**Sample Output:**
```
l
```

**Solution:**
```python
s = input()
print(s[len(s) // 2])
```
For length 5, `len(s) // 2` is 2 — the middle index. Integer division lands exactly on the centre for odd lengths.

---

## 3 — Reverse a String  [E]

Print the string reversed.

**Input Format:** A single line — a string `s`.
**Output Format:** The characters of `s` in reverse order.

**Sample Input:**
```
stressed
```
**Sample Output:**
```
desserts
```

**Solution:**
```python
s = input()
print(s[::-1])
```
A slice with step −1 walks the string from end to start.

---

## 4 — First N Characters  [M]

Read a string and a number `n`, and print the first `n` characters.

**Input Format:** Two lines — the string `s`, then an integer `n` (0 ≤ n ≤ len(s)).
**Output Format:** The first `n` characters of `s`.

**Sample Input:**
```
programming
3
```
**Sample Output:**
```
pro
```

**Solution:**
```python
s = input()
n = int(input())
print(s[:n])
```
`s[:n]` takes from the start up to (not including) index `n`.

---

## 5 — Every Second Character  [M]

Print every second character of a string, starting from the first.

**Input Format:** A single line — a string `s`.
**Output Format:** Characters at positions 0, 2, 4, … joined together.

**Sample Input:**
```
abcdefg
```
**Sample Output:**
```
aceg
```

**Solution:**
```python
s = input()
print(s[::2])
```
The step 2 skips every other character: positions 0, 2, 4, 6.

---

## 6 — Last N Characters  [H]

Read a string and a number `n`, and print the last `n` characters.

**Input Format:** Two lines — the string `s`, then an integer `n` (1 ≤ n ≤ len(s)).
**Output Format:** The last `n` characters of `s`.

**Sample Input:**
```
download
4
```
**Sample Output:**
```
load
```

**Solution:**
```python
s = input()
n = int(input())
print(s[-n:])
```
`s[-n:]` starts `n` characters from the end and runs to the end. When `n` equals the length, this returns the whole string.

---

*End of Topic 02 coding — 6 problems. Every reference solution verified by execution.*
