# Test 01 — String Basics

*Unit 4 · Strings. Covers Topics 01–03: introduction & immutability, indexing & slicing, and case & whitespace methods.*
*Marks: Section A — 10 MCQ × 1 = 10. Section B — 10 coding × 3 = 30. **Total 40.** Answers and marking scheme in `test-01-string-basics-answers.md`.*

---

## Section A — Multiple Choice (1 mark each)

**Q1. [E]** What does this print?
```python
print('Age ' + str(18))
```
- A) `Age 18`
- B) `Age18`
- C) `Age 18` with an error
- D) `Age +18`

**Q2. [M]** What does this print?
```python
print('coding'[-2])
```
- A) `g`
- B) `n`
- C) `i`
- D) `d`

**Q3. [M]** What does this print?
```python
print('elephant'[2:5])
```
- A) `eph a`
- B) `leph`
- C) `eph`
- D) `epha`

**Q4. [H]** What does this print?
```python
print('abcdef'[1::2])
```
- A) `ace`
- B) `bcd`
- C) `bdf` reversed
- D) `bdf`

**Q5. [H]** What happens here?
```python
s = 'cat'
s[1] = 'u'
print(s)
```
- A) An error — strings can't be changed in place
- B) `cut`
- C) `cat`
- D) `cau`

**Q6. [M]** What does this print?
```python
print('mIXeD'.title())
```
- A) `MIXED`
- B) `Mixed`
- C) `mIXeD`
- D) `MIxED`

**Q7. [M]** What does this print? (brackets show the exact edges)
```python
print('[' + 'ab  '.rstrip() + ']')
```
- A) `[ab  ]`
- B) `[  ab]`
- C) `[ab]`
- D) `[ab ]`

**Q8. [H]** What does this print?
```python
print('HELLO'.lower()[::-1])
```
- A) hello
- B) `OLLEH`
- C) `HELLO`
- D) `olleh`

**Q9. [M]** What does this print?
```python
print(len('ab' * 3))
```
- A) `6`
- B) 3
- C) `2`
- D) `ababab`

**Q10. [E]** What does this print?
```python
print('PyThOn'.swapcase())
```
- A) `PYTHON`
- B) `pYtHoN`
- C) python
- D) `PyThOn`

---

## Section B — Coding (3 marks each)

*Judge-format: read input with `input()`, print exact output.*

**Q11. [E] Last Three** — Print the last three characters of a string.
- **Input:** `birthday`  →  **Output:** `day`

**Q12. [M] Upper First Half** — Print the first half of a string (up to but not including the middle for even length) in uppercase.
- **Input:** `abcdef`  →  **Output:** `ABC`

**Q13. [E] Second Letter Capital** — Print the second character of a string in uppercase.
- **Input:** `hello`  →  **Output:** `E`

**Q14. [M] Reverse and Shout** — Print the string reversed and in uppercase.
- **Input:** `stop`  →  **Output:** `POTS`

**Q15. [M] Trimmed Length** — Print the length of the string after removing whitespace from both ends.
- **Input:** `  data  `  →  **Output:** `4`

**Q16. [H] Middle Three** — Print the three characters in the centre of an odd-length string (the middle character and its two neighbours).
- **Input:** `abcdefg`  →  **Output:** `cde`

**Q17. [M] Ends Uppercased** — Print the first and last characters joined together, in uppercase.
- **Input:** `python`  →  **Output:** `PN`

**Q18. [H] Count Vowels** — Print how many vowels (a, e, i, o, u) the string contains, ignoring case.
- **Input:** `Programming`  →  **Output:** `3`

**Q19. [M] Every Second, Uppercased** — Print every second character (positions 0, 2, 4, …) in uppercase.
- **Input:** `abcdefgh`  →  **Output:** `ACEG`

**Q20. [H] Clean Heading** — Print the string with surrounding whitespace removed and each word capitalised.
- **Input:** `  hello world  `  →  **Output:** `Hello World`

---
*End of Test 01 paper.*