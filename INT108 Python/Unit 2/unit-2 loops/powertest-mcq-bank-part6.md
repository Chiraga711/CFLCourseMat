# Loops MCQ Bank — Part 6: Count the Output & Reverse-Engineer the Code (Q251–Q300)

*Sections A–C: how many stars, values, or lines does the code produce? Sections D–E: which code produces this output?*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `loops-mcq-bank-part6-answers.md`.*

---

## Section A — How Many Stars? (Q251–Q262)

**Q251. [E]** How many stars does this print in total?
```python
for i in range(0, 6, 2):
    for j in range(4):
        print("*", end=" ")
```
- A) `12`
- B) `10`
- C) `24`
- D) `8`

**Q252. [M]** How many stars does this print in total?
```python
for i in range(1, 6):
    for j in range(i + 2):
        print("*", end=" ")
    print()
```
- A) `15`
- B) `20`
- C) `25`
- D) `35`

**Q253. [M]** How many **dots** does this print in total?
```python
for i in range(1, 5):
    for j in range(5 - i):
        print(".", end=" ")
    for k in range(i):
        print("*", end=" ")
    print()
```
- A) `6`
- B) `10`
- C) `16`
- D) `4`

**Q254. [M]** How many stars does this print in total?
```python
for i in range(4):
    for j in range(4):
        if (i + j) % 2 == 0:
            print("*", end=" ")
```
- A) `16`
- B) `4`
- C) `12`
- D) `8`

**Q255. [H]** How many stars does this print in total?
```python
for i in range(1, 5):
    for j in range(1, 5):
        if j > 4 - i:
            break
        print("*", end=" ")
    print()
```
- A) `16`
- B) `10`
- C) `6`
- D) `12`

**Q256. [M]** How many stars does this print in total?
```python
for i in range(1, 6):
    for j in range(1, 6):
        if i == 1 or i == 5 or j == 1 or j == 5:
            print("*", end=" ")
    print()
```
- A) `16`
- B) `25`
- C) `20`
- D) `9`

**Q257. [M]** How many stars does this print in total?
```python
for i in range(1, 4):
    for j in range(i):
        print("*", end=" ")
    print()
for i in range(2, 0, -1):
    for j in range(i):
        print("*", end=" ")
    print()
```
- A) `6`
- B) `12`
- C) `10`
- D) `9`

**Q258. [H]** How many stars does this print in total?
```python
for i in range(3):
    k = i
    while k < 5:
        print("*", end=" ")
        k = k + 2
```
- A) `6`
- B) `7`
- C) `9`
- D) `5`

**Q259. [M]** How many stars does this print in total?
```python
for i in range(1, 4):
    for j in range(i):
        for k in range(3):
            print("*", end=" ")
```
- A) `18`
- B) `6`
- C) `9`
- D) `12`

**Q260. [M]** How many stars does this print in total?
```python
for i in range(5):
    for j in range(5):
        if (i * j) % 2 == 1:
            continue
        print("*", end=" ")
```
- A) `25`
- B) `16`
- C) `12`
- D) `21`

**Q261. [M]** How many stars does this print in total?
```python
for i in range(1, 5):
    for j in range(i, 6):
        print("*", end=" ")
    print()
```
- A) `20`
- B) `14`
- C) `10`
- D) `18`

**Q262. [H]** How many stars does this print in total?
```python
for i in range(3):
    for j in range(3):
        print("*", end=" ")
for i in range(2, 6, 2):
    for j in range(2):
        print("*", end=" ")
```
- A) `9`
- B) `17`
- C) `13`
- D) `11`

---

## Section B — How Many Values? (Q263–Q272)

**Q263. [M]** How many numbers does this print?
```python
n = 45
while n > 3:
    print(n)
    n = n // 2
```
- A) `3`
- B) `6`
- C) `5`
- D) `4`

**Q264. [M]** How many numbers does this print?
```python
for i in range(1, 16):
    if i % 4 == 0:
        continue
    print(i)
```
- A) `15`
- B) `12`
- C) `3`
- D) `11`

**Q265. [H]** How many **different** numbers appear in the output?
```python
for i in range(1, 4):
    for j in range(1, 4):
        print(i * j, end=" ")
```
- A) `6`
- B) `9`
- C) `8`
- D) `5`

**Q266. [M]** How many numbers does this print?
```python
for i in range(2, 30):
    if i % 3 == 0 and i % 4 == 0:
        print(i)
```
- A) `9`
- B) `14`
- C) `2`
- D) `4`

**Q267. [H]** How many numbers does this print?
```python
n = 1
for i in range(3):
    while n < i * 4:
        print(n)
        n = n + 3
```
- A) `4`
- B) `3`
- C) `6`
- D) `2`

**Q268. [M]** How many **even** numbers does this print?
```python
for i in range(1, 5):
    for j in range(1, 4):
        print(i + j, end=" ")
```
- A) `12`
- B) `3`
- C) `5`
- D) `6`

**Q269. [E]** How many numbers does this print?
```python
for i in range(1, 6):
    if i * i > 10:
        break
    print(i)
```
- A) `5`
- B) `4`
- C) `3`
- D) `10`

**Q270. [M]** How many numbers appear in the output in total?
```python
for i in range(2, 9, 3):
    print(i)
print(i)
```
- A) `4`
- B) `3`
- C) `5`
- D) `8`

**Q271. [M]** With the inputs 7, 3, 9, 0, 5 (one per line), how many numbers does this print?
```python
v = int(input())
while v != 0:
    print(v)
    v = int(input())
```
- A) `5`
- B) `4`
- C) `0`
- D) `3`

**Q272. [M]** How many **odd** numbers does this print?
```python
for i in range(1, 6):
    for j in range(1, 6):
        print(i * j, end=" ")
```
- A) `25`
- B) `9`
- C) `12`
- D) `6`

---

## Section C — How Many Lines? (Q273–Q278)

**Q273. [E]** How many lines of output does this produce?
```python
for i in range(0, 10, 3):
    for j in range(2):
        print(j, end=" ")
    print()
```
- A) `10`
- B) `3`
- C) `4`
- D) `5`

**Q274. [M]** How many lines of output does this produce?
```python
for i in range(2):
    for j in range(3):
        print("*")
```
- A) `6`
- B) `2`
- C) `3`
- D) `1`

**Q275. [M]** How many lines of output does this produce?
```python
for i in range(1, 22):
    if i % 4 == 0:
        print(i)
```
- A) `21`
- B) `4`
- C) `6`
- D) `5`

**Q276. [H]** How many lines of output does this produce?
```python
for i in range(3):
    print(i, end=" ")
    if i % 2 == 0:
        print()
```
- A) `3`
- B) `2`
- C) `1`
- D) `4`

**Q277. [M]** How many lines of output does this produce?
```python
for i in range(4):
    for j in range(i - 1):
        print(j)
```
- A) `3`
- B) `6`
- C) `4`
- D) `0`

**Q278. [M]** How many lines of output does this produce?
```python
n = 81
while n > 1:
    print(n)
    n = n // 3
```
- A) `5`
- B) `3`
- C) `4`
- D) `81`

---

## Section D — Which Code Prints This? Patterns (Q279–Q290)

**Q279. [M]** Which code prints this?
```
0 1 2 3
0 1 2 3
0 1 2 3
```
- A)
  ```python
  for i in range(4):
      for j in range(3):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(3):
      for j in range(4):
          print(j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(3):
      for j in range(4):
          print(i, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(3):
      for j in range(1, 4):
          print(j, end=" ")
      print()
  ```

**Q280. [M]** Which code prints this?
```
1
2 2
3 3 3
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(1, i):
          print(i, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(j + 1, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(i, end=" ")
      print()
  ```

**Q281. [M]** Which code prints this?
```
5 5 5
5 5
5
```
- A)
  ```python
  for i in range(3, 0, -1):
      for j in range(i):
          print(5, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(5, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(3, 0, -1):
      for j in range(5 - i):
          print(5, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(3, 0, -1):
      for j in range(i):
          print(i, end=" ")
      print()
  ```

**Q282. [H]** Which code prints this?
```
1
1 2
1 2 3
1 2
1
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  for i in range(3, 0, -1):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  for i in range(2, 0, -1):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(1, i + 1):
          print(j, end=" ")
      print()
  for i in range(2, 0, -1):
      for j in range(i, 0, -1):
          print(j, end=" ")
      print()
  ```

**Q283. [M]** Which code prints this?
```
. . *
. * .
* . .
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          if i == j:
              print("*", end=" ")
          else:
              print(".", end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          if i + j == 3:
              print("*", end=" ")
          else:
              print(".", end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          if i * j == 3:
              print("*", end=" ")
          else:
              print(".", end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          if i + j == 4:
              print("*", end=" ")
          else:
              print(".", end=" ")
      print()
  ```

**Q284. [M]** Which code prints this?
```
7 7 7 7
7 7 7 7
```
- A)
  ```python
  for i in range(2):
      for j in range(4):
          print(i, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(2):
      for j in range(4):
          print(7, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(2):
      for j in range(4):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(4):
      for j in range(2):
          print(7, end=" ")
      print()
  ```

**Q285. [H]** Which code prints this?
```
1 3 5
1 3 5
```
- A)
  ```python
  for i in range(2):
      for j in range(1, 5, 2):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(2):
      for j in range(0, 6, 2):
          print(j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(2):
      for j in range(1, 6, 2):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(3):
      for j in range(1, 6, 2):
          print(j, end=" ")
      print()
  ```

**Q286. [M]** Which code prints this?
```
1
2
3
1
2
3
```
- A)
  ```python
  for i in range(2):
      for j in range(1, 4):
          print(j)
  ```
- B)
  ```python
  for i in range(2):
      for j in range(1, 4):
          print(j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(3):
      for j in range(1, 3):
          print(j)
  ```
- D)
  ```python
  for i in range(2):
      for j in range(1, 4):
          print(i)
  ```

**Q287. [H]** Which code prints this?
```
2 4
4 8
6 12
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(1, 3):
          print(i * j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(2, 7, 2):
      for j in range(1, 4):
          print(i * j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(2, 8, 3):
      for j in range(1, 3):
          print(i * j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(2, 7, 2):
      for j in range(1, 3):
          print(i * j, end=" ")
      print()
  ```

**Q288. [M]** Which code prints this?
```
8 6 4 2
```
- A)
  ```python
  for i in range(8, 2, -2):
      print(i, end=" ")
  ```
- B)
  ```python
  for i in range(8, 0, -2):
      print(i, end=" ")
  ```
- C)
  ```python
  for i in range(2, 9, 2):
      print(i, end=" ")
  ```
- D)
  ```python
  for i in range(8, 0, -3):
      print(i, end=" ")
  ```

**Q289. [M]** Which code prints this?
```
. . 1
. 2 2
3 3 3
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(".", end=" ")
      for k in range(3 - i):
          print(i, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(i):
          print(i, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(3 - i):
          print(".", end=" ")
      for k in range(i):
          print(i, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(3 - i):
          print(".", end=" ")
      for k in range(i):
          print(k + 1, end=" ")
      print()
  ```

**Q290. [H]** Which code prints this?
```
1 2
2 3
3 4
```
- A)
  ```python
  for i in range(1, 4):
      for j in range(i, i + 2):
          print(j, end=" ")
      print()
  ```
- B)
  ```python
  for i in range(1, 4):
      for j in range(i - 1, i + 1):
          print(j, end=" ")
      print()
  ```
- C)
  ```python
  for i in range(1, 4):
      for j in range(1, 3):
          print(j, end=" ")
      print()
  ```
- D)
  ```python
  for i in range(1, 4):
      for j in range(i, i + 1):
          print(j, end=" ")
      print()
  ```

---

## Section E — Which Code Prints This? Sequences (Q291–Q300)

**Q291. [M]** Which code prints `2 5 8 11 14`?
- A)
  ```python
  for i in range(2, 14, 3):
      print(i, end=" ")
  ```
- B)
  ```python
  for i in range(3, 15, 3):
      print(i, end=" ")
  ```
- C)
  ```python
  for i in range(2, 15, 2):
      print(i, end=" ")
  ```
- D)
  ```python
  for i in range(2, 15, 3):
      print(i, end=" ")
  ```

**Q292. [M]** Which code prints `1 2 4 8 16 32`?
- A)
  ```python
  p = 1
  while p <= 32:
      print(p, end=" ")
      p = p * 2
  ```
- B)
  ```python
  p = 1
  while p < 32:
      print(p, end=" ")
      p = p * 2
  ```
- C)
  ```python
  p = 1
  while p <= 32:
      print(p, end=" ")
      p = p + 2
  ```
- D)
  ```python
  for i in range(6):
      print(2 * i, end=" ")
  ```

**Q293. [H]** Which code prints `1 1 2 3 5 8`?
- A)
  ```python
  a = 1
  b = 1
  for i in range(6):
      print(b, end=" ")
      t = a + b
      a = b
      b = t
  ```
- B)
  ```python
  a = 1
  b = 1
  for i in range(6):
      print(a, end=" ")
      t = a + b
      a = b
      b = t
  ```
- C)
  ```python
  a = 1
  b = 1
  for i in range(6):
      print(a, end=" ")
      t = a + b
      a = t
      b = t
  ```
- D)
  ```python
  a = 0
  b = 1
  for i in range(6):
      print(a, end=" ")
      t = a + b
      a = b
      b = t
  ```

**Q294. [M]** Which code prints `100 50 25 12 6 3 1`?
- A)
  ```python
  n = 100
  while n > 1:
      print(n, end=" ")
      n = n // 2
  ```
- B)
  ```python
  n = 100
  while n > 0:
      print(n, end=" ")
      n = n / 2
  ```
- C)
  ```python
  n = 100
  while n > 0:
      print(n, end=" ")
      n = n // 2
  ```
- D)
  ```python
  n = 100
  while n >= 0:
      print(n, end=" ")
      n = n // 2
  ```

**Q295. [M]** Which code prints `3 6 9 12`?
- A)
  ```python
  for i in range(3, 13, 3):
      print(i, end=" ")
  ```
- B)
  ```python
  for i in range(3, 12, 3):
      print(i, end=" ")
  ```
- C)
  ```python
  for i in range(0, 13, 3):
      print(i, end=" ")
  ```
- D)
  ```python
  for i in range(3, 15, 4):
      print(i, end=" ")
  ```

**Q296. [H]** Which code prints `2 6 12 20`?
- A)
  ```python
  for i in range(1, 5):
      print(i * i + 1, end=" ")
  ```
- B)
  ```python
  for i in range(1, 5):
      print(4 * i - 2, end=" ")
  ```
- C)
  ```python
  for i in range(1, 5):
      print(i * i + 2, end=" ")
  ```
- D)
  ```python
  for i in range(1, 5):
      print(i * (i + 1), end=" ")
  ```

**Q297. [M]** Which code prints `5 3 1 -1`?
- A)
  ```python
  for i in range(5, 0, -2):
      print(i, end=" ")
  ```
- B)
  ```python
  for i in range(5, -2, -2):
      print(i, end=" ")
  ```
- C)
  ```python
  for i in range(5, -1, -2):
      print(i, end=" ")
  ```
- D)
  ```python
  for i in range(-1, 6, 2):
      print(i, end=" ")
  ```

**Q298. [H]** Which code prints `0 1 3 6 10`?
- A)
  ```python
  t = 0
  for i in range(5):
      t = t + i + 1
      print(t, end=" ")
  ```
- B)
  ```python
  t = 0
  for i in range(5):
      print(t, end=" ")
      t = t + i
  ```
- C)
  ```python
  t = 0
  for i in range(5):
      print(t, end=" ")
      t = t + i + 1
  ```
- D)
  ```python
  t = 0
  for i in range(5):
      print(t, end=" ")
      t = t + 2
  ```

**Q299. [M]** Which code prints `1 10 100 1000`?
- A)
  ```python
  p = 1
  while p < 1000:
      print(p, end=" ")
      p = p * 10
  ```
- B)
  ```python
  for i in range(4):
      print(10 * i, end=" ")
  ```
- C)
  ```python
  p = 10
  while p <= 1000:
      print(p, end=" ")
      p = p * 10
  ```
- D)
  ```python
  p = 1
  while p <= 1000:
      print(p, end=" ")
      p = p * 10
  ```

**Q300. [H]** Which code prints `1 2 4 5 7 8`?
- A)
  ```python
  for i in range(1, 9):
      if i % 3 != 0:
          continue
      print(i, end=" ")
  ```
- B)
  ```python
  for i in range(1, 9):
      if i % 3 == 0:
          continue
      print(i, end=" ")
  ```
- C)
  ```python
  for i in range(1, 9):
      if i % 3 == 0:
          break
      print(i, end=" ")
  ```
- D)
  ```python
  for i in range(1, 9):
      if i % 3 == 1:
          print(i, end=" ")
  ```

---

*End of Part 6 — Q251–Q300. Difficulty: 3 [E] · 33 [M] · 14 [H]. Every count and every correct option verified by executing the code; near-twin options were executed too and excluded where they matched.*
