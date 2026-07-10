# Topic 05 — Splitting & Joining · MCQ

*Unit 4 · Strings. Ten questions on `split` (with and without a separator), `join`, and combining them. Key ideas: `split()` with no argument collapses runs of whitespace, while `split(' ')` keeps empty pieces; `join` builds a string from a list of **strings**. Tags: [E] easy · [M] medium · [H] hard. Answers in `05-splitting-joining-mcq-answers.md`.*

---

**Q1. [E]** What does this print?
```python
print('a b c'.split())
```
- A) `['a', 'b', 'c']`
- B) `'a b c'`
- C) `['a b c']`
- D) `'abc'`

**Q2. [M]** What does this print?
```python
print('a,b,c'.split(','))
```
- A) `['a,b,c']`
- B) `['a', 'b', 'c']`
- C) `'a b c'`
- D) `['a', ',', 'b', ',', 'c']`

**Q3. [E]** What does this print?
```python
print(len('one two three'.split()))
```
- A) `1`
- B) `13`
- C) `3`
- D) `2`

**Q4. [M]** What does this print?
```python
print('red-green-blue'.split('-')[1])
```
- A) `red`
- B) `blue`
- C) `green-blue`
- D) `green`

**Q5. [E]** What does this print?
```python
print('-'.join(['a', 'b', 'c']))
```
- A) `a-b-c`
- B) `abc`
- C) `['a-b-c']`
- D) `a - b - c`

**Q6. [M]** What does this print?
```python
print(' '.join('a,b,c'.split(',')))
```
- A) `a,b,c`
- B) `a b c`
- C) `a-b-c`
- D) `['a', 'b', 'c']`

**Q7. [H]** What does this print?
```python
print('a-b-c-d'.split('-', 2))
```
- A) `['a', 'b', 'c', 'd']`
- B) `['a-b', 'c-d']`
- C) `['a', 'b', 'c-d']`
- D) `['a', 'b-c-d']`

**Q8. [H]** What does this print?
```python
print('a   b'.split(' '))
```
- A) `['a', 'b']`
- B) `['a', ' ', 'b']`
- C) `['a   b']`
- D) `['a', '', '', 'b']`

**Q9. [M]** What does this print?
```python
print('a   b'.split())
```
- A) `['a', 'b']`
- B) `['a', '', '', 'b']`
- C) `['a   b']`
- D) `['a', ' ', 'b']`

**Q10. [H]** What happens here?
```python
print('-'.join([1, 2, 3]))
```
- A) `1-2-3`
- B) An error — `join` needs a list of strings, not numbers
- C) `123`
- D) `[1, 2, 3]`
