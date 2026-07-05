# Test 1: The `if` Statement

*Conditional Statements series · Test for Lesson 1*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- Use only the single `if` statement for this test (no `else` or `elif` yet) — along with variables, numbers, and comparisons.
- Some values are decimals. To read a decimal number from the user, use `float(input(...))` — it works just like `int(input(...))` but keeps the decimal part.
- Currency is shown as ₹, but you only need to print the numbers.
- The answer key is in a separate file: `answer-keys/answers-01-if-statement.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
total = 50.0
if total > 40.0:
    total = total + 10.0
print(total)
```
- A) `50.0`
- B) `60.0`
- C) `40.0`
- D) `10.0`

**Q2.** What does this print?
```python
fee = 100.0
if fee > 200.0:
    fee = fee + 25.0
print(fee)
```
- A) `125.0`
- B) `0.0`
- C) `100.0`
- D) An error

**Q3.** What does this print?
```python
print(7.0 == 7)
```
- A) `True`
- B) `False`
- C) An error
- D) `7`

**Q4.** Which line correctly starts an `if` that checks whether `temperature` is at least 36.5?
- A) `if temperature >= 36.5:`
- B) `if temperature => 36.5:`
- C) `if temperature >= 36.5`
- D) `if (temperature) > = 36.5:`

**Q5.** What does this print?
```python
x = 3.0
if x > 5.0:
    print("big")
y = x * 2
print(y)
```
- A) `big` then `6.0`
- B) `6.0`
- C) `big`
- D) Nothing

---

## Part B — Coding Problems (5)

**P1 — Toll Plaza Surcharge.**
A toll plaza charges trucks a base toll of ₹100.00. A truck heavier than 10.0 tons pays an extra surcharge of ₹50.50. Ask for a truck's weight in tons, then calculate and print the **total toll**. (Start the toll at 100.00, add the surcharge only if the truck is overweight, and print the total either way.)

**P2 — Shopping Discount.**
A shop gives a 10% discount when the bill is ₹2000.00 or more. Ask for the bill amount. If it qualifies, calculate the **final amount to pay** (after the 10% is taken off) and print it. At the very end, always print `Thank you for shopping!`.

**P3 — Library Late Fine.**
A library charges ₹2.50 for each day a book is late. Ask how many days late a book is. If it is late (more than 0 days), calculate the **total fine** and print it.

**P4 — Speed Camera Fine.**
The speed limit is 60.0 km/h, with a fine of ₹500.00 for every km/h over the limit. Ask for a car's speed. If it is over the limit, calculate the **fine** (the number of km/h over × ₹500.00) and print it.

**P5 — Preheat the Oven.**
A recipe needs the oven at 180.0 °C. Ask for the current oven temperature. If it is still below 180.0, calculate **how many more degrees** it needs to heat up, and print that number.

---

*End of test. Check your work against the separate answer key.*
