# Functions & Recursion — Final MCQ Bank, Batch 4 (Q151–Q200)

*Unit 3 final revision bank. Batch 4 of 4. Covers Topic 07 (Math Module), Topic 08 (Recursion), and loops & nested loops used inside functions.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch4-answers.md`.*

---

## Topic 07 — Math Module

**Q151. [M]** What does this print?
```python
import math
print(math.sqrt(49))
```
- A) `7.0`
- B) `7`
- C) `49`
- D) An error

**Q152. [H]** What does this print?
```python
import math
print(math.pow(3, 2))
```
- A) `9`
- B) `9.0`
- C) `6`
- D) `6.0`

**Q153. [M]** What does this print?
```python
import math
print(math.ceil(7.2))
```
- A) `7`
- B) `7.2`
- C) `8`
- D) `7.0`

**Q154. [M]** What does this print?
```python
import math
print(math.floor(7.8))
```
- A) `8`
- B) `7.8`
- C) `8.0`
- D) `7`

**Q155. [H]** What happens here?
```python
print(math.floor(3.5))
```
- A) An error — `math` was never imported
- B) `3`
- C) `4`
- D) `3.5`

**Q156. [M]** What does this print?
```python
import math
print(type(math.sqrt(36)))
```
- A) `<class 'int'>`
- B) `<class 'float'>`
- C) `<class 'str'>`
- D) `6.0`

**Q157. [M]** What does this print?
```python
import math
print(math.ceil(5.0))
```
- A) `6`
- B) `5.0`
- C) `5`
- D) An error

**Q158. [H]** What does this print?
```python
import math
print(math.floor(-3.2))
```
- A) `-3`
- B) `3`
- C) `-3.2`
- D) `-4`

**Q159. [H]** What does this print?
```python
import math
print(math.ceil(-3.2))
```
- A) `-3`
- B) `-4`
- C) `-2`
- D) `3`

**Q160. [M]** What does this print?
```python
import math
print(int(math.pow(2, 4)))
```
- A) `16.0`
- B) `16`
- C) `8`
- D) `6`

**Q161. [M]** What does this print?
```python
import math
def h(a, b):
    return math.sqrt(a * a + b * b)

print(h(6, 8))
```
- A) `10`
- B) `14.0`
- C) `10.0`
- D) `100.0`

**Q162. [E]** What does this print?
```python
import math
print(round(math.pi, 2))
```
- A) `3.0`
- B) `3.1416`
- C) `3`
- D) `3.14`

**Q163. [M]** What does this print?
```python
import math
def boxes(n, c):
    return math.ceil(n / c)

print(boxes(23, 5))
```
- A) `5`
- B) `4`
- C) `4.6`
- D) `6`

**Q164. [M]** What does this print?
```python
import math
print(math.sqrt(64) == 8)
```
- A) `False`
- B) `True`
- C) `8.0`
- D) An error

---

## Topic 08 — Recursion

**Q165. [M]** What does this print?
```python
def f(n):
    if n == 0:
        return 1
    return n * f(n - 1)

print(f(3))
```
- A) `3`
- B) `0`
- C) `6`
- D) `9`

**Q166. [M]** What does this print?
```python
def r(n):
    if n == 0:
        return
    print(n * 2)
    r(n - 1)

r(3)
```
- A) `2 4 6`
- B) `6 4 2 0`
- C) `3 2 1`
- D) `6 4 2`

**Q167. [H]** What does this print?
```python
def f(n):
    if n == 0:
        return
    f(n - 1)
    print(n + 10)

f(3)
```
- A) `11 12 13`
- B) `13 12 11`
- C) `11 12 13 10`
- D) Nothing

**Q168. [M]** What does this print?
```python
def s(n):
    if n == 0:
        return 0
    return n + s(n - 1)

print(s(4))
```
- A) `4`
- B) `10`
- C) `24`
- D) `0`

**Q169. [H]** What happens here?
```python
def f(n):
    return f(n - 1)

print(f(3))
```
- A) It prints `3`
- B) It prints `0`
- C) It never stops and ends with a RecursionError
- D) It prints nothing and stops cleanly

**Q170. [M]** What does this print?
```python
def p(b, e):
    if e == 0:
        return 1
    return b * p(b, e - 1)

print(p(2, 4))
```
- A) `8`
- B) `6`
- C) `2`
- D) `16`

**Q171. [H]** What does this print?
```python
def f(n):
    if n == 0:
        return 0
    return (n % 10) * (n % 10) + f(n // 10)

print(f(23))
```
- A) `13`
- B) `5`
- C) `25`
- D) `6`

**Q172. [H]** What does this print?
```python
def d(n):
    if n <= 1:
        return 0
    return 1 + d(n // 2)

print(d(20))
```
- A) `5`
- B) `4`
- C) `20`
- D) `10`

**Q173. [M]** What does this print?
```python
def d(n):
    if n == 0:
        return 0
    return n % 10 + d(n // 10)

print(d(253))
```
- A) `253`
- B) `8`
- C) `10`
- D) `352`

**Q174. [M]** What does this print?
```python
def c(n):
    if n < 10:
        return 1
    return 1 + c(n // 10)

print(c(4072))
```
- A) `3`
- B) `5`
- C) `10`
- D) `4`

**Q175. [M]** What does this print?
```python
def p(b, e):
    if e == 0:
        return 1
    return b * p(b, e - 1)

print(p(9, 0))
```
- A) `1`
- B) `9`
- C) `0`
- D) `81`

**Q176. [H]** What does this print?
```python
def g(a, b):
    if b == 0:
        return a
    return g(b, a % b)

print(g(48, 18))
```
- A) `18`
- B) `6`
- C) `3`
- D) `12`

**Q177. [H]** What does this print?
```python
def m(n):
    if n == 0:
        return 0
    return 1 + m(n // 2)

print(m(16))
```
- A) `4`
- B) `16`
- C) `5`
- D) `8`

**Q178. [M]** What does this print?
```python
def pr(a, b):
    if a > b:
        return 1
    return a * pr(a + 1, b)

print(pr(2, 4))
```
- A) `6`
- B) `12`
- C) `8`
- D) `24`

**Q179. [H]** What does this print?
```python
def h(n):
    if n == 0:
        return
    print(n)
    h(n - 1)
    print(n * n)

h(2)
```
- A) `2 1 1 4`
- B) `2 1 4`
- C) `4 1 1 2`
- D) `2 1`

**Q180. [H]** What does this print?
```python
def g(n):
    if n <= 0:
        return 0
    return n + g(n - 2)

print(g(6))
```
- A) `21`
- B) `12`
- C) `9`
- D) `6`

**Q181. [M]** What does this print?
```python
def f(n):
    if n == 1:
        return 1
    return n + f(n - 1)

print(f(5))
```
- A) `10`
- B) `14`
- C) `15`
- D) `120`

**Q182. [M]** What does this print?
```python
def cd(n):
    if n < 0:
        return
    print(n, end=' ')
    cd(n - 1)

cd(3)
```
- A) `3 2 1`
- B) `0 1 2 3`
- C) `3 2 1 0 -1`
- D) `3 2 1 0`

---

## Loops & Nested Loops Inside Functions

**Q183. [E]** What does this print?
```python
def f(n):
    s = 0
    for i in range(1, n + 1):
        s = s + i
    return s

print(f(5))
```
- A) `15`
- B) `5`
- C) `10`
- D) `25`

**Q184. [M]** What does this print?
```python
def f(n):
    p = 1
    for i in range(1, n + 1):
        p = p * i
    return p

print(f(4))
```
- A) `10`
- B) `24`
- C) `12`
- D) `4`

**Q185. [M]** What does this print?
```python
def f(n):
    c = 0
    for i in range(1, n + 1):
        if i % 2 == 0:
            c = c + 1
    return c

print(f(10))
```
- A) `10`
- B) `4`
- C) `5`
- D) `6`

**Q186. [H]** What does this print?
```python
def f(n):
    for i in range(n):
        if i * i > 20:
            return i
    return -1

print(f(10))
```
- A) `4`
- B) `6`
- C) `-1`
- D) `5`

**Q187. [M]** What does this print?
```python
def f(n):
    t = 0
    for i in range(1, n + 1):
        for j in range(1, n + 1):
            t = t + 1
    return t

print(f(3))
```
- A) `9`
- B) `6`
- C) `3`
- D) `27`

**Q188. [M]** What does this print?
```python
def f(n):
    s = 0
    for i in range(1, n + 1):
        for j in range(1, i + 1):
            s = s + 1
    return s

print(f(4))
```
- A) `16`
- B) `10`
- C) `8`
- D) `6`

**Q189. [M]** What does this print?
```python
def f(n):
    m = 0
    for i in range(1, n + 1):
        if n % i == 0:
            m = i
    return m

print(f(12))
```
- A) `6`
- B) `1`
- C) `12`
- D) `4`

**Q190. [M]** What does this print?
```python
def f(n):
    r = 0
    while n > 0:
        r = r * 10 + n % 10
        n = n // 10
    return r

print(f(1234))
```
- A) `1234`
- B) `10`
- C) `4`
- D) `4321`

**Q191. [H]** What does this print?
```python
def f(n):
    c = 0
    for i in range(2, n):
        if n % i == 0:
            c = c + 1
    return c

print(f(15))
```
- A) `2`
- B) `0`
- C) `3`
- D) `4`

**Q192. [M]** What does this print?
```python
def f(a, b):
    c = 0
    for i in range(1, a + 1):
        if a % i == 0 and b % i == 0:
            c = c + 1
    return c

print(f(12, 8))
```
- A) `4`
- B) `3`
- C) `2`
- D) `1`

**Q193. [M]** What does this print?
```python
def f(n):
    s = 0
    i = 1
    while i <= n:
        s = s + i
        i = i + 2
    return s

print(f(9))
```
- A) `20`
- B) `45`
- C) `25`
- D) `16`

**Q194. [H]** What does this print?
```python
def f(n):
    count = 0
    for i in range(1, n + 1):
        for j in range(1, n + 1):
            if i + j == n:
                count = count + 1
    return count

print(f(5))
```
- A) `5`
- B) `2`
- C) `3`
- D) `4`

**Q195. [M]** What does this print?
```python
def f(n):
    total = 0
    for i in range(1, n + 1):
        total = total + i * i
    return total

print(f(3))
```
- A) `14`
- B) `6`
- C) `9`
- D) `36`

**Q196. [M]** What does this print?
```python
def f(n):
    c = 0
    for i in range(1, n + 1):
        if i % 2 == 0 or i % 3 == 0:
            c = c + 1
    return c

print(f(10))
```
- A) `5`
- B) `7`
- C) `8`
- D) `3`

**Q197. [H]** What does this print?
```python
def f(n):
    best = 0
    for i in range(1, n + 1):
        if i * (n - i) > best:
            best = i * (n - i)
    return best

print(f(6))
```
- A) `8`
- B) `6`
- C) `9`
- D) `5`

**Q198. [M]** What does this print?
```python
def f(n):
    s = 0
    for i in range(1, n + 1):
        for j in range(1, n + 1):
            if i == j:
                s = s + i * j
    return s

print(f(3))
```
- A) `9`
- B) `6`
- C) `36`
- D) `14`

**Q199. [H]** What does this print?
```python
def f(n):
    c = 0
    for i in range(1, n + 1):
        x = i
        while x % 2 == 0:
            x = x // 2
        if x == 1:
            c = c + 1
    return c

print(f(8))
```
- A) `4`
- B) `3`
- C) `8`
- D) `2`

**Q200. [M]** What does this print?
```python
def f(n):
    t = 0
    for i in range(1, n + 1):
        if i % 3 == 0:
            continue
        t = t + i
    return t

print(f(6))
```
- A) `21`
- B) `12`
- C) `9`
- D) `6`

---

*End of Batch 4 — Q151–Q200. Difficulty: 2 [E] · 31 [M] · 17 [H]. Every answer verified by executing the code.*