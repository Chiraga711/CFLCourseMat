# Topic 08 — Strings + Loops/Conditionals (Application) · Coding

*Unit 4 · Strings. Six judge-format problems that combine everything from the unit — slicing, methods, iteration, and conditionals — to solve real tasks. Read input with `input()`, produce exact-match output. Outputs are computed values (counts, totals), never guessable labels. Difficulty: [E] easy · [M] medium · [H] hard.*

---

## 1 — Palindrome Match Count  [M]

For each position in a string, check whether the character matches the character at the mirror position from the other end. Print how many positions match. (If every position matches, the word is a palindrome and the count equals the string's length.)

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the number of matching mirror positions.

**Sample Input:**
```
level
```
**Sample Output:**
```
5
```

**Solution:**
```python
s = input()
c = 0
for i in range(len(s)):
    if s[i] == s[len(s) - 1 - i]:
        c += 1
print(c)
```
Position `i` is compared with `len(s) - 1 - i` (its mirror). For `level`, all 5 match. The **count** carries information — unlike a plain `True`/`False`, it can't be guessed, and it reveals *how close* a word is to being a palindrome.

---

## 2 — Count Long Words  [M]

Print how many words in a sentence have more than 3 characters.

**Input Format:** A single line — a sentence `s`.
**Output Format:** A single integer — the number of words longer than 3 characters.

**Sample Input:**
```
the quick brown fox jumps
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
c = 0
for w in s.split():
    if len(w) > 3:
        c += 1
print(c)
```
Split into words, then test each word's length — `quick`, `brown`, `jumps` qualify.

---

## 3 — Make Initials  [H]

Print the initials of a name: the first letter of each word, uppercased and joined together.

**Input Format:** A single line — a name `s` (words separated by spaces).
**Output Format:** The uppercase initials.

**Sample Input:**
```
mahatma gandhi road
```
**Sample Output:**
```
MGR
```

**Solution:**
```python
s = input()
r = ''
for w in s.split():
    r = r + w[0].upper()
print(r)
```
Split into words, take each word's first character (`w[0]`), uppercase it, and build the result.

---

## 4 — Sum the Digits in Text  [M]

A string mixes letters and digits. Print the sum of all the digits it contains.

**Input Format:** A single line — a string `s`.
**Output Format:** A single integer — the sum of the digit characters.

**Sample Input:**
```
a1b2c3
```
**Sample Output:**
```
6
```

**Solution:**
```python
s = input()
total = 0
for ch in s:
    if ch.isdigit():
        total += int(ch)
print(total)
```
Only digit characters are converted with `int` and added: 1 + 2 + 3 = 6.

---

## 5 — Words Starting with a Vowel  [H]

Print how many words in a sentence begin with a vowel (a, e, i, o, u), ignoring case.

**Input Format:** A single line — a sentence `s`.
**Output Format:** A single integer — the number of words starting with a vowel.

**Sample Input:**
```
apple orange banana egg
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
c = 0
for w in s.split():
    if w[0].lower() in 'aeiou':
        c += 1
print(c)
```
Check the first letter of each word against the vowels — `apple`, `orange`, `egg` qualify (`banana` does not).

---

## 6 — Password Strength  [H]

A password's strength is the number of character *categories* it contains among three: uppercase letters, lowercase letters, and digits. Print that number (0 to 3).

**Input Format:** A single line — a password `s`.
**Output Format:** A single integer (0–3) — how many of the three categories appear.

**Sample Input:**
```
Abc123
```
**Sample Output:**
```
3
```

**Solution:**
```python
s = input()
has_upper = 0
has_lower = 0
has_digit = 0
for ch in s:
    if ch.isupper():
        has_upper = 1
    if ch.islower():
        has_lower = 1
    if ch.isdigit():
        has_digit = 1
print(has_upper + has_lower + has_digit)
```
Three flags track whether each category has appeared; their sum is the strength. `Abc123` has all three → 3. The **number** is more informative than a yes/no "strong enough" answer.

---

*End of Topic 08 coding — 6 problems. Every reference solution verified by execution. This completes the Strings unit topics.*
