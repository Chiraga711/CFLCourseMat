# Functions & Recursion — Final MCQ Bank, Batch 3 (Q101–Q150)

*Unit 3 final revision bank. Batch 3 of 4. Covers Topic 05 (Return Values), Topic 06 (Scope of Variables), and conditionals & operators used inside functions.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch3-answers.md`.*

---

## Topic 05 — Return Values

**Q101. [M]** What does this program display on screen?
```python
def add(a, b):
    return a + b

add(3, 4)
```
- A) Nothing
- B) `7`
- C) `None`
- D) An error

**Q102. [H]** What does this print?
```python
def show(n):
    print(n)

print(show(9))
```
- A) `9`
- B) `9` then `None`
- C) `None`
- D) `9` then `9`

**Q103. [M]** What does this print?
```python
def f(n):
    if n > 0:
        return 'yes'
    return 'no'

print(f(5))
```
- A) `no`
- B) `yes` then `no`
- C) `yes`
- D) `5`

**Q104. [M]** What does this print?
```python
def sq(n):
    return n * n

print(sq(2) + sq(3))
```
- A) `25`
- B) `4 9`
- C) `sq(2)+sq(3)`
- D) `13`

**Q105. [H]** What does this print?
```python
def f(a, b):
    return a + b, a - b

x, y = f(10, 4)
print(x, y)
```
- A) `14 6`
- B) `6 14`
- C) `14` then `6`
- D) An error

**Q106. [H]** What does this print?
```python
def first(n):
    for i in range(1, n + 1):
        if i * i > n:
            return i
    return -1

print(first(10))
```
- A) `3`
- B) `4`
- C) `-1`
- D) `10`

**Q107. [M]** What does this print?
```python
def f():
    print('hi')

x = f()
print(x)
```
- A) `hi`
- B) `None`
- C) `hi` then `None`
- D) An error

**Q108. [M]** What does this print?
```python
def f(n):
    if n < 0:
        return
    print(n)

f(-3)
```
- A) `-3`
- B) `None`
- C) An error
- D) Nothing

**Q109. [M]** What does this print?
```python
def is_big(n):
    return n > 100

print(is_big(50))
```
- A) `True`
- B) `False`
- C) `50`
- D) An error

**Q110. [M]** What does this print?
```python
def dbl(n):
    return n * 2

def trip(n):
    return n * 3

print(dbl(trip(2)))
```
- A) `6`
- B) `10`
- C) `12`
- D) `36`

**Q111. [M]** What does this print?
```python
def f():
    return 1
    return 2

print(f())
```
- A) `1`
- B) `2`
- C) `1` then `2`
- D) `3`

**Q112. [E]** What does this print?
```python
def f(n):
    return n + 1

r = f(9)
print(r)
```
- A) `9`
- B) `10`
- C) `None`
- D) An error

**Q113. [M]** What does this print?
```python
def sw(a, b):
    return b, a

p, q = sw(1, 2)
print(p, q)
```
- A) `1 2`
- B) `2 2`
- C) `2 1`
- D) An error

**Q114. [H]** What happens here?
```python
def f():
    print('x')

y = f()
print(y + 1)
```
- A) `x` then `1`
- B) `x` then `2`
- C) `x` then `None`
- D) `x` prints, then an error on `y + 1`

**Q115. [M]** What does this print?
```python
def f(a, b):
    return a > b

print(f(3, 8))
```
- A) `False`
- B) `True`
- C) `3`
- D) `8`

**Q116. [M]** What does this print?
```python
def half(n):
    return n // 2

def f(n):
    return half(n) + 1

print(f(10))
```
- A) `5`
- B) `6`
- C) `11`
- D) `10`

**Q117. [M]** What does this print?
```python
def f(n):
    if n % 2 == 0:
        return 'even'
    return 'odd'

print(f(7))
```
- A) `even`
- B) `7`
- C) `odd`
- D) `True`

**Q118. [H]** What does this print?
```python
def f(n):
    return n, n * n, n * n * n

a, b, c = f(2)
print(a, b, c)
```
- A) `2 2 2`
- B) `8 4 2`
- C) An error
- D) `2 4 8`

**Q119. [H]** What does this print?
```python
def f(n):
    print(n * 2)

result = f(5)
print(result)
```
- A) `10` then `None`
- B) `10`
- C) `None`
- D) `10` then `10`

**Q120. [M]** What does this print?
```python
def s(n):
    t = 0
    for i in range(1, n + 1):
        t = t + i
    return t

print(s(4))
```
- A) `4`
- B) `10`
- C) `24`
- D) `0`

---

## Topic 06 — Scope of Variables

**Q121. [M]** What does this print?
```python
x = 5
def f():
    x = 99

f()
print(x)
```
- A) `99`
- B) Nothing
- C) `5`
- D) An error

**Q122. [H]** What does this print?
```python
n = 3
def f(n):
    print(n)

f(8)
print(n)
```
- A) `8` then `3`
- B) `3` then `8`
- C) `8` then `8`
- D) `3` then `3`

**Q123. [M]** What does this print?
```python
c = 10
def f():
    print(c)

f()
```
- A) `0`
- B) An error
- C) Nothing
- D) `10`

**Q124. [H]** What happens here?
```python
t = 0
def f():
    print(t)
    t = t + 1

f()
```
- A) `0`
- B) `1`
- C) An error — `t` is used before assignment inside `f`
- D) `0` then `1`

**Q125. [H]** What happens here?
```python
def f():
    y = 1

f()
print(y)
```
- A) `1`
- B) `0`
- C) Nothing
- D) An error — `y` is local and gone after the call

**Q126. [M]** What does this print?
```python
v = 2
def inc(v):
    return v + 1

v = inc(v)
print(v)
```
- A) `3`
- B) `2`
- C) `1`
- D) An error

**Q127. [M]** What does this print?
```python
def a():
    z = 1
    print(z)

def b():
    z = 2
    print(z)

a()
b()
```
- A) `2` then `1`
- B) `1` then `2`
- C) `1` then `1`
- D) An error

**Q128. [H]** What does this print?
```python
def f(a):
    a = a + 10
    print(a)

x = 5
f(x)
print(x)
```
- A) `15` then `15`
- B) `5` then `15`
- C) `15` then `5`
- D) `5` then `5`

**Q129. [H]** What does this print?
```python
g = 1
def f():
    global g
    g = 50

f()
print(g)
```
- A) `1`
- B) An error
- C) Nothing
- D) `50`

**Q130. [H]** What does this print?
```python
def f():
    for i in range(3):
        pass
    print(i)

f()
```
- A) `2`
- B) `3`
- C) `0`
- D) An error

**Q131. [M]** What does this print?
```python
total = 0
def add(x):
    return total + x

print(add(5))
```
- A) `0`
- B) `5`
- C) An error
- D) Nothing

**Q132. [H]** What does this print?
```python
k = 100
def f(k):
    return k * 2

print(f(3))
print(k)
```
- A) `6` then `6`
- B) `200` then `100`
- C) `6` then `100`
- D) `6` then `200`

**Q133. [E]** What does this print?
```python
def f():
    a = 7
    return a

print(f())
```
- A) `a`
- B) `None`
- C) An error
- D) `7`

**Q134. [M]** What does this print?
```python
def f(n):
    n = n * 2
    return n

m = 4
print(f(m), m)
```
- A) `8 4`
- B) `8 8`
- C) `4 4`
- D) `4 8`

**Q135. [M]** What does this print?
```python
PI = 3
def area(r):
    return PI * r * r

print(area(2))
```
- A) `6`
- B) `12`
- C) `9`
- D) An error

**Q136. [H]** What does this print?
```python
count = 0
def bump():
    return count + 1

count = bump()
count = bump()
print(count)
```
- A) `1`
- B) `0`
- C) `2`
- D) `3`

---

## Conditionals & Operators Inside Functions

**Q137. [M]** What does this print?
```python
def f(a, b):
    if a % b == 0:
        return 'divisible'
    return 'not'

print(f(15, 3))
```
- A) `not`
- B) `5`
- C) `0`
- D) `divisible`

**Q138. [M]** What does this print?
```python
def f(n):
    if n > 0 and n % 2 == 0:
        return 'pos even'
    return 'other'

print(f(6))
```
- A) `pos even`
- B) `other`
- C) `6`
- D) `True`

**Q139. [H]** What does this print?
```python
def f(a, b, c):
    if a > b and a > c:
        return a
    if b > c:
        return b
    return c

print(f(3, 9, 5))
```
- A) `3`
- B) `9`
- C) `5`
- D) `17`

**Q140. [M]** What does this print?
```python
def f(n):
    return (n % 2 == 0) and (n > 10)

print(f(8))
```
- A) `True`
- B) `8`
- C) An error
- D) `False`

**Q141. [M]** What does this print?
```python
def f(x):
    if not x > 5:
        return 'small'
    return 'big'

print(f(3))
```
- A) `small`
- B) `big`
- C) `3`
- D) `True`

**Q142. [H]** What does this print?
```python
def f(a, b):
    if a == b or a + b == 10:
        return 'match'
    return 'no'

print(f(4, 6))
```
- A) `no`
- B) `match`
- C) `10`
- D) An error

**Q143. [H]** What does this print?
```python
def f(m):
    if m >= 40:
        if m >= 75:
            return 'distinction'
        return 'pass'
    return 'fail'

print(f(50))
```
- A) `distinction`
- B) `fail`
- C) `pass`
- D) `50`

**Q144. [M]** What does this print?
```python
def f(n):
    c = 0
    for i in range(1, n + 1):
        if n % i == 0:
            c = c + 1
    return c

print(f(6))
```
- A) `6`
- B) `3`
- C) `2`
- D) `4`

**Q145. [M]** What does this print?
```python
def bigger(a, b):
    if a > b:
        return a
    return b

print(bigger(3, 8))
```
- A) `8`
- B) `3`
- C) `11`
- D) `True`

**Q146. [M]** What does this print?
```python
def f(n):
    total = 0
    for i in range(1, n + 1):
        if i % 2 == 0:
            total = total + i
    return total

print(f(6))
```
- A) `6`
- B) `12`
- C) `9`
- D) `21`

**Q147. [H]** What does this print?
```python
def f(n):
    if n % 3 == 0 and n % 5 == 0:
        return 'both'
    elif n % 3 == 0:
        return 'three'
    elif n % 5 == 0:
        return 'five'
    return 'none'

print(f(15))
```
- A) `three`
- B) `five`
- C) `both`
- D) `none`

**Q148. [M]** What does this print?
```python
def f(a, b):
    if a > b:
        return a - b
    return b - a

print(f(3, 10))
```
- A) `7`
- B) `-7`
- C) `13`
- D) `3`

**Q149. [H]** What does this print?
```python
def f(n):
    count = 0
    for i in range(1, n + 1):
        for j in range(1, n + 1):
            if i * j == n:
                count = count + 1
    return count

print(f(6))
```
- A) `6`
- B) `4`
- C) `2`
- D) `3`

**Q150. [M]** What does this print?
```python
def f(x, y):
    return x > 0 and y > 0

print(f(5, -2))
```
- A) `True`
- B) `5`
- C) An error
- D) `False`

---

*End of Batch 3 — Q101–Q150. Difficulty: 2 [E] · 29 [M] · 19 [H]. Every answer verified by executing the code.*