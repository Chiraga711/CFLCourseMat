# Topic 03 — String Methods I (Case & Whitespace) · MCQ

*Unit 4 · Strings. Ten questions on `upper`, `lower`, `title`, `capitalize`, `strip`/`lstrip`/`rstrip`, and `swapcase`. Remember: these methods return a **new** string and never change the original. Tags: [E] easy · [M] medium · [H] hard. Answers in `03-string-methods-1-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
print('hello'.upper())
```
- A) `HELLO`
- B) `hello`
- C) `Hello`
- D) An error

**Q2. [E]** What does this print?
```python
print('WORLD'.lower())
```
- A) `WORLD`
- B) `world`
- C) `World`
- D) `wORLD`

**Q3. [M]** What does this print?
```python
print('hello world'.title())
```
- A) `Hello world`
- B) `HELLO WORLD`
- C) `Hello World`
- D) `hello world`

**Q4. [H]** What does this print?
```python
print('hello WORLD'.capitalize())
```
- A) `Hello WORLD`
- B) `Hello World`
- C) `HELLO WORLD`
- D) `Hello world`

**Q5. [E]** What does this print?
```python
print('  hi  '.strip())
```
- A) `hi`
- B) `  hi  `
- C) `  hi`
- D) `hi  `

**Q6. [M]** What does this print? (the quotes show where the text begins and ends)
```python
print('[' + '  hi  '.lstrip() + ']')
```
- A) `[  hi]`
- B) `[hi  ]`
- C) `[hi]`
- D) `[  hi  ]`

**Q7. [M]** What does this print? (the brackets show the exact edges)
```python
print('[' + '  hi  '.rstrip() + ']')
```
- A) `[hi  ]`
- B) `[hi]`
- C) `[  hi]`
- D) `[  hi  ]`

**Q8. [M]** What does this print?
```python
print('Hello World'.swapcase())
```
- A) `HELLO WORLD`
- B) `hello world`
- C) `Hello World`
- D) `hELLO wORLD`

**Q9. [H]** What does this print?
```python
s = 'hello'
s.upper()
print(s)
```
- A) `hello`
- B) `HELLO`
- C) `Hello`
- D) An error

**Q10. [H]** What does this print?
```python
print('  Python  '.strip().upper())
```
- A) `  PYTHON  `
- B) `PYTHON`
- C) `  python  `
- D) `Python`
