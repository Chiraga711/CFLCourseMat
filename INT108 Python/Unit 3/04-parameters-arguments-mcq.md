# Parameters & Arguments — MCQ Set (Q1–Q5)

*Unit 3 · Topic 04. Covers: parameters vs arguments, positional arguments, keyword arguments, and default arguments.*
*Tags: [E] easy · [M] medium · [H] hard. Answers with explanations follow at the end.*

---

**Q1. [M]** What does this print?
```python
def subtract(a, b):
    print(a - b)

subtract(3, 10)
```
- A) `7`
- B) `13`
- C) `-7`
- D) An error

**Q2. [E]** In the definition `def greet(name):`, the word `name` is called a:
- A) Parameter
- B) Argument
- C) Return value
- D) Keyword

**Q3. [H]** What does this print?
```python
def power(base, exp):
    print(base, exp)

power(exp=3, base=2)
```
- A) `3 2`
- B) `2 3`
- C) An error — arguments are in the wrong order
- D) `2 2`

**Q4. [M]** What does this print?
```python
def greet(name, msg="Hi"):
    print(msg, name)

greet("Sam")
```
- A) `Sam Hi`
- B) An error — `msg` was not given
- C) `Hi`
- D) `Hi Sam`

**Q5. [H]** Why does this definition cause an error?
```python
def f(a=1, b):
    print(a + b)
```
- A) A function can have at most one parameter with a default
- B) `a` and `b` cannot both be numbers
- C) A parameter with a default cannot come **before** one without a default
- D) Default values must be strings

---

## Answer Key

**Q1 — C.** Arguments fill parameters **in order**: `a` becomes 3, `b` becomes 10, so 3 − 10 = −7. Order matters — swapping the arguments changes the answer.

**Q2 — A.** A name listed inside the parentheses of a `def` is a **parameter** — the placeholder. The actual value passed in when you *call* the function is the **argument**.

**Q3 — B.** **Keyword arguments** name their target, so order no longer matters: `base` gets 2 and `exp` gets 3 regardless of the order they're written. Prints `2 3`.

**Q4 — D.** `msg` has a **default** of `"Hi"`, so calling `greet("Sam")` uses it: `Sam` fills `name`, `msg` stays `"Hi"`, output `Hi Sam`.

**Q5 — C.** A parameter **with** a default cannot appear before one **without** a default — Python can't tell which argument a later value belongs to. Writing `def f(a, b=1):` is the correct order.

---

*Letter spread: A×1 · B×1 · C×2 · D×1. Difficulty: 1 [E] · 2 [M] · 2 [H]. Every answer verified by executing the code.*
