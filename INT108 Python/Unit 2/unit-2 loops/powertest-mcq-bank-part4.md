# Loops MCQ Bank — Part 4: Nested Loops Deep Dive (Q151–Q200)

*Fifty questions entirely on nested loops: iteration counting, grid computation, control flow across two loops, patterns, and applied mini-problems.*
*Tags: [M] medium · [H] hard. Answers are in the separate file `loops-mcq-bank-part4-answers.md`.*

---

## Section A — Counting Iterations (Q151–Q160)

**Q151. [M]** How many times does the inner body run in total?
```python
for i in range(0, 10, 2):
    for j in range(0, 9, 3):
        print("x")
```
- A) `30`
- B) `18`
- C) `15`
- D) `90`

**Q152. [M]** How many times does the inner body run in total?
```python
for i in range(4):
    for j in range(i, 3):
        print("x")
```
- A) `6`
- B) `12`
- C) `9`
- D) `10`

**Q153. [M]** How many times does the inner body run in total?
```python
for i in range(1, 4):
    for j in range(2 * i - 1):
        print("x")
```
- A) `6`
- B) `12`
- C) `15`
- D) `9`

**Q154. [H]** How many times does the inner body run in total?
```python
for i in range(5):
    for j in range(i - 2):
        print("x")
```
- A) `10`
- B) `3`
- C) `6`
- D) An error — the range goes negative

**Q155. [H]** How many times does the **innermost** body run in total?
```python
for i in range(3):
    for j in range(i):
        for k in range(j):
            print("x")
```
- A) `1`
- B) `6`
- C) `3`
- D) `27`

**Q156. [M]** How many times does `c = c + 1` run?
```python
c = 0
for i in range(3):
    for j in range(1, 6):
        if j == 2:
            break
        c = c + 1
print(c)
```
- A) `15`
- B) `6`
- C) `3`
- D) `2`

**Q157. [M]** How many times does the inner body run in total?
```python
for i in range(1, 6):
    for j in range(i + 1, 6):
        print("x")
```
- A) `25`
- B) `10`
- C) `15`
- D) `20`

**Q158. [M]** Which of these runs its inner body exactly **8** times?
- A) `for i in range(4):` with inner `for j in range(4):`
- B) `for i in range(2):` with inner `for j in range(2):`
- C) `for i in range(3):` with inner `for j in range(3):`
- D) `for i in range(2):` with inner `for j in range(4):`

**Q159. [M]** Which range fills the blank so the inner body runs exactly **12** times in total?
```python
for i in range(3):
    for j in range(____):
        print("x")
```
- A) `range(3, 7)`
- B) `range(12)`
- C) `range(3)`
- D) `range(1, 4)`

**Q160. [M]** How many times does the bare `print()` run?
```python
for i in range(2, 9, 3):
    for j in range(2):
        print(j, end=" ")
    print()
```
- A) `6`
- B) `3`
- C) `2`
- D) `9`

---

## Section B — Grid Computation & Maths (Q161–Q172)

**Q161. [H]** What does this print?
```python
for i in range(1, 5):
    f = 1
    for j in range(1, i + 1):
        f = f * j
    print(f, end=" ")
```
- A) `1 2 3 4`
- B) `1 1 2 6`
- C) `24 24 24 24`
- D) `1 2 6 24`

**Q162. [M]** What does this print?
```python
for i in range(2, 4):
    p = 1
    for j in range(3):
        p = p * i
        print(p, end=" ")
```
- A) `2 4 8 2 4 8`
- B) `6 6 6 9 9 9`
- C) `2 4 8 3 9 27`
- D) `8 27`

**Q163. [H]** What does this print?
```python
s = 0
for i in range(1, 4):
    for j in range(1, 4):
        s = s + i * j
    print(s, end=" ")
```
- A) `6 18 36`
- B) `6 12 18`
- C) `36 36 36`
- D) `6 6 6`

**Q164. [M]** What does this print?
```python
t = 0
for i in range(1, 4):
    for j in range(1, 4):
        d = i - j
        if d < 0:
            d = -d
        t = t + d
print(t)
```
- A) `0`
- B) `8`
- C) `12`
- D) `6`

**Q165. [H]** What does this print?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 5):
        if i * j > i + j:
            c = c + 1
print(c)
```
- A) `12`
- B) `6`
- C) `10`
- D) `8`

**Q166. [M]** What does this print?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 5):
        if i == 1 or i == 4 or j == 1 or j == 4:
            c = c + 1
print(c)
```
- A) `12`
- B) `16`
- C) `8`
- D) `4`

**Q167. [M]** What does this print?
```python
t = 0
for i in range(1, 5):
    for j in range(1, 5):
        if i == j:
            t = t + i * j
print(t)
```
- A) `10`
- B) `16`
- C) `30`
- D) `4`

**Q168. [H]** How many times does this print `6`?
```python
for i in range(1, 5):
    for j in range(1, 5):
        if i * j == 6:
            print(6)
```
- A) `1`
- B) `2`
- C) `4`
- D) `6`

**Q169. [H]** What does this print?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 5):
        p = i * j
        k = 1
        ok = 0
        while k * k <= p:
            if k * k == p:
                ok = 1
            k = k + 1
        if ok == 1:
            c = c + 1
print(c)
```
- A) `4`
- B) `3`
- C) `8`
- D) `6`

**Q170. [M]** What does this print?
```python
t = 0
for i in range(1, 4):
    for j in range(1, 4):
        if j > i:
            t = t + i * j
print(t)
```
- A) `36`
- B) `14`
- C) `11`
- D) `22`

**Q171. [M]** What does this print?
```python
m = 0
for i in range(1, 5):
    for j in range(1, 5):
        v = i * j - i - j
        if v > m:
            m = v
print(m)
```
- A) `8`
- B) `16`
- C) `7`
- D) `4`

**Q172. [H]** What does the **fourth line** of output show?
```python
for i in range(1, 5):
    for j in range(1, i + 1):
        if i % j == 0:
            print(j, end=" ")
    print()
```
- A) `1 2 3 4`
- B) `1 2 4`
- C) `4`
- D) `1 4`

---

## Section C — Control Flow in Nested Loops (Q173–Q186)

**Q173. [M]** How many times does `c = c + 1` run?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 7):
        if j > i:
            break
        c = c + 1
print(c)
```
- A) `24`
- B) `4`
- C) `6`
- D) `10`

**Q174. [M]** What does this print?
```python
c = 0
for i in range(1, 4):
    for j in range(1, 4):
        if i == j:
            continue
        c = c + 1
print(c)
```
- A) `6`
- B) `9`
- C) `3`
- D) `8`

**Q175. [M]** What does this print?
```python
c = 0
for i in range(1, 4):
    if i == 2:
        continue
    for j in range(1, 4):
        c = c + 1
print(c)
```
- A) `9`
- B) `3`
- C) `6`
- D) `8`

**Q176. [H]** What does this print?
```python
for i in range(1, 5):
    s = 0
    for j in range(1, 4):
        s = s + i * j
    print(s, end=" ")
    if s > 12:
        break
```
- A) `6 12`
- B) `6 12 18`
- C) `6 12 18 24`
- D) `18`

**Q177. [H]** What does this print?
```python
c = 0
for i in range(2, 8):
    for j in range(2, i):
        if i % j == 0:
            break
    else:
        c = c + 1
print(c)
```
- A) `6`
- B) `2`
- C) `3`
- D) `4`

**Q178. [H]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 4):
        pass
    else:
        print(i, end=" ")
```
- A) `1 2 3`
- B) `3`
- C) Nothing — `else` needs a `break`
- D) `1`

**Q179. [M]** What does this print?
```python
a = 1
while a <= 2:
    b = 1
    while b <= 2:
        print(a * 10 + b, end=" ")
        b = b + 1
    a = a + 1
```
- A) `11 12 21 22`
- B) `11 12 21 22 …` forever
- C) `11 21 12 22`
- D) `10 20`

**Q180. [H]** What happens when this runs?
```python
i = 1
while i <= 3:
    j = 1
    while j <= i:
        j = j + 1
        i = i + 1
```
- A) It ends with `i` equal to 4
- B) It ends after 3 passes of the outer loop
- C) It runs forever — `j` can never exceed `i`
- D) An error

**Q181. [H]** What does this print?
```python
n = 8
while n > 1:
    for j in range(2):
        n = n // 2
    print(n, end=" ")
```
- A) `2 0`
- B) `4 2 1`
- C) `4 1`
- D) `2 1`

**Q182. [M]** What does this print?
```python
found = 0
for i in range(2, 7):
    for j in range(2, 7):
        if i * j == 18 and found == 0:
            print(j)
            found = 1
```
- A) `18`
- B) `3`
- C) `9`
- D) `6`

**Q183. [H]** What does the **second line** of output show?
```python
for i in range(1, 4):
    for j in range(3 - i):
        print(0, end=" ")
    for k in range(i):
        print(i, end=" ")
    print()
```
- A) `0 0 2`
- B) `2 2 0`
- C) `0 2 2`
- D) `2 2`

**Q184. [M]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 6):
        if j == 2:
            break
        print(i, j, end="  ")
```
- A) `1 1  1 2  1 3`
- B) `1 1  2 1  3 1`
- C) `1 2  2 2  3 2`
- D) `1 1`

**Q185. [M]** What does this print?
```python
c = 0
for i in range(1, 4):
    for j in range(1, 4):
        if (i + j) % 3 == 0:
            continue
        c = c + 1
print(c)
```
- A) `6`
- B) `9`
- C) `3`
- D) `7`

**Q186. [H]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, i + 1):
        pass
print(i, j)
```
- A) `4 4`
- B) `3 4`
- C) `4 3`
- D) `3 3`

---

## Section D — Patterns & Reverse Engineering (Q187–Q194)

**Q187. [M]** What does this print?
```python
for i in range(1, 4):
    for j in range(i, 0, -1):
        print(j, end=" ")
    print()
```
- A)
  ```
  1 2 3
  1 2
  1
  ```
- B)
  ```
  1
  2 1
  3 2 1
  ```
- C)
  ```
  3 2 1
  2 1
  1
  ```
- D)
  ```
  1
  1 2
  1 2 3
  ```

**Q188. [M]** Which code prints this?
```
1 2 3
1 2 3
```
- A)
  ```python
  for i in range(3):
      for j in range(1, 3):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(2):
      for j in range(1, 4):
          print(i, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(2):
      for j in range(1, 4):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(2):
          print(i, end=" ")
      print()
  ```

**Q189. [M]** What does the **third line** of output show?
```python
for i in range(1, 4):
    for j in range(1, 5):
        print(i * j, end=" ")
    print()
```
- A) `3 6 9 12`
- B) `3 6 9`
- C) `1 2 3 4`
- D) `4 8 12 16`

**Q190. [H]** Which value fills the blank so the code prints the pattern shown?
```
1
2 4
3 6 9
```
```python
for i in range(1, 4):
    for j in range(1, ____):
        print(i * j, end=" ")
    print()
```
- A) `i`
- B) `4`
- C) `j + 1`
- D) `i + 1`

**Q191. [M]** How many numbers does this print in total?
```python
for i in range(1, 5):
    for j in range(2 * i - 1):
        print(i, end=" ")
    print()
```
- A) `10`
- B) `20`
- C) `16`
- D) `12`

**Q192. [H]** What does this print?
```python
for i in range(1, 5):
    for j in range(1, 5):
        if i == 1 or i == 4 or j == 1 or j == 4:
            print("*", end=" ")
        else:
            print(".", end=" ")
    print()
```
- A) A solid 4 × 4 square of stars
- B) A hollow square — a star border with dots inside
- C) Stars on the two diagonals only
- D) Dots on the border with stars inside

**Q193. [M]** What does this print?
```python
for i in range(1, 4):
    for j in range(3 - i):
        print(".", end="")
    for k in range(i):
        print("*", end="")
    print()
```
- A)
  ```
  *..
  **.
  ***
  ```
- B)
  ```
  ***
  .**
  ..*
  ```
- C)
  ```
  .*.
  *.*
  ***
  ```
- D)
  ```
  ..*
  .**
  ***
  ```

**Q194. [H]** Which code prints four rows whose lengths are 7, 5, 3, 1?
- A)
  ```python
  for i in range(4):
      for j in range(7 - 2 * i):
          print("*", end=" ")
      print()
  ```
- B)
  ```python
  for i in range(4):
      for j in range(7 - i):
          print("*", end=" ")
      print()
  ```
- C)
  ```python
  for i in range(7, 0, -2):
      for j in range(4):
          print("*", end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 8, 2):
      for j in range(i):
          print("*", end=" ")
      print()
  ```

---

## Section E — Applied Mini-Problems (Q195–Q200)

**Q195. [M]** What does this print?
```python
c = 0
for i in range(1, 7):
    for j in range(i + 1, 7):
        if j - i == 2:
            c = c + 1
print(c)
```
- A) `6`
- B) `4`
- C) `5`
- D) `2`

**Q196. [M]** What does this print?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 5):
        if j < i:
            c = c + 1
print(c)
```
- A) `10`
- B) `16`
- C) `6`
- D) `8`

**Q197. [H]** What does this print?
```python
t = 0
for i in range(1, 4):
    for j in range(1, 4):
        if i > j:
            t = t + i
        else:
            t = t + j
print(t)
```
- A) `22`
- B) `14`
- C) `18`
- D) `36`

**Q198. [H]** What does this print?
```python
c = 0
for i in range(1, 7):
    for j in range(1, 7):
        if (i * j) % 12 == 0:
            c = c + 1
print(c)
```
- A) `3`
- B) `5`
- C) `12`
- D) `7`

**Q199. [H]** What does this print?
```python
c = 0
for i in range(1, 7):
    for j in range(1, 7):
        if 12 % i == 0 and 12 % j == 0:
            c = c + 1
print(c)
```
- A) `10`
- B) `25`
- C) `5`
- D) `36`

**Q200. [H]** What does this print?
```python
t = 0
for i in range(1, 5):
    for j in range(1, 5):
        if i == j:
            continue
        if i * j > 8:
            break
        t = t + 1
print(t)
```
- A) `12`
- B) `9`
- C) `10`
- D) `16`

---

*End of Part 4 — Q151–Q200. Difficulty: 28 [M] · 22 [H]. Every answer verified by executing the code.*
