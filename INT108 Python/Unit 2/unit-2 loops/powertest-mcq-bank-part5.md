# Loops MCQ Bank — Part 5: Fill in the Blank (Q201–Q250)

*Fifty complete-the-code questions: each shows a target output, and the blank is a `range()`, a condition, an update, a keyword, an initialization, or an expression.*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `loops-mcq-bank-part5-answers.md`.*

---

## Section A — Complete the `range()` (Q201–Q210)

**Q201. [M]** Which range fills the blank so the code prints `4 7 10 13`?
```python
for i in range(____):
    print(i, end=" ")
```
- A) `4, 13, 3`
- B) `4, 14, 3`
- C) `4, 16, 4`
- D) `3, 13, 3`

**Q202. [M]** Which range fills the blank so the code prints `9 6 3`?
```python
for i in range(____):
    print(i, end=" ")
```
- A) `9, 3, -3`
- B) `3, 9, 3`
- C) `9, -1, -3`
- D) `9, 0, -3`

**Q203. [M]** Which range fills the blank so the code prints **only** `End`?
```python
for i in range(____):
    print(i)
print("End")
```
- A) `range(1)`
- B) `range(0, 5)`
- C) `range(5, 5)`
- D) `range(0, 1)`

**Q204. [M]** Which range fills the blank so the code prints `1 4 9 16 25`?
```python
for i in range(____):
    print(i * i, end=" ")
```
- A) `1, 6`
- B) `5`
- C) `1, 5`
- D) `25`

**Q205. [M]** Which range fills the blank so the code prints `5 10 15 20`?
```python
for i in range(____):
    print(i, end=" ")
```
- A) `5, 21, 5`
- B) `5, 20, 5`
- C) `0, 21, 5`
- D) `5, 25, 10`

**Q206. [M]** Which stop value makes the body run exactly **7** times?
```python
for i in range(3, ____):
    print("x")
```
- A) `7`
- B) `9`
- C) `11`
- D) `10`

**Q207. [M]** Which inner range makes the inner body run **10** times in total?
```python
for i in range(2):
    for j in range(____):
        print("x")
```
- A) `10`
- B) `2`
- C) `5`
- D) `8`

**Q208. [M]** Which value fills the blank so the code prints rows of 4, 3, 2, 1 stars?
```python
for i in range(4):
    for j in range(____):
        print("*", end="")
    print()
```
- A) `i`
- B) `4 - i`
- C) `i + 1`
- D) `3 - i`

**Q209. [M]** Which step fills the blank so the code prints `7 5 3 1`?
```python
for i in range(7, 0, ____):
    print(i, end=" ")
```
- A) `-1`
- B) `-2`
- C) `2`
- D) `-3`

**Q210. [H]** Which stop value makes `i` end the loop holding exactly **30**?
```python
for i in range(0, ____, 6):
    pass
print(i)
```
- A) `24`
- B) `29`
- C) `30`
- D) `31`

---

## Section B — Complete the Condition (Q211–Q220)

**Q211. [M]** Which condition fills the blank so the code prints `5 4 3 2 1`?
```python
n = 5
while ____:
    print(n, end=" ")
    n = n - 1
```
- A) `n >= 0`
- B) `n > 1`
- C) `n > 0`
- D) `n < 5`

**Q212. [M]** Which condition fills the blank so the code prints `3 6 12 24 48 96`?
```python
n = 3
while ____:
    print(n, end=" ")
    n = n * 2
```
- A) `n < 100`
- B) `n < 96`
- C) `n <= 200`
- D) `n > 0`

**Q213. [M]** Which condition fills the blank so the code prints `30` (the sum of the multiples of 3 from 1 to 12)?
```python
total = 0
for i in range(1, 13):
    if ____:
        continue
    total = total + i
print(total)
```
- A) `i % 3 != 0`
- B) `i % 3 == 0`
- C) `i // 3 == 0`
- D) `i % 2 != 0`

**Q214. [H]** Which condition fills the blank so the code prints `1 2 3 4 5 6`?
```python
for i in range(1, 10):
    if ____:
        break
    print(i, end=" ")
```
- A) `i * i >= 36`
- B) `i > 36`
- C) `i == 6`
- D) `i * i > 36`

**Q215. [H]** Which condition fills the blank so the code prints `0`?
```python
a = 10
b = 5
while ____:
    a = a - b
print(a)
```
- A) `a > b`
- B) `a == b`
- C) `a >= b`
- D) `b > 0`

**Q216. [M]** Which condition fills the blank so that `Done` is printed?
```python
for i in range(5):
    if ____:
        break
else:
    print("Done")
```
- A) `i == 3`
- B) `i == 7`
- C) `i >= 0`
- D) `i < 5`

**Q217. [M]** The stream should end only when a **negative** number is entered (a 0 keeps it going). Which condition fills the blank?
```python
v = int(input())
while ____:
    v = int(input())
print("Done")
```
- A) `v > 0`
- B) `v >= 0`
- C) `v < 0`
- D) `v != 0`

**Q218. [M]** Which condition fills the blank so the code prints `5` (the even numbers above 10, up to 20)?
```python
c = 0
for i in range(1, 21):
    if ____:
        c = c + 1
print(c)
```
- A) `i % 2 == 0`
- B) `i % 2 == 0 or i > 10`
- C) `i > 10`
- D) `i % 2 == 0 and i > 10`

**Q219. [H]** Which condition fills the blank so the code prints `20 15`?
```python
a = 0
b = 30
while ____:
    a = a + 4
    b = b - 3
print(a, b)
```
- A) `a > b`
- B) `a != b`
- C) `a < b`
- D) `b < a`

**Q220. [H]** Which condition fills the blank so the code prints `4` (the digit count of 1083)?
```python
n = 1083
c = 0
while ____:
    c = c + 1
    n = n // 10
print(c)
```
- A) `n > 0`
- B) `n > 1`
- C) `n >= 0`
- D) `n != 1`

---

## Section C — Complete the Update (Q221–Q230)

**Q221. [M]** Which update fills the blank so the code prints `20 15 10 5`?
```python
n = 20
while n > 0:
    print(n, end=" ")
    ____
```
- A) `n = n - 5`
- B) `n = n - 4`
- C) `n = n + 5`
- D) `n = n // 5`

**Q222. [M]** Which update fills the blank so the code prints `1 2 4 8 16`?
```python
p = 1
for i in range(5):
    print(p, end=" ")
    ____
```
- A) `p = p + 2`
- B) `p = p * p`
- C) `p = p + 1`
- D) `p = p * 2`

**Q223. [M]** Which update fills the blank so the code prints `204` (the reverse of 402)?
```python
n = 402
rev = 0
while n > 0:
    ____
    n = n // 10
print(rev)
```
- A) `rev = rev + n % 10`
- B) `rev = rev * 10 + n // 10`
- C) `rev = rev * 10 + n % 10`
- D) `rev = rev + n // 10`

**Q224. [H]** Which update fills the blank so this loop actually **ends**?
```python
i = 0
while i != 100:
    ____
```
- A) `i = i + 3`
- B) `i = i + 5`
- C) `i = i * 2`
- D) `i = i + 7`

**Q225. [H]** Which line fills the blank so the code prints the Fibonacci numbers `1 2 3 5 8`?
```python
a = 0
b = 1
for i in range(5):
    t = a + b
    ____
    b = t
    print(b, end=" ")
```
- A) `a = t`
- B) `a = b`
- C) `a = a + b`
- D) `b = a`

**Q226. [M]** Which update fills the blank so the code prints `64 32 16 8`?
```python
x = 64
for i in range(4):
    print(x, end=" ")
    ____
```
- A) `x = x - 32`
- B) `x = x / 2`
- C) `x = x - 16`
- D) `x = x // 2`

**Q227. [H]** Which line fills the blank so the code prints `6` (the GCD of 24 and 18)?
```python
a = 24
b = 18
while b != 0:
    t = b
    ____
    a = t
print(a)
```
- A) `b = b % a`
- B) `b = a // b`
- C) `b = a % b`
- D) `b = a - t`

**Q228. [M]** Which line fills the blank so the code prints `12` (the digit sum of 507)?
```python
n = 507
s = 0
while n > 0:
    ____
    n = n // 10
print(s)
```
- A) `s = s + n % 10`
- B) `s = s * 10 + n % 10`
- C) `s = s + n // 10`
- D) `s = n % 10`

**Q229. [M]** Which line fills the blank so the code prints `1 3 6 10`?
```python
t = 0
for i in range(1, 5):
    ____
    print(t, end=" ")
```
- A) `t = t + 1`
- B) `t = t + i`
- C) `t = t * i`
- D) `t = i`

**Q230. [H]** Which update fills the blank so the code prints `1 4 1 4`?
```python
a = 1
for i in range(4):
    print(a, end=" ")
    ____
```
- A) `a = 4 - a`
- B) `a = a + 3`
- C) `a = a * 4`
- D) `a = 5 - a`

---

## Section D — Choose the Statement or Initialization (Q231–Q238)

**Q231. [E]** Which keyword fills the blank so the code prints `1 2 4 5`?
```python
for i in range(1, 6):
    if i == 3:
        ____
    print(i, end=" ")
```
- A) `break`
- B) `pass`
- C) `continue`
- D) `else`

**Q232. [M]** Which keyword fills the blank so the code prints `1 2` and then `Stop`?
```python
for i in range(1, 6):
    if i == 3:
        ____
    print(i, end=" ")
print("Stop")
```
- A) `break`
- B) `continue`
- C) `pass`
- D) `print(i)`

**Q233. [M]** Which statement fills the blank so the code prints `1 2 3 4` — nothing more, nothing less?
```python
for i in range(1, 5):
    if i == 2:
        ____
    print(i, end=" ")
```
- A) `continue`
- B) `pass`
- C) `break`
- D) `print(i)`

**Q234. [M]** Which initialization fills the blank so the code prints `24`?
```python
p = ____
for i in range(1, 5):
    p = p * i
print(p)
```
- A) `0`
- B) `4`
- C) `i`
- D) `1`

**Q235. [H]** The values read are always between 1 and 99. Which initialization **guarantees** the code finds the smallest value?
```python
small = ____
for k in range(3):
    v = int(input())
    if v < small:
        small = v
print(small)
```
- A) `0`
- B) `1`
- C) `100`
- D) `50`

**Q236. [M]** Which initialization fills the blank so the code prints `0` when 7 is never found?
```python
found = ____
for i in range(2, 11, 2):
    if i == 7:
        found = 1
print(found)
```
- A) `0`
- B) `1`
- C) `7`
- D) `-1`

**Q237. [H]** Which line fills the blank so the code reads numbers until a 0 and prints their sum (for the input 4, 5, 0 it prints `9`)?
```python
t = 0
v = int(input())
while v != 0:
    t = t + v
    ____
print(t)
```
- A) `v = int(input())`
- B) `v = 0`
- C) `t = t + v`
- D) `print(t)`

**Q238. [M]** Which line fills the blank so the stars appear as a 2 × 2 square (two per line)?
```python
for i in range(2):
    for j in range(2):
        print("*", end=" ")
    ____
```
- A) `pass`
- B) `break`
- C) `print(i)`
- D) `print()`

---

## Section E — Complete the Expression (Q239–Q245)

**Q239. [M]** Which expression fills the blank so the code prints `1 4 9 16`?
```python
for i in range(1, 5):
    print(____, end=" ")
```
- A) `i + 3`
- B) `i * 2`
- C) `i * i`
- D) `i * 4`

**Q240. [H]** Which expression fills the blank so the code prints `0 2 6 12`?
```python
for i in range(1, 5):
    print(____, end=" ")
```
- A) `i * i - 1`
- B) `i * (i - 1)`
- C) `i * i`
- D) `2 * i - 2`

**Q241. [H]** Which expression fills the blank so the code prints `1 4 9 6 5`?
```python
for i in range(1, 6):
    print(____, end=" ")
```
- A) `i * i // 10`
- B) `(i * i) % 10`
- C) `i % 10`
- D) `i * i - 10`

**Q242. [M]** Which expression fills the blank so the code prints the pattern shown?
```
1
3 3
5 5 5
```
```python
for i in range(1, 4):
    for j in range(i):
        print(____, end=" ")
    print()
```
- A) `i`
- B) `2 * i + 1`
- C) `i * i`
- D) `2 * i - 1`

**Q243. [M]** Which expression fills the blank so the code prints `20` (the sum 1·2 + 2·3 + 3·4)?
```python
t = 0
for i in range(1, 4):
    t = t + ____
print(t)
```
- A) `i * i + 1`
- B) `i + i + 1`
- C) `i * (i + 1)`
- D) `i * i`

**Q244. [M]** Which condition fills the blank so the code prints the identity pattern shown?
```
1 0 0
0 1 0
0 0 1
```
```python
for i in range(1, 4):
    for j in range(1, 4):
        if ____:
            print(1, end=" ")
        else:
            print(0, end=" ")
    print()
```
- A) `i == j`
- B) `i != j`
- C) `i == 1`
- D) `j == 1`

**Q245. [H]** Which expression fills the blank so the code prints `1 -1 1 -1`?
```python
for i in range(4):
    print(____, end=" ")
```
- A) `i % 2`
- B) `1 - 2 * (i % 2)`
- C) `1 - i % 2`
- D) `2 * (i % 2) - 1`

---

## Section F — Complete for a Target Behavior (Q246–Q250)

**Q246. [E]** Which condition fills the blank so the code prints `hi` exactly **5** times?
```python
c = 0
while ____:
    print("hi")
    c = c + 1
```
- A) `c < 4`
- B) `c < 6`
- C) `c <= 5`
- D) `c < 5`

**Q247. [M]** Which stop value fills the blank so the code prints the 7-times table up to 70?
```python
for j in range(1, ____):
    print(7 * j, end=" ")
```
- A) `10`
- B) `70`
- C) `11`
- D) `7`

**Q248. [M]** Which condition fills the blank so the code prints `15` (the numbers from 1 to 20 **not** divisible by 4)?
```python
c = 0
for i in range(1, 21):
    if ____:
        c = c + 1
print(c)
```
- A) `i % 4 != 0`
- B) `i % 4 == 0`
- C) `i // 4 != 0`
- D) `i % 4 > 1`

**Q249. [M]** Which inner range fills the blank so the code prints the numbers 1 to 12 in order?
```python
n = 1
for i in range(3):
    for j in range(____):
        print(n, end=" ")
        n = n + 1
```
- A) `3`
- B) `4`
- C) `12`
- D) `i`

**Q250. [H]** Which line fills the blank so the code prints the sequence `3 10 5 16 8 4 2 1`?
```python
n = 6
while n != 1:
    if n % 2 == 0:
        n = n // 2
    else:
        ____
    print(n, end=" ")
```
- A) `n = 3 * n`
- B) `n = n + 1`
- C) `n = n * n + 1`
- D) `n = 3 * n + 1`

---

*End of Part 5 — Q201–Q250. Difficulty: 2 [E] · 33 [M] · 15 [H]. Every correct completion — and every near-miss distractor — verified by executing the code.*
