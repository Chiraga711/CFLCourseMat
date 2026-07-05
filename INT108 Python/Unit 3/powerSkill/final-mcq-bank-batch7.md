# Functions & Recursion — Final MCQ Bank, Batch 7 (Q286–Q307)

*Bonus set: Fill-in-the-Blank, Default Arguments & Keyword Arguments. These test whether you can **choose the right code** (not just trace output) — completing a blank, picking a valid definition or call, and reasoning about defaults and keyword binding.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch7-answers.md`.*

---

## Fill in the Blank

**Q286. [E]** Fill in the blank so the program prints `10`.
```python
def add(a, b):
    return ______

print(add(4, 6))
```
- A) `a + b`
- B) `a - b`
- C) `a * b`
- D) `a / b`

**Q287. [E]** Fill in the blank so the program prints `25`.
```python
def square(n):
    return ______

print(square(5))
```
- A) `n + n`
- B) `n * n`
- C) `n - n`
- D) `n // n`

**Q288. [M]** Fill in the blank so the program prints `True`.
```python
def check_even(n):
    return ______

print(check_even(8))
```
- A) `n % 2 == 1`
- B) `n // 2 == 0`
- C) `n % 2 == 0`
- D) `n * 2 == 0`

**Q289. [E]** Fill in the blank so the program prints `9`.
```python
def greater(a, b):
    if a > b:
        return ______
    else:
        return b

print(greater(9, 4))
```
- A) `b`
- B) `a + b`
- C) `a - b`
- D) `a`

**Q290. [M]** Fill in the blank so the program prints `10`.
```python
def total(n):
    s = 0
    for i in range(1, n + 1):
        s = s + ______
    return s

print(total(4))
```
- A) `i`
- B) `1`
- C) `n`
- D) `s`

**Q291. [M]** Fill in the blank so the program prints `3`.
```python
def count_even(n):
    count = 0
    for i in range(1, n + 1):
        if i % 2 == 0:
            count = count + ______
    return count

print(count_even(6))
```
- A) `i`
- B) `1`
- C) `2`
- D) `n`

**Q292. [M]** Fill in the blank so the program prints `True`.
```python
def divisible(a, b):
    return ______

print(divisible(12, 4))
```
- A) `a // b == 0`
- B) `a * b == 0`
- C) `a % b == 0`
- D) `a + b == 0`

**Q293. [E]** Fill in the blank so the program prints `Negative or Zero`.
```python
def result(n):
    if n > 0:
        return "Positive"
    else:
        return ______

print(result(-5))
```
- A) `"Positive"`
- B) `n`
- C) `0`
- D) `"Negative or Zero"`

**Q294. [M]** Fill in the blank so the program prints `10`.
```python
def multiply_sum(a, b):
    return (a + b) * ______

print(multiply_sum(2, 3))
```
- A) `2`
- B) `1`
- C) `3`
- D) `5`

**Q295. [H]** Fill in the blank so the program prints `10`.
```python
def nested_sum(n):
    total = 0
    for i in range(1, n + 1):
        for j in range(1, i + 1):
            total = total + ______
    return total

print(nested_sum(3))
```
- A) `i`
- B) `j`
- C) `1`
- D) `n`

---

## Default Arguments

**Q296. [M]** What does this print?
```python
def greet(name="Student"):
    return "Hello " + name

print(greet())
```
- A) `Hello`
- B) `Student Hello`
- C) `Hello Student`
- D) An error

**Q297. [M]** What does this print?
```python
def calculate(a, b=10):
    if a > b:
        return a - b
    else:
        return a + b

print(calculate(7))
```
- A) `3`
- B) `7`
- C) `10`
- D) `17`

**Q298. [M]** What does this print?
```python
def calculate(a, b=10):
    if a > b:
        return a - b
    else:
        return a + b

print(calculate(15))
```
- A) `5`
- B) `10`
- C) `15`
- D) `25`

**Q299. [M]** What does this print?
```python
def total(a, b=1, c=2):
    return a + b + c

print(total(5))
```
- A) `5`
- B) `8`
- C) `6`
- D) `7`

**Q300. [H]** What does this print?
```python
def total(a, b=1, c=2):
    return a + b + c

print(total(5, 4))
```
- A) `7`
- B) `9`
- C) `11`
- D) `12`

---

## Keyword Arguments

**Q301. [H]** What does this print?
```python
def result(a, b, c):
    return a + b * c

print(result(c=2, a=3, b=4))
```
- A) `14`
- B) `20`
- C) An error
- D) `11`

**Q302. [M]** What does this print?
```python
def show(name, age):
    return name + " is " + str(age)

print(show(age=20, name="Ravi"))
```
- A) `Ravi is 20`
- B) `20 is Ravi`
- C) `name is age`
- D) An error

**Q303. [H]** What does this print?
```python
def calc(a, b, c):
    if a > b:
        return a + c
    else:
        return b + c

print(calc(b=8, c=2, a=5))
```
- A) `7`
- B) `10`
- C) `13`
- D) `15`

**Q304. [M]** What does this print?
```python
def area(length, width):
    return length * width

print(area(width=5, length=4))
```
- A) `9`
- B) `45`
- C) `20`
- D) An error

---

## Which Is Correct?

**Q305. [M]** Which function **definition** is valid?
- A) `def fun(a=5, b):`
- B) `def fun(a=5, b=10, c):`
- C) `def fun(a=2, b):`
- D) `def fun(a, b=5):`

**Q306. [M]** Which function **call** is valid for this definition?
```python
def add(a, b):
    return a + b
```
- A) `add(a=4, b=5)`
- B) `add(x=4, y=5)`
- C) `add(a=4, y=5)`
- D) `add(4, x=5)`

**Q307. [E]** Which statement about keyword arguments is true?
- A) They must be written in the same order as the parameters
- B) They cannot be used with numbers
- C) They use the parameter names when calling the function
- D) They are used only with loops

---

*End of Batch 7 — Q286–Q307. Difficulty: 5 [E] · 13 [M] · 4 [H]. Every answer verified by executing the code.*