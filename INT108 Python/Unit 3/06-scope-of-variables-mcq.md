# Scope of Variables — MCQ Set (Q1–Q5)

*Unit 3 · Topic 06. Covers: local variables, global variables, the lifetime of variables, and common scope mistakes.*
*Tags: [E] easy · [M] medium · [H] hard. Answers with explanations follow at the end.*

---

**Q1. [M]** What does this print?
```python
x = 10

def f():
    x = 99

f()
print(x)
```
- A) `10`
- B) `99`
- C) Nothing
- D) An error

**Q2. [H]** What does this print?
```python
n = 5

def f(n):
    print(n)

f(20)
print(n)
```
- A) `5` then `20`
- B) `20` then `20`
- C) `20` then `5`
- D) `5` then `5`

**Q3. [M]** What does this print?
```python
count = 7

def show():
    print(count)

show()
```
- A) `0`
- B) `7`
- C) An error — `count` is not defined inside the function
- D) Nothing

**Q4. [H]** What happens when this runs?
```python
total = 0

def add():
    print(total)
    total = total + 1

add()
```
- A) It prints `0`, then `total` becomes 1
- B) It prints `1`
- C) It prints `0` then `1`
- D) An error — `total` is used before it is assigned inside the function

**Q5. [H]** What happens when this runs?
```python
def f():
    y = 42

f()
print(y)
```
- A) It prints `42`
- B) It prints `0`
- C) An error — `y` exists only inside `f` and is gone after the call
- D) It prints nothing

---

## Answer Key

**Q1 — A.** The `x = 99` inside `f` creates a **new local variable** that vanishes when the function ends. The global `x` is untouched, so `10` prints. Assigning inside a function does not change a same-named global.

**Q2 — C.** The parameter `n` is **local** and shadows the global `n` only *inside* the function: `f(20)` prints `20`. Outside, the global `n` is still `5`. Prints `20` then `5`.

**Q3 — B.** **Reading** a global from inside a function is allowed, so `show()` sees `count` and prints `7`. (Problems only arise when you try to *assign* to it — see Q4.)

**Q4 — D.** Because `total` is **assigned** somewhere in the function, Python treats it as local *throughout* the function — so the earlier `print(total)` tries to read a local that has no value yet. This is the classic **UnboundLocalError**: reading, then assigning, a global of the same name.

**Q5 — C.** `y` is a **local** variable — it lives only while `f` is running and is gone afterward. Trying to use it outside is a **NameError**. This is the lifetime rule: locals do not survive the call.

---

*Letter spread: A×1 · B×1 · C×2 · D×1. Difficulty: 0 [E] · 2 [M] · 3 [H]. Every answer verified by executing the code.*
