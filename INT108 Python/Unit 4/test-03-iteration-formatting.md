# Test 03 — Iteration, Formatting & Application

*Unit 4 · Strings. Covers Topics 06–08: iteration & building, formatting, and applied string processing. Every question is a real text-processing scenario, and the coding section combines skills across topics.*
*Marks: Section A — 10 MCQ × 1 = 10. Section B — 10 coding × 3 = 30. **Total 40.** Answers and marking scheme in `test-03-iteration-formatting-answers.md`.*

---

## Section A — Multiple Choice (1 mark each)

**Q1. [E]** A loyalty app counts the letters in a coupon code:
```python
c = 0
for ch in 'SAVE20':
    if ch.isalpha():
        c += 1
print(c)
```
What does it print?
- A) `4`
- B) `6`
- C) `2`
- D) `SAVE`

**Q2. [M]** A spam filter builds a censored version of a word:
```python
r = ''
for ch in 'bad':
    r = r + '*'
print(r)
```
What is printed?
- A) `bad`
- B) `***`
- C) `*`
- D) `b*a*d`

**Q3. [H]** A typing game reverses what the player typed:
```python
r = ''
for ch in 'top':
    r = ch + r
print(r)
```
What is printed?
- A) `top`
- B) `ttoopp`
- C) `pot`
- D) `opt`

**Q4. [E]** A search box checks whether the term appears in a product name:
```python
print('cat' in 'category')
```
- A) `False`
- B) `cat`
- C) `3`
- D) `True`

**Q5. [M]** A receipt prints the total:
```python
total = 249.5
print(f'{total:.2f}')
```
What is printed?
- A) `249.50`
- B) `249.5`
- C) `249`
- D) `250.00`

**Q6. [H]** A billing system tries to show two decimals with `round`:
```python
print(round(99.0, 2))
```
What is printed?
- A) `99.00`
- B) `99.0`
- C) `99`
- D) `99.000`

**Q7. [M]** A keypad app finds the next letter:
```python
print(chr(ord('C') + 1))
```
- A) `C`
- B) `68`
- C) `D`
- D) `B`

**Q8. [M]** An invoice line multiplies quantity by price inside an f-string:
```python
q = 3
p = 50
print(f'Total: {q * p}')
```
- A) `Total: {q * p}`
- B) `Total: 350`
- C) `Total: 53`
- D) `Total: 150`

**Q9. [M]** A grader counts the digits in a roll number:
```python
c = 0
for ch in 'CS2024':
    if ch.isdigit():
        c += 1
print(c)
```
- A) `4`
- B) `2`
- C) `6`
- D) `2024`

**Q10. [M]** A tag system shows tags in reverse order:
```python
print(' '.join('red green blue'.split()[::-1]))
```
- A) `red green blue`
- B) `blue green red`
- C) `eulb neerg der`
- D) `blue,green,red`

---

## Section B — Coding (3 marks each)

*Judge-format: read input with `input()`, print exact output. Where two inputs are shown separated by ` / `, they arrive on separate lines.*

**Q11. [E] Receipt Line** — A shop prints one receipt line. Read an item name and its price in paise; print `ITEM: PRICE` with the price in rupees to two decimals.
- **Input:** `Tea / 1550`  →  **Output:** `Tea: 15.50`

**Q12. [E] Count Spaces** — A word processor reports how many spaces a line contains. Print the count.
- **Input:** `a b c d`  →  **Output:** `3`

**Q13. [M] Censor a Word** — A chat filter replaces a banned word with asterisks of the same length. Read the word and print the mask.
- **Input:** `secret`  →  **Output:** `******`

**Q14. [M] Next Letters** — A simple encoder shifts every character of a code forward by one. Print the encoded string.
- **Input:** `abc`  →  **Output:** `bcd`

**Q15. [M] Letter Frequency** — A text tool counts how often a chosen letter appears, ignoring case. Read the text and the letter; print the count.
- **Input:** `Banana / A`  →  **Output:** `3`

**Q16. [M] Average Word Length** — A readability checker prints the average word length of a sentence, to two decimals.
- **Input:** `the quick brown fox`  →  **Output:** `4.00`

**Q17. [M] Alternating Caps** — A styling tool makes text alternate: characters at even positions uppercase, odd positions lowercase. Print the styled string.
- **Input:** `hello`  →  **Output:** `HeLlO`

**Q18. [H] Mirror Positions** — Read two strings of the same length. Print how many positions `i` satisfy: character `i` of the first string equals character `i`-from-the-end of the second string.
- **Input:** `abc / cxa`  →  **Output:** `2`

**Q19. [H] Longest Word** — A headline tool picks the longest word of a sentence (the first one if there is a tie). Print it.
- **Input:** `I love programming languages`  →  **Output:** `programming`

**Q20. [H] Checksum** — A simple checksum is the sum of the character codes of every character, taken mod 100. Print it.
- **Input:** `abc`  →  **Output:** `94`

---
*End of Test 03 paper.*