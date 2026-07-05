# Built-in Functions — MCQ Set (Q1–Q50)

*Unit 3 · Topic 02. Covers: `int()`, `float()`, `str()`, `type()`, `input()`, `round()`, `max()`, `min()`, `sum()`, `len()`, `print()`.*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `02-built-in-functions-mcq-answers.md`.*

---

## Section A — Conversions: `int()`, `float()`, `str()` (Q1–Q12)

**Q1. [E]** What is `int(7.9)`?
- A) `8`
- B) `7`
- C) `7.9`
- D) `7.0`

**Q2. [E]** What is `float(5)`?
- A) `5`
- B) `0.5`
- C) `5.0`
- D) An error

**Q3. [M]** What kind of value does `str(45)` produce?
- A) The text `"45"`
- B) The number `45`
- C) The float `45.0`
- D) An error

**Q4. [M]** What is `int(-3.7)`?
- A) `-4`
- B) `4`
- C) `3`
- D) `-3`

**Q5. [M]** What is `int("42")`?
- A) `"42"`
- B) `42`
- C) An error
- D) `42.0`

**Q6. [H]** What does `int("4.5")` produce?
- A) `4`
- B) `4.5`
- C) An error
- D) `5`

**Q7. [M]** What is `float("3.5")`?
- A) `3.5`
- B) `"3.5"`
- C) `3`
- D) An error

**Q8. [M]** What is `int(4.99)`?
- A) `5`
- B) `4.99`
- C) An error
- D) `4`

**Q9. [M]** What does `print(float(7))` show?
- A) `7`
- B) `7.0`
- C) `7.00`
- D) An error

**Q10. [H]** What is `int(float("7.8"))`?
- A) `7`
- B) `7.8`
- C) `8`
- D) An error

**Q11. [M]** What is `len(str(3.0))`?
- A) `1`
- B) `2`
- C) `3`
- D) An error

**Q12. [M]** Which of these conversions **fails** with an error?
- A) `float("10")`
- B) `str(10)`
- C) `int(10.0)`
- D) `int("ten")`

---

## Section B — `type()` and `input()` (Q13–Q20)

**Q13. [E]** What does `print(type(5))` show?
- A) `<class 'int'>`
- B) `<class 'float'>`
- C) `<class 'str'>`
- D) `5`

**Q14. [M]** What does `print(type(5.0))` show?
- A) `<class 'int'>`
- B) `<class 'number'>`
- C) `<class 'float'>`
- D) `<class 'str'>`

**Q15. [M]** What does `print(type("5"))` show?
- A) `<class 'int'>`
- B) `<class 'str'>`
- C) `<class 'float'>`
- D) `<class 'text'>`

**Q16. [H]** What does `print(type(7 / 1))` show?
- A) `<class 'int'>`
- B) `<class 'str'>`
- C) It depends on the result
- D) `<class 'float'>`

**Q17. [M]** What does `print(type(7 // 2))` show?
- A) `<class 'int'>`
- B) `<class 'float'>`
- C) `<class 'str'>`
- D) `3`

**Q18. [M]** No matter what the user types, `input()` always returns:
- A) An integer
- B) Whatever the user typed, as a number
- C) A string
- D) A float

**Q19. [H]** The user types `25`. What does this print?
```python
n = input()
print(type(n))
```
- A) `<class 'int'>`
- B) `<class 'str'>`
- C) `25`
- D) `<class 'input'>`

**Q20. [M]** Why do we write `int(input())` when reading a number?
- A) To make the program print faster
- B) Because `input()` only accepts integers
- C) To round the input
- D) Because `input()` gives back text, and `int()` converts it so maths works

---

## Section C — `round()` (Q21–Q28)

**Q21. [E]** What is `round(7.6)`?
- A) `8`
- B) `7`
- C) `7.6`
- D) `8.0`

**Q22. [E]** What is `round(7.2)`?
- A) `8`
- B) `7`
- C) `7.2`
- D) `7.0`

**Q23. [H]** What is `round(2.5)`?
- A) `3`
- B) `2.5`
- C) An error
- D) `2`

**Q24. [H]** What is `round(3.5)`?
- A) `3`
- B) `3.5`
- C) `4`
- D) An error

**Q25. [M]** What is `round(3.14159, 2)`?
- A) `3.14`
- B) `3.1`
- C) `3.142`
- D) `3`

**Q26. [M]** What is `round(9.87, 1)`?
- A) `9.8`
- B) `9.9`
- C) `10`
- D) `9.87`

**Q27. [M]** What is `round(7)`?
- A) `7.0`
- B) An error
- C) `7`
- D) `8`

**Q28. [H]** What is `round(-2.5)`?
- A) `-3`
- B) `-2.5`
- C) `3`
- D) `-2`

---

## Section D — `max()`, `min()`, `sum()`, `len()` (Q29–Q40)

**Q29. [E]** What is `max(4, 9, 2)`?
- A) `4`
- B) `9`
- C) `2`
- D) `15`

**Q30. [E]** What is `min(4, 9, 2)`?
- A) `2`
- B) `9`
- C) `4`
- D) `15`

**Q31. [M]** What is `max(3, 3.5)`?
- A) `3`
- B) An error
- C) `3.5`
- D) `3.0`

**Q32. [M]** What is `min(-2, -8)`?
- A) `-2`
- B) `2`
- C) `8`
- D) `-8`

**Q33. [M]** What is `sum([10, 20, 30])`?
- A) `[60]`
- B) `60`
- C) An error
- D) `102030`

**Q34. [H]** What does `sum(10, 20, 30)` produce?
- A) `60`
- B) `30`
- C) An error
- D) `10`

**Q35. [M]** What is `sum([1.5, 2.5])`?
- A) `4.0`
- B) `4`
- C) An error
- D) `1.52.5`

**Q36. [E]** What is `len("hello")`?
- A) `4`
- B) `6`
- C) An error
- D) `5`

**Q37. [M]** What is `len(" hi ")`?
- A) `2`
- B) `4`
- C) `3`
- D) An error

**Q38. [M]** What is `len("3.14")`?
- A) `4`
- B) `3`
- C) An error
- D) `5`

**Q39. [H]** What does `len(2500)` produce?
- A) `4`
- B) `2500`
- C) An error
- D) `0`

**Q40. [M]** What is `len(str(2500))`?
- A) An error
- B) `2500`
- C) `2`
- D) `4`

---

## Section E — Combining Functions (Q41–Q50)

**Q41. [M]** What is `max(min(6, 2), 4)`?
- A) `4`
- B) `2`
- C) `6`
- D) `8`

**Q42. [M]** What does `print(3, 7)` show?
- A) `37`
- B) `3 7`
- C) `3,7`
- D) An error

**Q43. [E]** What does `print()` with nothing inside do?
- A) It causes an error
- B) It prints `0`
- C) It prints an empty line
- D) Nothing at all happens

**Q44. [H]** The user types `7.5`. What happens?
```python
n = int(input())
print(n)
```
- A) It prints `7`
- B) It prints `8`
- C) It prints `7.5`
- D) An error

**Q45. [M]** What does `print(int("5") + int("3"))` show?
- A) `8`
- B) `"53"`
- C) `53`
- D) An error

**Q46. [H]** What does `print(round(0.1 + 0.2, 2))` show?
- A) `0.30000000000000004`
- B) `0.3`
- C) `0.33`
- D) An error

**Q47. [M]** What is `len(str(12 * 100))`?
- A) `5`
- B) `6`
- C) `4`
- D) An error

**Q48. [M]** What is `min(max(3, 8), max(2, 5))`?
- A) `2`
- B) `3`
- C) `8`
- D) `5`

**Q49. [H]** What does `print(type(round(7.6)))` show?
- A) `<class 'float'>`
- B) `<class 'int'>`
- C) `<class 'round'>`
- D) `8`

**Q50. [H]** The user types `6.7`. What does this print?
```python
n = float(input())
print(int(n) + round(n))
```
- A) `13`
- B) `12`
- C) `14`
- D) `13.7`

---

*End of set — 50 questions. Difficulty: 9 [E] · 28 [M] · 13 [H]. Every answer verified by executing the code.*
