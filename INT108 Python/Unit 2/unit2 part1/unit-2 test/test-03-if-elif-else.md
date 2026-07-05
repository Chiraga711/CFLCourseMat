# Test 3: The `if-elif-else` Statement

*Conditional Statements series · Test for Lesson 3*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- Use the `if-elif-else` statement for this test (multi-way choices) — but no `and`/`or`/`not` or nested `if`s yet.
- For decimal input, use `float(input(...))`; for whole-number input, use `int(input(...))`.
- A reminder: Python runs the **first** matching branch and skips the rest, so the **order** of conditions matters.
- The answer key is in a separate file: `answer-keys/answers-03-if-elif-else.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What does this print?
```python
wind = 35.0
if wind < 12.0:
    print("Calm")
elif wind < 30.0:
    print("Breezy")
elif wind < 50.0:
    print("Windy")
else:
    print("Stormy")
```
- A) `Calm`
- B) `Breezy`
- C) `Windy`
- D) `Stormy`

**Q2.** What does this print?
```python
ph = 7.0
if ph < 7.0:
    print("Acidic")
elif ph == 7.0:
    print("Neutral")
else:
    print("Basic")
```
- A) `Acidic`
- B) `Neutral`
- C) `Basic`
- D) An error

**Q3.** What does this print?
```python
score = 5
if score > 10:
    print("High")
elif score > 8:
    print("Medium")
```
- A) `High`
- B) `Medium`
- C) An error
- D) Nothing

**Q4.** What does this print?
```python
income = 600000
if income <= 250000:
    rate = 0
elif income <= 500000:
    rate = 5
else:
    rate = 20
print(rate)
```
- A) `20`
- B) `0`
- C) `5`
- D) `25`

**Q5.** In this code, which result can a student **never** get?
```python
if marks >= 50:
    print("Pass")
elif marks >= 80:
    print("Distinction")
else:
    print("Fail")
```
- A) `Pass`
- B) `Distinction`
- C) `Fail`
- D) All of them can happen

---

## Part B — Coding Problems (5)

**P1 — Earthquake Severity.**
Ask for an earthquake's magnitude on the Richter scale (a decimal). Print its severity: below 4.0 → `Minor`, below 5.0 → `Light`, below 6.0 → `Moderate`, below 7.0 → `Strong`, otherwise → `Major`.

**P2 — Income Tax.**
A simplified tax system works in brackets: income up to ₹250000 pays no tax; up to ₹500000 pays 5%; up to ₹1000000 pays 20%; above that pays 30%. Ask for a person's annual income, then **calculate and print the tax owed**. (Each bracket charges its flat rate on the whole income — a simplified version of real tax.)

**P3 — Air Quality Advisory.**
Ask for the Air Quality Index (AQI) as a whole number. Print the advisory: ≤ 50 → `Good`, ≤ 100 → `Moderate`, ≤ 150 → `Unhealthy for sensitive groups`, ≤ 200 → `Unhealthy`, otherwise → `Hazardous`.

**P4 — Service Tip Calculator.**
A diner rates the service from 1 to 10. The tip percentage depends on the rating: 9 or 10 → 25%, 7 or 8 → 20%, 5 or 6 → 10%, below 5 → 5%. Ask for the bill amount and the service rating, then **calculate and print the tip**.

**P5 — Typing Speed Level.**
Ask for a typing speed in words per minute (a whole number). Print the level: below 20 → `Beginner`, below 40 → `Average`, below 60 → `Fast`, otherwise → `Expert`.

---

*End of test. Check your work against the separate answer key.*
