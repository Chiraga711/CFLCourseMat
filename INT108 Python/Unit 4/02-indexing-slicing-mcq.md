# Topic 02 — Indexing & Slicing · MCQ

*Unit 4 · Strings. Ten questions on accessing characters by position (including negative indices) and extracting ranges with slicing. Tags: [E] easy · [M] medium · [H] hard. Answers in `02-indexing-slicing-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
print('python'[0])
```
- A) `p`
- B) `python`
- C) `n`
- D) An error

**Q2. [E]** What does this print?
```python
print('hello'[-1])
```
- A) `h`
- B) `o`
- C) `hello`
- D) An error

**Q3. [M]** What does this print?
```python
print('world'[1:4])
```
- A) `orld`
- B) `wor`
- C) `orl`
- D) `orl d`

**Q4. [E]** What does this print?
```python
print('abcdef'[:3])
```
- A) `abcd`
- B) `def`
- C) `abcdef`
- D) `abc`

**Q5. [M]** What does this print?
```python
print('abcdef'[3:])
```
- A) `def`
- B) `abc`
- C) `abcd`
- D) `ef`

**Q6. [M]** What does this print?
```python
print('python'[-3:])
```
- A) `pyt`
- B) `hon`
- C) `tho`
- D) `hon `

**Q7. [M]** What does this print?
```python
print('abcdefgh'[::2])
```
- A) `bdfh`
- B) `abcd`
- C) `aceg`
- D) `aceg h`

**Q8. [M]** What does this print?
```python
print('hello'[::-1])
```
- A) `hello`
- B) `hlo`
- C) `olle`
- D) `olleh`

**Q9. [H]** What does this print?
```python
s = 'python'
print(s[len(s) - 1])
```
- A) `n`
- B) `p`
- C) `6`
- D) An error

**Q10. [H]** What happens here?
```python
print('abc'[5])
```
- A) `c`
- B) An error — the index is past the end of the string
- C) `abc`
- D) Nothing is printed
