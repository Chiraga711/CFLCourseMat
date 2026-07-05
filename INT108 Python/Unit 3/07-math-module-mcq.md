# Math Module — MCQ Set (Q1–Q5)

*Unit 3 · Topic 07. Covers: importing modules, using the `math` module, and the functions `sqrt()`, `pow()`, `ceil()`, `floor()`.*
*Tags: [E] easy · [M] medium · [H] hard. Answers with explanations follow at the end.*

---

**Q1. [M]** What does this print?
```python
import math
print(math.sqrt(16))
```
- A) `4`
- B) `16`
- C) `4.0`
- D) An error

**Q2. [H]** What does this print?
```python
import math
print(math.pow(2, 3))
```
- A) `6`
- B) `8.0`
- C) `8`
- D) `6.0`

**Q3. [M]** What does this print?
```python
import math
print(math.ceil(4.1))
```
- A) `4`
- B) `4.1`
- C) `4.0`
- D) `5`

**Q4. [M]** What does this print?
```python
import math
print(math.floor(4.9))
```
- A) `4`
- B) `5`
- C) `4.9`
- D) `5.0`

**Q5. [H]** What happens when this runs?
```python
print(math.sqrt(9))
```
- A) It prints `3.0`
- B) An error — the `math` module was never imported
- C) It prints `3`
- D) It prints `9`

---

## Answer Key

**Q1 — C.** `math.sqrt` always returns a **float**, so the square root of 16 prints as `4.0`, not `4`. This surprises students who expect a whole number.

**Q2 — B.** `math.pow` also returns a **float**: 2 to the power 3 is `8.0`. (The `**` operator would give the integer `8` here — but `**` is outside this course; `math.pow` is the tool taught, and it always produces a float.)

**Q3 — D.** `math.ceil` rounds **up** to the next whole number, so 4.1 becomes 5. (Ceiling always goes up, even for a tiny fractional part.)

**Q4 — A.** `math.floor` rounds **down**, so 4.9 becomes 4. (Floor always goes down, no matter how close to the next number.)

**Q5 — B.** `math.sqrt` can only be used after `import math`. Without that line, the name `math` is unknown and Python raises a NameError. Every program that uses the module must import it first.

---

*Letter spread: A×1 · B×2 · C×1 · D×1. Difficulty: 0 [E] · 3 [M] · 2 [H]. Every answer verified by executing the code.*
