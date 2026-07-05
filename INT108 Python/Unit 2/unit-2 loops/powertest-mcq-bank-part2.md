# Loops MCQ Bank — Part 2 (Q55–Q100)

*Sections 5–8: nested loops, pattern reading, accumulators & loop idioms, and loops in application.*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `loops-mcq-bank-part2-answers.md`.*

---

## Section 5 — Nested Loops (Q55–Q68)

**Q55. [E]** What does this print?
```python
for i in range(1, 3):
    for j in range(1, 3):
        print(i + j)
```
- A) `2 3 4 5`
- B) `2 3 3 4`
- C) `1 2 1 2`
- D) `2 4`

**Q56. [E]** How many times does the inner body run in total?
```python
for i in range(2):
    for j in range(2 * 3):
        print("x")
```
- A) `8`
- B) `6`
- C) `12`
- D) `36`

**Q57. [M]** What does the **second line** of output show?
```python
for i in range(1, 4):
    for j in range(i * 2):
        print(i, end=" ")
    print()
```
- A) `2 2`
- B) `1 1`
- C) `2 2 2`
- D) `2 2 2 2`

**Q58. [M]** What does this print?
```python
total = 0
for i in range(1, 3):
    for j in range(1, 4):
        total = total + i * j
print(total)
```
- A) `18`
- B) `12`
- C) `36`
- D) `6`

**Q59. [M]** What does this print?
```python
count = 0
for i in range(1, 5):
    for j in range(1, 5):
        if i == j:
            count = count + 1
print(count)
```
- A) `16`
- B) `4`
- C) `1`
- D) `8`

**Q60. [H]** What does this print?
```python
for i in range(1, 4):
    for j in range(i, 4):
        print(i * 10 + j, end=" ")
```
- A) `11 12 13 21 22 23 31 32 33`
- B) `11 22 33`
- C) `11 12 13 22 23 33`
- D) `13 23 33`

**Q61. [H]** What does this print?
```python
for i in range(3):
    for i in range(2):
        print(i, end=" ")
```
- A) `0 1 0 1 0 1`
- B) `0 1`
- C) `0 1 2 0 1 2`
- D) An error — `i` is used twice

**Q62. [H]** What does this print?
```python
for i in range(1, 4):
    n = i
    while n < 4:
        n = n * 2
    print(n)
```
- A) `2 4 6`
- B) `4 4 4`
- C) `1 2 3`
- D) `4 4 6`

**Q63. [M]** How many times does the inner body run in total?
```python
for i in range(3):
    for j in range(i):
        print(j)
```
- A) `6`
- B) `3`
- C) `9`
- D) `0`

**Q64. [H]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 6):
        if i * j > 6:
            break
        print(i * j, end=" ")
```
- A) `1 2 3 4 5 2 4 6 3 6`
- B) `1 2 3 4 5 2 4 3 6`
- C) `1 2 3 4 5`
- D) `1 2 3 2 4 6 3 6 9`

**Q65. [E]** What does this print?
```python
for i in range(2):
    for j in range(3):
        print(j, end=" ")
```
- A) `0 1 2` on one line, `0 1 2` on the next
- B) `0 1 0 1 0 1`
- C) `0 1 2 0 1 2` all on one line
- D) `0 0 1 1 2 2`

**Q66. [M]** What does this print?
```python
count = 0
for i in range(2):
    for j in range(3):
        for k in range(2):
            count = count + 1
print(count)
```
- A) `7`
- B) `6`
- C) `8`
- D) `12`

**Q67. [M]** What does this print?
```python
count = 0
for i in range(1, 6):
    for j in range(1, 6):
        if i + j == 6:
            count = count + 1
print(count)
```
- A) `2`
- B) `5`
- C) `3`
- D) `25`

**Q68. [M]** Which code prints this?
```
1 2 3
2 4 6
3 6 9
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(i * j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(i + j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(i * i, end=" ")
      print()
  ```

---

## Section 6 — Pattern Reading (Q69–Q78)

**Q69. [E]** What shape does this print?
```python
for i in range(3):
    for j in range(3):
        print("*", end=" ")
    print()
```
- A) A growing triangle
- B) A shrinking triangle
- C) A solid 3 × 3 square
- D) A single row of 9 stars

**Q70. [M]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 4):
        if i == j:
            print("*", end=" ")
        else:
            print(".", end=" ")
    print()
```
- A)
  ```
  * * *
  . . .
  * * *
  ```
- B)
  ```
  * . .
  . * .
  . . *
  ```
- C)
  ```
  . . *
  . * .
  * . .
  ```
- D)
  ```
  * * *
  * * *
  * * *
  ```

**Q71. [M]** What does this print?
```python
for i in range(3, 0, -1):
    for j in range(1, i + 1):
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
  1 2
  1 2 3
  ```
- C)
  ```
  3 2 1
  2 1
  1
  ```
- D)
  ```
  3
  3 3
  3 3 3
  ```

**Q72. [M]** What does this print?
```python
for i in range(1, 4):
    for j in range(i):
        print(i, end="")
    print()
```
- A)
  ```
  1
  2 2
  3 3 3
  ```
- B)
  ```
  111
  222
  333
  ```
- C)
  ```
  1
  12
  123
  ```
- D)
  ```
  1
  22
  333
  ```

**Q73. [E]** Which value fills the blank so the code prints the pattern shown?
```
5
5 5
5 5 5
```
```python
for i in range(1, 4):
    for j in range(____):
        print(5, end=" ")
    print()
```
- A) `3`
- B) `i`
- C) `j`
- D) `i + 1`

**Q74. [H]** What does this print?
```python
for i in range(1, 4):
    for j in range(1, 2 * i, 2):
        print(j, end=" ")
    print()
```
- A)
  ```
  1
  1 2
  1 2 3
  ```
- B)
  ```
  1 3 5
  1 3
  1
  ```
- C)
  ```
  1
  1 3
  1 3 5
  ```
- D)
  ```
  2
  2 4
  2 4 6
  ```

**Q75. [M]** How many stars does this print in total?
```python
for i in range(1, 6):
    for j in range(7 - i):
        print("*", end=" ")
    print()
```
- A) `15`
- B) `25`
- C) `30`
- D) `20`

**Q76. [M]** Which code prints this?
```
3 2 1
3 2 1
```
- A)
  ```python
  for i in range(2):
      for j in range(3, 0, -1):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(3):
      for j in range(2, 0, -1):
          print(j, end=" ")
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
  for i in range(2):
      for j in range(3, 1, -1):
          print(j, end=" ")
      print()
  ```

**Q77. [H]** What does this print?
```python
for i in range(3):
    for j in range(3):
        if (i + j) % 2 == 0:
            print("*", end=" ")
        else:
            print("-", end=" ")
    print()
```
- A)
  ```
  * * *
  - - -
  * * *
  ```
- B)
  ```
  * - *
  - * -
  * - *
  ```
- C)
  ```
  - * -
  * - *
  - * -
  ```
- D)
  ```
  * - -
  - * -
  - - *
  ```

**Q78. [M]** What does this print?
```python
for i in range(2):
    for j in range(2):
        print("*", end=" ")
        print()
```
- A) A 2 × 2 square of stars
- B) `* * * *` on one line
- C) Four lines, each with a single star
- D) Two lines with two stars each

---

## Section 7 — Accumulators & Loop Idioms (Q79–Q92)

**Q79. [E]** What does this print?
```python
count = 0
for i in range(1, 21):
    if i % 4 == 0:
        count = count + 1
print(count)
```
- A) `5`
- B) `4`
- C) `20`
- D) `60`

**Q80. [M]** What does this print?
```python
p = 0
for i in range(1, 5):
    p = p * i
print(p)
```
- A) `24`
- B) `10`
- C) `4`
- D) `0`

**Q81. [M]** What does this print?
```python
big = 0
for i in range(1, 5):
    v = i * (5 - i)
    if v > big:
        big = v
print(big)
```
- A) `4`
- B) `6`
- C) `16`
- D) `5`

**Q82. [H]** What does this print?
```python
small = 0
for i in range(3, 7):
    if i < small:
        small = i
print(small)
```
- A) `0`
- B) `3`
- C) `6`
- D) An error

**Q83. [E]** What does this print?
```python
found = 0
for i in range(1, 6):
    if i * i == 16:
        found = 1
print(found)
```
- A) `4`
- B) `0`
- C) `1`
- D) `16`

**Q84. [E]** What does this code compute?
```python
n = 6
r = 1
for i in range(1, n + 1):
    r = r * i
print(r)
```
- A) The sum 1 + 2 + … + n
- B) The factorial of n
- C) n squared
- D) 2 to the power n

**Q85. [M]** What does this code compute?
```python
c = 0
m = 273
while m > 0:
    c = c + 1
    m = m // 10
print(c)
```
- A) The digit sum of 273
- B) The reverse of 273
- C) The largest digit of 273
- D) The number of digits in 273

**Q86. [H]** What does this code compute?
```python
a = 24
b = 18
while b != 0:
    t = b
    b = a % b
    a = t
print(a)
```
- A) The larger of the two numbers
- B) The remainder of 24 ÷ 18
- C) The greatest common divisor of 24 and 18
- D) The least common multiple of 24 and 18

**Q87. [M]** What does this print?
```python
total = 100
for i in range(1, 5):
    if i % 2 == 0:
        total = total + i
    else:
        total = total - i
print(total)
```
- A) `102`
- B) `98`
- C) `110`
- D) `100`

**Q88. [M]** What does this print?
```python
total = 0
for i in range(4, 13, 4):
    total = total + i
print(total // 3)
```
- A) `24`
- B) `8`
- C) `7`
- D) `12`

**Q89. [H]** What does this print?
```python
s = 0
p = 1
for i in range(1, 4):
    s = s + i
    p = p * i
print(p - s)
```
- A) `6`
- B) `12`
- C) `3`
- D) `0`

**Q90. [M]** What does this print?
```python
c = 0
for i in range(2, 11, 3):
    c = c + 1
print(c, i)
```
- A) `4 11`
- B) `3 10`
- C) `3 8`
- D) `4 8`

**Q91. [H]** What does this print?
```python
best = 0
pos = 0
for i in range(1, 6):
    v = (i - 3) * (i - 3)
    if v > best:
        best = v
        pos = i
print(pos, best)
```
- A) `1 4`
- B) `5 4`
- C) `3 0`
- D) `1 2`

**Q92. [M]** What does this print?
```python
d = 0
for i in range(1, 5):
    d = i - d
print(d)
```
- A) `4`
- B) `10`
- C) `-2`
- D) `2`

---

## Section 8 — Loops in Application (Q93–Q100)

**Q93. [M]** What does this print?
```python
c = 0
for i in range(1, 19):
    if 18 % i == 0:
        c = c + 1
print(c)
```
- A) `5`
- B) `6`
- C) `18`
- D) `3`

**Q94. [M]** What does this print?
```python
s = 0
for i in range(1, 12):
    if 12 % i == 0:
        s = s + i
print(s)
```
- A) `28`
- B) `12`
- C) `16`
- D) `10`

**Q95. [M]** What does this print?
```python
n = 205
p = 1
while n > 0:
    d = n % 10
    p = p * d
    n = n // 10
print(p)
```
- A) `0`
- B) `10`
- C) `7`
- D) `25`

**Q96. [H]** What does this print?
```python
n = 1200
r = 0
while n > 0:
    r = r * 10 + n % 10
    n = n // 10
print(r)
```
- A) `0021`
- B) `2100`
- C) `1200`
- D) `21`

**Q97. [M]** What does this print?
```python
c = 0
for k in range(10, 31):
    if k % 3 == 0 and k % 2 != 0:
        c = c + 1
print(c)
```
- A) `7`
- B) `3`
- C) `4`
- D) `10`

**Q98. [M]** What does this print?
```python
k = 1
while True:
    if k * k > 50:
        break
    k = k + 1
print(k, k * k)
```
- A) `7 49`
- B) `50 2500`
- C) `8 64`
- D) `7 64`

**Q99. [M]** What does this print?
```python
c = 0
for i in range(1, 9):
    if 8 % i == 0 and 12 % i == 0:
        c = c + 1
print(c)
```
- A) `4`
- B) `6`
- C) `2`
- D) `3`

**Q100. [H]** What does this print?
```python
n = 10
steps = 0
while n != 1:
    if n % 2 == 0:
        n = n // 2
    else:
        n = 3 * n + 1
    steps = steps + 1
print(steps)
```
- A) `6`
- B) `5`
- C) `9`
- D) `4`

---

*End of Part 2 — Q55–Q100. Difficulty: 8 [E] · 26 [M] · 12 [H]. Every answer verified by executing the code.*
