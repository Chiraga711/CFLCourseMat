# Return Values — MCQ Set (Q1–Q5)

*Unit 3 · Topic 05. Covers: functions with and without a return value, the difference between `print()` and `return`, `None`, and returning multiple values.*
*Tags: [E] easy · [M] medium · [H] hard. Answers with explanations follow at the end.*

---

**Q1. [M]** What does this program display on the screen?
```python
def add(a, b):
    return a + b

add(2, 3)
```
- A) `5`
- B) Nothing
- C) `None`
- D) An error

**Q2. [H]** What does this print?
```python
def show(n):
    print(n * 2)

print(show(5))
```
- A) `10`
- B) `10` then `10`
- C) `None`
- D) `10` then `None`

**Q3. [M]** What does this print?
```python
def f(n):
    if n > 0:
        return "positive"
    return "not positive"

print(f(7))
```
- A) `positive`
- B) `not positive`
- C) `positive` then `not positive`
- D) `7`

**Q4. [H]** What does this print?
```python
def stats(a, b):
    return a + b, a * b

s, p = stats(3, 4)
print(s, p)
```
- A) `12 7`
- B) `7` then `12`
- C) `7 12`
- D) An error — a function can only return one value

**Q5. [M]** What does this print?
```python
def sq(n):
    return n * n

print(sq(3) + sq(4))
```
- A) `12`
- B) `25`
- C) `9 16`
- D) `sq(3) + sq(4)`

---

## Answer Key

**Q1 — B.** The function **returns** 5, but the result is never printed or stored, so nothing appears on screen. Returning a value is not the same as displaying it — that's the heart of `return` vs `print`.

**Q2 — D.** Two things happen. Inside, `print(n * 2)` displays `10`. But `show` has no `return`, so it hands back **`None`** — and the outer `print(show(5))` displays that: `10` then `None`. A function that only prints still returns `None`.

**Q3 — A.** `return` **exits the function immediately**. Since 7 > 0, it returns `"positive"` and the second `return` never runs. Only `positive` prints.

**Q4 — C.** A function **can** return several values at once (separated by commas), and `s, p = stats(3, 4)` unpacks them: `s` gets 3 + 4 = 7, `p` gets 3 × 4 = 12. Prints `7 12`.

**Q5 — B.** Because `sq` **returns** its result, the value can be used in an expression: `sq(3)` is 9, `sq(4)` is 16, and 9 + 16 = 25. This is exactly what a returned value makes possible and a printed one does not.

---

*Letter spread: A×1 · B×2 · C×1 · D×1. Difficulty: 0 [E] · 3 [M] · 2 [H]. Every answer verified by executing the code.*
