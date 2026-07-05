# Recursion — MCQ Set (Q1–Q5)

*Unit 3 · Topic 08. Covers: the meaning of recursion, the base condition, the recursive call, how recursion works through the call stack, recursive factorial and Fibonacci, and the advantages and limitations of recursion.*
*Tags: [E] easy · [M] medium · [H] hard. Answers with explanations follow at the end.*

---

**Q1. [M]** What does this print?
```python
def fact(n):
    if n == 0:
        return 1
    return n * fact(n - 1)

print(fact(4))
```
- A) `4`
- B) `10`
- C) `0`
- D) `24`

**Q2. [M]** What does this print?
```python
def cd(n):
    if n == 0:
        return
    print(n)
    cd(n - 1)

cd(3)
```
- A) `3 2 1`
- B) `1 2 3`
- C) `3 2 1 0`
- D) `0 1 2 3`

**Q3. [H]** What does this print?
```python
def f(n):
    if n == 0:
        return
    f(n - 1)
    print(n)

f(3)
```
- A) `3 2 1`
- B) `1 2 3`
- C) `3 2 1 0`
- D) Nothing

**Q4. [H]** What happens when this runs?
```python
def f(n):
    print(n)
    f(n - 1)

f(3)
```
- A) It prints `3 2 1` then stops
- B) It prints `3` once and stops
- C) It prints `3 2 1 0 …` counting down forever, then crashes with a RecursionError
- D) An error before anything prints

**Q5. [H]** Calling `fib(5)` on the function below returns `5`. How many **total calls** to `fib` happen while computing it?
```python
def fib(n):
    if n < 2:
        return n
    return fib(n - 1) + fib(n - 2)
```
- A) `5`
- B) `6`
- C) `10`
- D) `15`

---

## Answer Key

**Q1 — D.** The calls unwind as 4 × 3 × 2 × 1 × (base case 1) = 24. Each call multiplies `n` by the factorial of `n − 1`, and the base case `fact(0)` returns 1 to stop the chain.

**Q2 — A.** `print(n)` comes **before** the recursive call, so each number prints on the way *down*: 3, then 2, then 1, and the base case `n == 0` returns without printing. Output `3 2 1`.

**Q3 — B.** Here `print(n)` comes **after** the recursive call. So the calls stack all the way down to the base case first, and the printing happens as the stack **unwinds** — in reverse: `1 2 3`. Moving one line changes the order completely; this is the heart of understanding the call stack.

**Q4 — C.** There is **no base condition**, so nothing ever stops the recursion — it keeps calling `f(n - 1)` with smaller and smaller numbers. Python allows only a limited depth of calls, so after printing many lines it stops with a **RecursionError**. Every recursive function needs a base case.

**Q5 — D.** `fib` calls itself twice each time (except at the base cases), and those calls repeat the same work over and over. Counting every call for `fib(5)` gives **15** — far more than the answer of 5. This explosion of repeated calls is exactly why naive recursive Fibonacci is **slow**, and a key limitation of recursion.

---

*Letter spread: A×1 · B×1 · C×1 · D×2. Difficulty: 0 [E] · 2 [M] · 3 [H]. Every answer verified by executing the code.*
