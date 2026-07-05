# Loops MCQ Bank — Part 1 (Q1–Q54)

*Sections 1–4: `for` & `range()` fundamentals, `while` loops, infinite loops, and loop control (`break` / `continue` / `pass` / loop `else`).*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `loops-mcq-bank-part1-answers.md`.*

---

## Section 1 — `for` & `range()` Fundamentals (Q1–Q18)

**Q1. [E]** What does this print?
```python
for i in range(2, 15, 4):
    print(i)
```
- A) `2 6 10 14`
- B) `2 6 10`
- C) `4 8 12`
- D) `2 6 10 14 18`

**Q2. [E]** What does this print?
```python
for i in range(4):
    print(3)
```
- A) `3` once
- B) `0 1 2 3`
- C) `3 3 3 3`
- D) `3 6 9 12`

**Q3. [E]** Which values does this print?
```python
for i in range(6):
    print(i)
```
- A) `1` to `6`
- B) `0` to `6`
- C) `0` to `5`
- D) Just `6`

**Q4. [E]** What does this print?
```python
for i in range(1, 4):
    print(i * i + 1)
```
- A) `1 4 9`
- B) `2 5 10`
- C) `2 4 6`
- D) `1 2 3`

**Q5. [M]** What does this print?
```python
for i in range(1, 6):
    pass
print(i)
```
- A) `4`
- B) `6`
- C) `5`
- D) An error — `i` no longer exists

**Q6. [M]** What does this print?
```python
for i in range(3):
    i = i + 10
    print(i)
```
- A) `0 1 2`
- B) `10 11 12`
- C) `10` (the loop stops after one pass)
- D) `10 10 10`

**Q7. [M]** How many numbers does this loop print?
```python
for i in range(10, 41, 5):
    print(i)
```
- A) `7`
- B) `6`
- C) `8`
- D) `31`

**Q8. [M]** What does this print?
```python
for i in range(2, 8, -1):
    print(i)
print("End")
```
- A) `2 3 4 5 6 7` then `End`
- B) `7 6 5 4 3 2` then `End`
- C) An error
- D) `End` only

**Q9. [M]** What does this print?
```python
for i in range(2, 11, 2):
    print(i // 2)
```
- A) `1 2 3 4 5`
- B) `2 4 6 8 10`
- C) `1 2 3 4`
- D) `0 1 2 3 4`

**Q10. [M]** What does this print?
```python
for i in range(1, 4):
    print(i, 5 - i)
```
- A) `1 5`, `2 5`, `3 5`
- B) `1 4`, `2 3`, `3 2`
- C) `4 3 2`
- D) `1 4`, `2 3`, `3 2`, `4 1`

**Q11. [M]** With `n = 3`, what does this print?
```python
n = 3
for i in range(n, n * 3):
    print(i, end=" ")
```
- A) `3 6 9`
- B) `3 4 5 6 7 8 9`
- C) `1 2 3`
- D) `3 4 5 6 7 8`

**Q12. [M]** How many times does the body of this loop run?
```python
for i in range(7, 70, 7):
    print(i)
```
- A) `10`
- B) `7`
- C) `9`
- D) `63`

**Q13. [M]** What does this print?
```python
total = 0
for i in range(1, 5):
    total = total + i * i
print(total)
```
- A) `10`
- B) `16`
- C) `55`
- D) `30`

**Q14. [M]** What does this print?
```python
for i in range(3, 0, -1):
    print(i * 10 - i)
```
- A) `27 18 9`
- B) `30 20 10`
- C) `9 18 27`
- D) `29 19 9`

**Q15. [H]** What does this print?
```python
total = 0
for i in range(1, 6):
    total = total + i
    print(total)
```
- A) `1 2 3 4 5`
- B) `1 3 6 10 15`
- C) `15`
- D) `15 15 15 15 15`

**Q16. [H]** Which loop prints exactly `9 7 5 3 1`?
- A) `for i in range(9, 1, -2):`
- B) `for i in range(9, 0, -2):`
- C) `for i in range(1, 10, 2):`
- D) `for i in range(10, 0, -2):`

**Q17. [H]** What does this print?
```python
for i in range(5, 100, 7):
    pass
print(i)
```
- A) `99`
- B) `103`
- C) `96`
- D) `95`

**Q18. [H]** What does this print?
```python
s = 0
for i in range(4):
    s = s + 2 * i + 1
print(s)
```
- A) `16`
- B) `9`
- C) `28`
- D) `13`

---

## Section 2 — `while` Loops (Q19–Q32)

**Q19. [E]** What does this print?
```python
i = 3
while i > 0:
    print(i * 2)
    i = i - 1
```
- A) `3 2 1`
- B) `6 4 2`
- C) `6 4 2 0`
- D) `2 4 6`

**Q20. [E]** What does this print?
```python
n = 17
while n > 5:
    n = n - 4
print(n)
```
- A) `5`
- B) `9`
- C) `1`
- D) `17`

**Q21. [E]** What does this print?
```python
n = 30
count = 0
while n >= 10:
    n = n - 7
    count = count + 1
print(count)
```
- A) `4`
- B) `3`
- C) `2`
- D) `30`

**Q22. [M]** What does this print?
```python
x = 20
while x >= 5:
    x = x - 5
    print(x)
```
- A) `20 15 10 5`
- B) `15 10 5`
- C) `20 15 10 5 0`
- D) `15 10 5 0`

**Q23. [M]** What does this print?
```python
x = 1
while x < 20:
    x = x * 3
    print(x)
```
- A) `1 3 9`
- B) `3 9`
- C) `3 9 27 81`
- D) `3 9 27`

**Q24. [M]** What does this print?
```python
count = 0
n = 100
while n > 1:
    n = n // 2
    count = count + 1
print(count)
```
- A) `50`
- B) `5`
- C) `6`
- D) `7`

**Q25. [M]** What does this print?
```python
n = 7
while n % 5 != 0:
    n = n + 3
print(n)
```
- A) `10`
- B) `7`
- C) `13`
- D) `15`

**Q26. [M]** What does this print?
```python
n = 10
while n > 0:
    n = n - 4
    print(n)
```
- A) `6 2`
- B) `10 6 2`
- C) `6 2 -2`
- D) `6 2 0`

**Q27. [M]** What does this print?
```python
n = 2
while n * n < 50:
    n = n + 2
print(n)
```
- A) `6`
- B) `8`
- C) `10`
- D) `7`

**Q28. [M]** What does this print?
```python
n = 45
s = 0
while n > 0:
    s = s + n % 10
    n = n // 10
print(s)
```
- A) `45`
- B) `54`
- C) `20`
- D) `9`

**Q29. [H]** What does this print?
```python
a = 10
b = 3
while a > 0 and b < 12:
    a = a - 3
    b = b + 4
print(a, b)
```
- A) `4 11`
- B) `1 11`
- C) `-2 19`
- D) `1 15`

**Q30. [H]** What does this print?
```python
a = 1
b = 1
while b < 20:
    t = a + b
    a = b
    b = t
    print(b)
```
- A) `2 3 5 8 13 21`
- B) `2 3 5 8 13`
- C) `1 2 3 5 8 13`
- D) `1 1 2 3 5 8 13 21`

**Q31. [H]** What does this print?
```python
i = 1
total = 0
while total <= 20:
    total = total + i * i
    i = i + 1
print(i, total)
```
- A) `4 14`
- B) `5 30`
- C) `4 30`
- D) `5 14`

**Q32. [H]** What does this print?
```python
n = 1
while n < 100:
    n = n * n + 1
print(n)
```
- A) `101`
- B) `26`
- C) `677`
- D) `2`

---

## Section 3 — Infinite Loops (Q33–Q38)

**Q33. [E]** Which line, added as the last line of the body, makes this loop stop?
```python
n = 8
while n > 0:
    print(n)
```
- A) `n = n + 2`
- B) `n = n - 2`
- C) `print(n - 2)`
- D) `n == n - 2`

**Q34. [M]** What happens when this runs?
```python
while True:
    print("hi")
    if 5 > 10:
        break
```
- A) Prints `hi` once
- B) Prints nothing
- C) An error
- D) Prints `hi` forever

**Q35. [M]** What happens when this runs?
```python
x = 5
while x < 100:
    x = x * 1
```
- A) It ends after one pass
- B) It ends when `x` reaches 100
- C) It runs forever — `x` never changes
- D) An error

**Q36. [M]** This loop never ends. Which replacement for the body line fixes it?
```python
i = 1
while i < 50:
    total = total + i
```
- A) `total = total + 1`
- B) `i = i * 2`
- C) `print(i)`
- D) `total = i`

**Q37. [H]** Which of these loops never ends?
- A)
  ```python
  i = 0
  while i < 5:
      i = i + 1
  ```
- B)
  ```python
  i = 10
  while i > 0:
      i = i - 2
  ```
- C)
  ```python
  i = 0
  while i != 7:
      i = i + 2
  ```
- D)
  ```python
  i = 5
  while i <= 5:
      i = i + 1
  ```

**Q38. [H]** What happens when this runs?
```python
n = 3
while n % 2 == 1:
    n = n + 2
```
- A) It stops when `n` reaches 4
- B) It stops after one pass
- C) It stops when `n` becomes even
- D) It runs forever — adding 2 keeps `n` odd

---

## Section 4 — `break`, `continue`, `pass`, loop `else` (Q39–Q54)

**Q39. [E]** In a `while True:` loop, which statement is the only one that can end the loop?
- A) `pass`
- B) `continue`
- C) `break`
- D) `else`

**Q40. [E]** What does this print?
```python
n = 0
while n < 3:
    n = n + 1
    if n == 2:
        pass
    print(n)
```
- A) `1 2 3`
- B) `1 3`
- C) `1 2`
- D) `3`

**Q41. [E]** What does this print?
```python
total = 0
for i in range(4):
    if i == 1:
        pass
    total = total + i
print(total)
```
- A) `5`
- B) `0`
- C) `3`
- D) `6`

**Q42. [E]** What does this print?
```python
n = 3
while n > 0:
    n = n - 1
else:
    print(n, "end")
```
- A) `0 end`
- B) `3 end`
- C) `1 end`
- D) Nothing — `else` needs a `break`

**Q43. [M]** What does this print?
```python
total = 0
for i in range(1, 7):
    if i % 2 == 0:
        continue
    total = total + i
print(total)
```
- A) `21`
- B) `12`
- C) `9`
- D) `0`

**Q44. [M]** What does this print?
```python
for i in range(1, 6):
    if i == 3:
        continue
    print(i * i)
```
- A) `1 4 9 16 25`
- B) `1 4 16 25`
- C) `1 4`
- D) `16 25`

**Q45. [M]** What does this print?
```python
for i in range(1, 6):
    print(i)
    if i == 3:
        break
```
- A) `1 2`
- B) `1 2 3`
- C) `1 2 3 4 5`
- D) `3`

**Q46. [M]** What does this print?
```python
n = 1
while True:
    n = n * 2
    if n > 50:
        break
    print(n)
```
- A) `2 4 8 16 32`
- B) `2 4 8 16 32 64`
- C) `1 2 4 8 16 32`
- D) `64`

**Q47. [M]** What does this print?
```python
n = 7
while n < 10:
    if n % 4 == 0:
        print("Found")
        break
    n = n + 1
else:
    print("None")
```
- A) `None`
- B) `Found` then `None`
- C) Nothing
- D) `Found` only

**Q48. [M]** What does this print?
```python
p = 1
for i in range(1, 6):
    if i == 4:
        continue
    p = p * i
print(p)
```
- A) `120`
- B) `24`
- C) `30`
- D) `6`

**Q49. [M]** What does this print?
```python
for i in range(10, 0, -1):
    if i * i < 50:
        break
    print(i)
```
- A) `10 9 8`
- B) `10 9 8 7`
- C) `10 9`
- D) `7 6 5 4 3 2 1`

**Q50. [H]** What does this print?
```python
for i in range(3):
    if i == 1:
        continue
    print(i)
else:
    print("Done")
```
- A) `0 2` then `Done`
- B) `0 2` only
- C) `0 1 2` then `Done`
- D) `Done` only

**Q51. [H]** What does this print?
```python
total = 0
for i in range(1, 10):
    total = total + i
    if total > 10:
        break
print(i, total)
```
- A) `4 10`
- B) `5 15`
- C) `5 10`
- D) `9 45`

**Q52. [H]** What does this print?
```python
n = 0
s = 0
while n < 6:
    n = n + 1
    if n % 3 == 0:
        continue
    s = s + n
print(s)
```
- A) `21`
- B) `9`
- C) `18`
- D) `12`

**Q53. [H]** What does this print?
```python
s = 0
for i in range(1, 11):
    if i % 2 == 0:
        continue
    if i > 7:
        break
    s = s + i
print(s)
```
- A) `25`
- B) `9`
- C) `16`
- D) `10`

**Q54. [H]** What does this print?
```python
total = 0
for i in range(1, 8):
    if i % 3 == 0:
        total = total + 10
    else:
        total = total + 1
    if total > 15:
        break
print(i, total)
```
- A) `3 12`
- B) `6 24`
- C) `7 25`
- D) `6 15`

---

*End of Part 1 — 54 questions. Difficulty: 12 [E] · 27 [M] · 15 [H]. Every answer verified by executing the code.*
