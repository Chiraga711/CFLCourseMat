# Topic 04 — String Methods II (Search & Test) · MCQ

*Unit 4 · Strings. Ten questions on `find`, `index`, `count`, `replace`, `startswith`/`endswith`, and the `is…` test methods. Key idea: `find` returns −1 for a missing substring, but `index` raises an error. Tags: [E] easy · [M] medium · [H] hard. Answers in `04-string-methods-2-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
print('banana'.find('a'))
```
- A) `1`
- B) `0`
- C) `2`
- D) `3`

**Q2. [M]** What does this print?
```python
print('banana'.find('z'))
```
- A) `0`
- B) `-1`
- C) An error
- D) `None`

**Q3. [H]** What happens here?
```python
print('banana'.index('z'))
```
- A) `-1`
- B) `0`
- C) An error — `index` raises `ValueError` when the substring is not found
- D) `None`

**Q4. [E]** What does this print?
```python
print('banana'.count('a'))
```
- A) `2`
- B) `1`
- C) `6`
- D) `3`

**Q5. [E]** What does this print?
```python
print('aaa'.replace('a', 'b'))
```
- A) `bbb`
- B) `baa`
- C) `aaa`
- D) `bba`

**Q6. [M]** What does this print?
```python
print('aaaa'.replace('a', 'b', 2))
```
- A) `bbbb`
- B) `bbaa`
- C) `bbba`
- D) `aabb`

**Q7. [M]** What does this print?
```python
print('hello.py'.startswith('hello'))
```
- A) `False`
- B) `hello`
- C) `True`
- D) `.py`

**Q8. [M]** What does this print?
```python
print('hello.py'.endswith('.txt'))
```
- A) `True`
- B) `.py`
- C) An error
- D) `False`

**Q9. [M]** What does this print?
```python
print('12a45'.isdigit())
```
- A) `False`
- B) `True`
- C) `12045`
- D) `3`

**Q10. [H]** What does this print?
```python
print('hello world'.isalpha())
```
- A) `True`
- B) `False`
- C) `hello`
- D) `11`
