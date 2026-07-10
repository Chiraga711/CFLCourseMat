# Topic 07 — Formatting · MCQ

*Unit 4 · Strings. Ten questions on f-strings, two-decimal formatting (`:.2f`), the `.format()` method, and the `ord`/`chr` character-code functions. Key idea: `:.2f` always shows two decimals (keeping trailing zeros), unlike `round()`. Tags: [E] easy · [M] medium · [H] hard. Answers in `07-formatting-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
name = 'Ravi'
print(f'Hi {name}')
```
- A) `Hi Ravi`
- B) `Hi {name}`
- C) `Hi name`
- D) `Ravi`

**Q2. [M]** What does this print?
```python
a = 3
b = 4
print(f'{a + b}')
```
- A) `{a + b}`
- B) `7`
- C) `34`
- D) `a + b`

**Q3. [M]** What does this print?
```python
x = 3.5
print(f'{x:.2f}')
```
- A) `3.5`
- B) `3`
- C) `3.50`
- D) `3.500`

**Q4. [H]** What does this print?
```python
print(round(3.5, 2))
```
- A) `3.50`
- B) `4`
- C) `3.500`
- D) `3.5`

**Q5. [M]** What does this print?
```python
print(f'{10 / 4:.2f}')
```
- A) `2.50`
- B) `2.5`
- C) `2`
- D) `2.500`

**Q6. [M]** What does this print?
```python
print(ord('A'))
```
- A) `97`
- B) `65`
- C) `A`
- D) `1`

**Q7. [M]** What does this print?
```python
print(chr(66))
```
- A) `A`
- B) `66`
- C) `B`
- D) `b`

**Q8. [E]** What does this print?
```python
print('{} and {}'.format('a', 'b'))
```
- A) `{} and {}`
- B) `a and a`
- C) `b and a`
- D) `a and b`

**Q9. [H]** What does this print?
```python
print('{1} {0}'.format('world', 'hello'))
```
- A) `hello world`
- B) `world hello`
- C) `{1} {0}`
- D) `hello hello`

**Q10. [H]** What does this print?
```python
print(chr(ord('a') + 1))
```
- A) `a`
- B) `b`
- C) `98`
- D) `ab`
