# Topic 06 — Iteration & Building · MCQ

*Unit 4 · Strings. Ten questions on looping over characters (`for ch in s`), building a result string by accumulation, index-based loops with `len`, and membership tests (`in` / `not in`). Tags: [E] easy · [M] medium · [H] hard. Answers in `06-iteration-building-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
for ch in 'ab':
    print(ch)
```
- A) `a` and `b` on separate lines
- B) `ab`
- C) `a b`
- D) `ch ch`

**Q2. [E]** What does this print?
```python
c = 0
for ch in 'hello':
    c += 1
print(c)
```
- A) `4`
- B) `5`
- C) `hello`
- D) `1`

**Q3. [H]** What does this print?
```python
r = ''
for ch in 'abc':
    r = ch + r
print(r)
```
- A) `abc`
- B) `aabbcc`
- C) `cba`
- D) `c`

**Q4. [M]** What does this print?
```python
print('cat' in 'concatenate')
```
- A) `False`
- B) `cat`
- C) `3`
- D) `True`

**Q5. [M]** What does this print?
```python
c = 0
for ch in 'education':
    if ch in 'aeiou':
        c += 1
print(c)
```
- A) `5`
- B) `4`
- C) `9`
- D) `3`

**Q6. [M]** What does this print?
```python
r = ''
for ch in 'a1b2c3':
    if ch in '0123456789':
        r = r + ch
print(r)
```
- A) `abc`
- B) `123`
- C) `a1b2c3`
- D) `6`

**Q7. [H]** What does this print?
```python
r = ''
for ch in 'abc':
    r = r + ch * 2
print(r)
```
- A) `abcabc`
- B) `abc`
- C) `aabbcc`
- D) `cba`

**Q8. [M]** What does this print?
```python
s = 'code'
for i in range(len(s)):
    print(s[i], end='')
```
- A) `0123`
- B) `c o d e`
- C) `edoc`
- D) `code`

**Q9. [M]** What does this print?
```python
print('x' not in 'python')
```
- A) `True`
- B) `False`
- C) `x`
- D) An error

**Q10. [H]** What does this print?
```python
c = 0
for ch in 'a b c d':
    if ch == ' ':
        c += 1
print(c)
```
- A) `4`
- B) `3`
- C) `7`
- D) `0`
