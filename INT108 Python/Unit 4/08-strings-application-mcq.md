# Topic 08 — Strings + Loops/Conditionals (Application) · MCQ

*Unit 4 · Strings. The capstone topic: ten questions that combine indexing, slicing, methods, iteration, and conditionals to solve real problems — palindromes, validation, counting, and transforming text. Tags: [E] easy · [M] medium · [H] hard. Answers in `08-strings-application-mcq-answers.md`.*

---

**Q1. [M]** A program checks whether a word reads the same forwards and backwards:
```python
s = 'level'
print(s == s[::-1])
```
What does it print?
- A) `True`
- B) `False`
- C) `level`
- D) `levellevel`

**Q2. [M]** What does this print?
```python
s = 'a b c d e'
print(len(s.split()) > 3)
```
- A) `False`
- B) `True`
- C) `5`
- D) `4`

**Q3. [H]** What does this print?
```python
s = 'a-b-c'
print(s.replace('-', ' ').upper())
```
- A) `a b c`
- B) `A-B-C`
- C) `A B C`
- D) `ABC`

**Q4. [M]** What does this print?
```python
c = 0
for ch in 'HeLLo':
    if ch.isupper():
        c += 1
print(c)
```
- A) `2`
- B) `5`
- C) `4`
- D) `3`

**Q5. [H]** A program builds initials from a name:
```python
r = ''
for w in 'big red apple'.split():
    r = r + w[0]
print(r.upper())
```
What is printed?
- A) `BRA`
- B) `bra`
- C) `BIG`
- D) `B R A`

**Q6. [M]** What does this print?
```python
total = 0
for ch in '12345':
    total += int(ch)
print(total)
```
- A) `12345`
- B) `15`
- C) `5`
- D) `54321`

**Q7. [M]** A form validates a 4-digit year:
```python
s = '2024'
print(s.isdigit() and len(s) == 4)
```
What does it print?
- A) `False`
- B) `2024`
- C) `True`
- D) `4`

**Q8. [H]** What does this print?
```python
print(' '.join('one two three'.split()[::-1]))
```
- A) `one two three`
- B) `eerht owt eno`
- C) `three-two-one`
- D) `three two one`

**Q9. [M]** What does this print?
```python
v = 'aeiou'
c = 0
for ch in 'programming':
    if ch in v:
        c += 1
print(c)
```
- A) `3`
- B) `4`
- C) `2`
- D) `11`

**Q10. [M]** What does this print?
```python
s = 'hello world'
print(s.title() == 'Hello World')
```
- A) `False`
- B) `True`
- C) `Hello World`
- D) `hello world`
