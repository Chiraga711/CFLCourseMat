# Functions & Recursion — Final MCQ Bank, Batch 1 (Q1–Q50)

*Unit 3 final revision bank. Batch 1 of 4. Covers Topic 01 (Introduction), Topic 02 (Built-in Functions), and operators used inside functions.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch1-answers.md`.*

---

## Topic 01 — Introduction to Functions

**Q1. [E]** What is a function, in the simplest terms?
- A) A named block of code that can be run whenever you call it
- B) A variable that stores many values
- C) A loop that repeats code automatically
- D) A built-in Python error

**Q2. [E]** Which keyword is used to create (define) a function in Python?
- A) `function`
- B) `def`
- C) `define`
- D) `func`

**Q3. [M]** Writing the same block of code three times instead of using a function mainly causes which problem?
- A) The program cannot compile
- B) Python runs out of memory
- C) A bug must be fixed in three separate places instead of one
- D) The output prints three times

**Q4. [M]** A team fixes one line inside a function and every place that uses it is corrected at once. This advantage is called:
- A) Code reusability
- B) Faster execution
- C) Keyword arguments
- D) Easy debugging

**Q5. [M]** Reading `if is_weekend(day):` instantly tells you what the line checks, without seeing the function's code. This advantage is called:
- A) Better readability
- B) Modularity
- C) Recursion
- D) Easy debugging

**Q6. [M]** Breaking one large program into small, separate, named functions each with a single job is called:
- A) Reusability
- B) Modularity
- C) Readability
- D) Iteration

**Q7. [M]** How many times does the body of `t` run here?
```python
def t():
    print('x')

t()
t()
```
- A) 1 time — a body runs only once
- B) 0 times — nothing is returned
- C) 2 times — once per call
- D) 3 times — including the definition

**Q8. [E]** Which of these is a **built-in** function you have used since your first programs?
- A) `is_prime()`
- B) `digit_sum()`
- C) `grade()`
- D) `print()`

**Q9. [M]** What does this program print?
```python
def f():
    print('hi')

print('done')
```
- A) `done`
- B) `hi` then `done`
- C) `hi`
- D) `done` then `hi`

**Q10. [H]** Even a function that is called only **once** can still be worth writing. Why?
- A) It runs faster than repeated code
- B) It can improve modularity and readability, not just save typing
- C) Python requires every program to have functions
- D) It automatically removes all bugs

---

## Topic 02 — Built-in Functions

**Q11. [E]** What is `int(12.7)`?
- A) `13`
- B) `12.7`
- C) `12`
- D) `12.0`

**Q12. [E]** What is `float(8)`?
- A) `8`
- B) `0.8`
- C) An error
- D) `8.0`

**Q13. [M]** What is `len(str(7))`?
- A) `1`
- B) `7`
- C) `0`
- D) An error

**Q14. [E]** What is `int("55")`?
- A) `"55"`
- B) `55`
- C) `5`
- D) An error

**Q15. [H]** What does `int("9.9")` produce?
- A) `9`
- B) `10`
- C) An error
- D) `9.9`

**Q16. [H]** What is `round(6.5)`?
- A) `7`
- B) `6.5`
- C) An error
- D) `6`

**Q17. [H]** What is `round(8.5)`?
- A) `9`
- B) `8.5`
- C) An error
- D) `8`

**Q18. [H]** What is `round(2.375, 2)`?
- A) `2.37`
- B) `2.4`
- C) `2.375`
- D) `2.38`

**Q19. [E]** What is `max(7, 2, 7)`?
- A) `2`
- B) `16`
- C) `14`
- D) `7`

**Q20. [M]** What is `min(-5, -1)`?
- A) `-5`
- B) `-1`
- C) `5`
- D) `1`

**Q21. [M]** What is `sum([5, 15])`?
- A) `515`
- B) `20`
- C) `[20]`
- D) An error

**Q22. [H]** What does `sum(1, 2)` produce?
- A) `3`
- B) `12`
- C) An error
- D) `1`

**Q23. [E]** What is `len("code")`?
- A) `4`
- B) `5`
- C) `3`
- D) An error

**Q24. [M]** What is `len("a b")` (note the space)?
- A) `2`
- B) `3`
- C) `4`
- D) An error

**Q25. [H]** What does `len(100)` produce?
- A) `3`
- B) `100`
- C) An error
- D) `0`

**Q26. [E]** What does `print(type(4.0))` show?
- A) `<class 'float'>`
- B) `<class 'int'>`
- C) `<class 'str'>`
- D) `4.0`

**Q27. [M]** What does `print(type('4'))` show?
- A) `<class 'int'>`
- B) `<class 'str'>`
- C) `<class 'float'>`
- D) `<class 'char'>`

**Q28. [M]** What does `print(type(8 // 2))` show?
- A) `<class 'float'>`
- B) `<class 'str'>`
- C) `<class 'int'>`
- D) `4`

**Q29. [H]** What does `print(type(8 / 2))` show?
- A) `<class 'int'>`
- B) `<class 'str'>`
- C) `4.0`
- D) `<class 'float'>`

**Q30. [M]** After `x = input()`, no matter what the user types, `type(x)` is:
- A) `<class 'str'>`
- B) `<class 'int'>`
- C) `<class 'float'>`
- D) It depends on what was typed

**Q31. [M]** What is `max(3, 9.0)`?
- A) `9`
- B) `9.0`
- C) `3`
- D) An error

**Q32. [M]** What is `round(4.0)`?
- A) `4.0`
- B) `5`
- C) `4`
- D) An error

**Q33. [M]** What is `int(-2.9)`?
- A) `-2`
- B) `-3`
- C) `2`
- D) `3`

**Q34. [M]** What is `len(str(12))`?
- A) `12`
- B) `2`
- C) `1`
- D) An error

**Q35. [H]** What does `round(0.1 + 0.2, 1)` give?
- A) `0.30000000000000004`
- B) `0.4`
- C) `0.3`
- D) An error

**Q36. [H]** What is `max(min(9, 4), 6)`?
- A) `4`
- B) `9`
- C) `3`
- D) `6`

---

## Operators Inside Functions

**Q37. [M]** What does this print?
```python
def f(a, b):
    return a % b

print(f(17, 5))
```
- A) `3`
- B) `2`
- C) `3.4`
- D) `12`

**Q38. [M]** What does this print?
```python
def f(a, b):
    return a // b

print(f(17, 5))
```
- A) `2`
- B) `3.4`
- C) `3`
- D) `4`

**Q39. [M]** What does this print?
```python
def f(n):
    return n % 2 == 0

print(f(8))
```
- A) `False`
- B) `0`
- C) `8`
- D) `True`

**Q40. [H]** What does this print?
```python
def f(a, b):
    return a > b and a % 2 == 0

print(f(8, 3))
```
- A) `True`
- B) `False`
- C) `8`
- D) An error

**Q41. [H]** What does this print?
```python
def f(a, b, c):
    return a < b or b > c

print(f(2, 5, 1))
```
- A) `False`
- B) `True`
- C) `5`
- D) An error

**Q42. [M]** What does this print?
```python
def f(x):
    return not x > 10

print(f(4))
```
- A) `False`
- B) `4`
- C) `True`
- D) An error

**Q43. [M]** What does this print?
```python
def f(a, b):
    return a + b * 2

print(f(3, 4))
```
- A) `11`
- B) `14`
- C) `10`
- D) `24`

**Q44. [M]** What does this print?
```python
def f(a, b):
    return (a + b) * 2

print(f(3, 4))
```
- A) `11`
- B) `14`
- C) `10`
- D) `24`

**Q45. [H]** What does this print?
```python
def grade(m):
    return m >= 50 and m < 75

print(grade(60))
```
- A) `False`
- B) `60`
- C) `True`
- D) `C`

**Q46. [M]** What does this print?
```python
def f(n):
    return n % 3 == 0 or n % 5 == 0

print(f(9))
```
- A) `True`
- B) `False`
- C) `9`
- D) `3`

**Q47. [H]** What does this print?
```python
def f(a, b):
    return a == b or a == 0

print(f(0, 5))
```
- A) `False`
- B) `True`
- C) `0`
- D) An error

**Q48. [H]** What does this print?
```python
def f(x, y):
    return x // y + x % y

print(f(23, 5))
```
- A) `8`
- B) `4`
- C) `3`
- D) `7`

**Q49. [M]** What does this print?
```python
def f(n):
    return 10 % n == 0

print(f(4))
```
- A) `False`
- B) `True`
- C) `2`
- D) `4`

**Q50. [M]** What does this print?
```python
def f(a, b):
    return not (a > b)

print(f(3, 8))
```
- A) `False`
- B) `3`
- C) `8`
- D) `True`

---

*End of Batch 1 — Q1–Q50. Difficulty: 9 [E] · 26 [M] · 15 [H]. Every answer verified by executing the code.*