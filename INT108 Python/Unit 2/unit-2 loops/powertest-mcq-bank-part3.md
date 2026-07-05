# Loops MCQ Bank — Part 3: Loops in Application, Extended (Q101–Q150)

*The applied tier: digit algorithms, number theory, nested loops with maths, nested conditionals under iteration, and search patterns.*
*Tags: [M] medium · [H] hard (no easy questions in this part). Answers are in the separate file `loops-mcq-bank-part3-answers.md`.*

---

## Section A — Digit-Loop Applications (Q101–Q110)

**Q101. [M]** What does this print?
```python
n = 3852
big = 0
while n > 0:
    d = n % 10
    if d > big:
        big = d
    n = n // 10
print(big)
```
- A) `5`
- B) `8`
- C) `2`
- D) `3`

**Q102. [M]** What does this print?
```python
n = 5297
small = 9
while n > 0:
    d = n % 10
    if d < small:
        small = d
    n = n // 10
print(small)
```
- A) `9`
- B) `5`
- C) `2`
- D) `7`

**Q103. [M]** What does this print?
```python
n = 8674
c = 0
while n > 0:
    if n % 10 > 5:
        c = c + 1
    n = n // 10
print(c)
```
- A) `3`
- B) `2`
- C) `4`
- D) `1`

**Q104. [M]** What does this print?
```python
n = 7245
s = 0
while n > 0:
    d = n % 10
    if d % 2 == 1:
        s = s + d
    n = n // 10
print(s)
```
- A) `18`
- B) `6`
- C) `7`
- D) `12`

**Q105. [H]** What does this print?
```python
n = 4936
s = 0
sign = 1
while n > 0:
    s = s + sign * (n % 10)
    sign = sign * (-1)
    n = n // 10
print(s)
```
- A) `22`
- B) `8`
- C) `-8`
- D) `0`

**Q106. [M]** What does this print?
```python
n = 2552
m = n
r = 0
while m > 0:
    r = r * 10 + m % 10
    m = m // 10
if r == n:
    print(1)
else:
    print(0)
```
- A) `1`
- B) `0`
- C) `2552`
- D) `2`

**Q107. [H]** After the loop body has run **exactly twice**, what is the value of `rev`?
```python
n = 6081
rev = 0
while n > 0:
    rev = rev * 10 + n % 10
    n = n // 10
```
- A) `1`
- B) `81`
- C) `18`
- D) `1806`

**Q108. [H]** What does this print?
```python
n = 41352
while n > 0:
    d = n % 10
    if d > 4:
        break
    n = n // 10
print(d)
```
- A) `2`
- B) `3`
- C) `41352`
- D) `5`

**Q109. [M]** What does this print?
```python
n = 587
while n >= 10:
    s = 0
    while n > 0:
        s = s + n % 10
        n = n // 10
    n = s
print(n)
```
- A) `2`
- B) `20`
- C) `11`
- D) `5`

**Q110. [M]** What does this code compute?
```python
n = 906
c = 0
while n > 0:
    if n % 10 == 0:
        c = c + 1
    n = n // 10
print(c)
```
- A) The number of digits in `n`
- B) How many zero digits `n` contains
- C) The digit sum of `n`
- D) The number with its zeros removed

---

## Section B — Divisors, Primes & GCD (Q111–Q120)

**Q111. [M]** What does this print?
```python
c = 0
for i in range(1, 17):
    if 16 % i == 0:
        c = c + 1
print(c)
```
- A) `4`
- B) `6`
- C) `5`
- D) `3`

**Q112. [H]** What does this print?
```python
n = 21
c = 0
for i in range(1, n + 1):
    if n % i == 0:
        c = c + 1
if c == 2:
    print(1)
else:
    print(c)
```
- A) `1`
- B) `True`
- C) `21`
- D) `4`

**Q113. [M]** What does this print?
```python
count = 0
for k in range(20, 41):
    d = 0
    for i in range(1, k + 1):
        if k % i == 0:
            d = d + 1
    if d == 2:
        count = count + 1
print(count)
```
- A) `4`
- B) `5`
- C) `6`
- D) `3`

**Q114. [H]** After the loop body has run **exactly twice**, what are the values of `a` and `b`?
```python
a = 52
b = 20
while b != 0:
    t = b
    b = a % b
    a = t
```
- A) `20 12`
- B) `12 8`
- C) `8 4`
- D) `4 0`

**Q115. [M]** What does this print?
```python
a = 6
b = 10
k = a
while k % b != 0:
    k = k + a
print(k)
```
- A) `60`
- B) `10`
- C) `16`
- D) `30`

**Q116. [M]** What does this print?
```python
n = 119
i = 2
while n % i != 0:
    i = i + 1
print(i)
```
- A) `17`
- B) `3`
- C) `7`
- D) `119`

**Q117. [H]** What does this print?
```python
n = 20
t = 0
for i in range(1, n):
    if n % i == 0:
        t = t + i
print(t == n)
```
- A) `False`
- B) `True`
- C) `22`
- D) `20`

**Q118. [H]** What does this print?
```python
count = 0
for k in range(1, 31):
    d = 0
    for i in range(1, k + 1):
        if k % i == 0:
            d = d + 1
    if d == 3:
        count = count + 1
print(count)
```
- A) `2`
- B) `3`
- C) `5`
- D) `10`

**Q119. [M]** What does this print?
```python
k = 1
while (k * k) % 10 != 6:
    k = k + 1
print(k)
```
- A) `6`
- B) `16`
- C) `4`
- D) `36`

**Q120. [M]** What does this print?
```python
s = 0
for i in range(1, 31):
    if 30 % i == 0 and 45 % i == 0:
        s = s + i
print(s)
```
- A) `15`
- B) `9`
- C) `45`
- D) `24`

---

## Section C — Nested Loops with Maths (Q121–Q132)

**Q121. [M]** What does this print?
```python
c = 0
for i in range(1, 13):
    for j in range(1, 13):
        if i * j == 12:
            c = c + 1
print(c)
```
- A) `6`
- B) `3`
- C) `12`
- D) `4`

**Q122. [M]** What does this print?
```python
t = 0
for i in range(1, 4):
    for j in range(1, 4):
        if (i + j) % 2 == 0:
            t = t + i + j
print(t)
```
- A) `12`
- B) `20`
- C) `30`
- D) `16`

**Q123. [H]** What does this print?
```python
found = 0
for i in range(2, 7):
    for j in range(2, 7):
        if i * j > 20 and found == 0:
            print(i, j)
            found = 1
```
- A) `4 5`
- B) `5 4`
- C) `4 6`
- D) `5 5`

**Q124. [H]** What does this print?
```python
for i in range(1, 4):
    m = 4
    while m < i * 3:
        m = m + 4
    print(m, end=" ")
```
- A) `3 6 9`
- B) `4 4 8`
- C) `4 6 12`
- D) `4 8 12`

**Q125. [M]** How many times does the inner body run in total?
```python
c = 0
for i in range(1, 5):
    for j in range(i, i * 2):
        c = c + 1
print(c)
```
- A) `6`
- B) `10`
- C) `16`
- D) `4`

**Q126. [H]** What does this print?
```python
c = 0
for i in range(5):
    for j in range(5):
        if (i - 2) * (i - 2) + (j - 2) * (j - 2) <= 1:
            c = c + 1
print(c)
```
- A) `5`
- B) `9`
- C) `1`
- D) `4`

**Q127. [M]** What does this print?
```python
c = 0
for i in range(1, 5):
    for j in range(1, 5):
        if (i * j) % 10 == 2:
            c = c + 1
print(c)
```
- A) `2`
- B) `6`
- C) `3`
- D) `4`

**Q128. [M]** What does this print?
```python
t = 0
for i in range(1, 4):
    for j in range(1, 4):
        if i < j:
            t = t + i
        else:
            t = t + j
print(t)
```
- A) `18`
- B) `12`
- C) `14`
- D) `9`

**Q129. [H]** What does this print?
```python
c = 0
for i in range(1, 4):
    for j in range(0, 10, i):
        c = c + 1
print(c)
```
- A) `30`
- B) `19`
- C) `15`
- D) `10`

**Q130. [H]** What does this print?
```python
c = 0
for i in range(1, 4):
    for j in range(1, 4):
        for k in range(1, 4):
            if i + j + k == 6:
                c = c + 1
print(c)
```
- A) `7`
- B) `6`
- C) `1`
- D) `27`

**Q131. [M]** What does this print?
```python
for i in range(1, 4):
    s = 0
    for j in range(1, 4):
        s = s + i * j
    print(s, end=" ")
```
- A) `1 2 3`
- B) `6 6 6`
- C) `6 12 36`
- D) `6 12 18`

**Q132. [H]** What does this print?
```python
c = 0
for i in range(1, 7):
    for j in range(1, 7):
        if j % i == 0:
            c = c + 1
print(c)
```
- A) `6`
- B) `21`
- C) `14`
- D) `36`

---

## Section D — Nested Conditionals in Loops (Q133–Q142)

**Q133. [H]** What does this print?
```python
c = 0
for i in range(1, 13):
    if i % 2 == 0:
        c = c + 1
    elif i % 3 == 0:
        c = c + 1
print(c)
```
- A) `10`
- B) `8`
- C) `6`
- D) `12`

**Q134. [M]** What does this print?
```python
c = 0
for i in range(1, 25):
    if i % 4 == 0:
        if i % 6 == 0:
            c = c + 1
print(c)
```
- A) `2`
- B) `10`
- C) `4`
- D) `0`

**Q135. [H]** What does this print?
```python
best = 0
pos = 0
for i in range(1, 7):
    v = i % 3 + 1
    if v >= best:
        best = v
        pos = i
print(pos)
```
- A) `2`
- B) `3`
- C) `5`
- D) `6`

**Q136. [M]** What does this print?
```python
t = 0
for i in range(1, 8):
    if i % 2 == 0:
        t = t + i
    else:
        t = t + 1
print(t)
```
- A) `28`
- B) `12`
- C) `7`
- D) `16`

**Q137. [M]** Day 1 is a Monday, so days where `day % 7` is 6 or 0 are the weekend. What does this print?
```python
t = 0
for day in range(1, 11):
    if day % 7 == 6 or day % 7 == 0:
        t = t + 250
    else:
        t = t + 100
print(t)
```
- A) `1300`
- B) `1000`
- C) `1450`
- D) `2500`

**Q138. [H]** What does this print?
```python
c = 0
for i in range(1, 16):
    if i % 15 == 0:
        c = c + 100
    elif i % 5 == 0:
        c = c + 10
    elif i % 3 == 0:
        c = c + 1
print(c)
```
- A) `34`
- B) `124`
- C) `115`
- D) `140`

**Q139. [M]** What does this print?
```python
c = 0
for i in range(1, 10):
    if i % 2 == 0:
        if i > 5:
            c = c + 2
        else:
            c = c + 1
print(c)
```
- A) `8`
- B) `4`
- C) `10`
- D) `6`

**Q140. [H]** What does this print?
```python
for i in range(1, 6):
    if i % 2 == 0:
        if i > 3:
            print(i, end=" ")
    else:
        print(0, end=" ")
```
- A) `0 4`
- B) `2 4`
- C) `0 0 4 0`
- D) `0 0 0 0`

**Q141. [M]** What does this print?
```python
n = 38562
e = 0
o = 0
while n > 0:
    if n % 10 % 2 == 0:
        e = e + 1
    else:
        o = o + 1
    n = n // 10
print(e - o)
```
- A) `1`
- B) `-1`
- C) `5`
- D) `3`

**Q142. [H]** What does this print?
```python
t = 0
for i in range(1, 10):
    if i % 2 == 1 and t < 10:
        t = t + i
print(t)
```
- A) `25`
- B) `16`
- C) `9`
- D) `10`

---

## Section E — Search, `break` & `while` Applications (Q143–Q150)

**Q143. [H]** What does this print?
```python
k = 50
while True:
    k = k + 1
    m = k
    s = 0
    while m > 0:
        s = s + m % 10
        m = m // 10
    if s == 7:
        break
print(k)
```
- A) `61`
- B) `70`
- C) `106`
- D) `52`

**Q144. [M]** What does this print?
```python
k = 7
while k < 100:
    k = k + 7
print(k)
```
- A) `98`
- B) `100`
- C) `105`
- D) `107`

**Q145. [M]** What does this print?
```python
p = 1
c = 0
while p <= 1000:
    p = p * 3
    c = c + 1
print(c)
```
- A) `7`
- B) `6`
- C) `1000`
- D) `8`

**Q146. [H]** What does this print?
```python
n = 68
steps = 0
while n >= 10:
    p = 1
    while n > 0:
        p = p * (n % 10)
        n = n // 10
    n = p
    steps = steps + 1
print(steps)
```
- A) `2`
- B) `3`
- C) `48`
- D) `4`

**Q147. [H]** What does this print?
```python
n = 13
for i in range(2, n):
    if n % i == 0:
        print(i)
        break
else:
    print(0)
```
- A) `13`
- B) `1`
- C) Nothing prints
- D) `0`

**Q148. [M]** What does this print?
```python
k = 99
while True:
    if k % 10 == 1:
        break
    k = k - 9
print(k)
```
- A) `81`
- B) `91`
- C) `9`
- D) `90`

**Q149. [H]** What does this print?
```python
a = 2
b = 100
c = 0
while a < b:
    a = a * 2
    b = b // 2
    c = c + 1
print(a, b, c)
```
- A) `32 6 4`
- B) `16 8 3`
- C) `16 12 3`
- D) `8 25 2`

**Q150. [M]** What does this print?
```python
k = 1
while k * k + k <= 100:
    k = k + 1
print(k)
```
- A) `9`
- B) `10`
- C) `11`
- D) `100`

---

*End of Part 3 — Q101–Q150. Difficulty: 28 [M] · 22 [H]. Every answer verified by executing the code.*
