# Functions & Recursion — Final MCQ Bank, Batch 6 (Q246–Q285)

*Bonus set: Recursion dry-run (neutral function names). 40 trace questions with names like `fun`, `solve`, `calc`, `process` that don't reveal the logic — you must trace the recursion by hand.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch6-answers.md`.*

---

**Q246. [M]** What does this print?
```python
def fun(n):
    if n <= 1:
        return 2
    return n + fun(n - 2)

print(fun(6))
```
- A) `14`
- B) `10`
- C) `12`
- D) `16`

**Q247. [H]** What does this print?
```python
def solve(n):
    if n == 0:
        return 0
    if n % 2 == 0:
        return solve(n - 1) + n
    return solve(n - 1) - n

print(solve(5))
```
- A) `3`
- B) `-3`
- C) `-5`
- D) `5`

**Q248. [M]** What does this print?
```python
def calc(n):
    if n < 10:
        return n + 1
    return (n % 10) + calc(n // 10)

print(calc(234))
```
- A) `8`
- B) `9`
- C) `10`
- D) `12`

**Q249. [H]** What does this print?
```python
def process(a, b):
    if b == 0:
        return a
    return process(b, a % b) + 1

print(process(20, 6))
```
- A) `2`
- B) `6`
- C) `8`
- D) `4`

**Q250. [M]** What does this print?
```python
def compute(n):
    if n <= 0:
        return 1
    return n * compute(n - 2)

print(compute(6))
```
- A) `48`
- B) `24`
- C) `36`
- D) `720`

**Q251. [H]** What does this print?
```python
def test(n):
    if n == 1:
        return 3
    return test(n - 1) * 2 - 1

print(test(4))
```
- A) `13`
- B) `17`
- C) `15`
- D) `19`

**Q252. [H]** What does this print?
```python
def check(n):
    if n == 0:
        return 0
    return (n % 2) + check(n // 2)

print(check(13))
```
- A) `2`
- B) `4`
- C) `3`
- D) `5`

**Q253. [H]** What does this print?
```python
def find(n):
    if n <= 2:
        return n
    return find(n - 1) + find(n - 3)

print(find(6))
```
- A) `5`
- B) `6`
- C) `8`
- D) `7`

**Q254. [H]** What does this print?
```python
def output(x):
    if x < 5:
        return x
    if x % 2 == 0:
        return output(x // 2) + 2
    return output(x - 3) + 1

print(output(18))
```
- A) `8`
- B) `6`
- C) `7`
- D) `9`

**Q255. [M]** What does this print?
```python
def value(n):
    if n == 0:
        return 1
    return value(n - 1) + n * n

print(value(3))
```
- A) `13`
- B) `15`
- C) `14`
- D) `16`

**Q256. [H]** What does this print?
```python
def action(n):
    if n <= 1:
        return n
    return action(n // 2) + action(n - 2)

print(action(7))
```
- A) `3`
- B) `4`
- C) `5`
- D) `6`

**Q257. [M]** What does this print?
```python
def result(a, b):
    if b == 1:
        return a
    return a + result(a, b - 1)

print(result(3, 4))
```
- A) `9`
- B) `10`
- C) `15`
- D) `12`

**Q258. [M]** What does this print?
```python
def task(n):
    if n == 0:
        return 0
    if n % 10 > 5:
        return 1 + task(n // 10)
    return task(n // 10)

print(task(7862))
```
- A) `3`
- B) `1`
- C) `2`
- D) `4`

**Q259. [H]** What does this print?
```python
def logic(n):
    if n <= 0:
        return 0
    return n + logic(n - 1) - logic(n - 2)

print(logic(4))
```
- A) `4`
- B) `6`
- C) `5`
- D) `7`

**Q260. [H]** What does this print?
```python
def work(n):
    if n == 1:
        return 1
    if n % 2 == 0:
        return work(n - 1) * 2
    return work(n - 1) + 3

print(work(5))
```
- A) `10`
- B) `11`
- C) `13`
- D) `15`

**Q261. [M]** What does this print?
```python
def count(n):
    if n < 10:
        return n % 2
    return (n % 2) + count(n // 10)

print(count(5724))
```
- A) `1`
- B) `3`
- C) `4`
- D) `2`

**Q262. [M]** What does this print?
```python
def number(n):
    if n <= 1:
        return 1
    return n + number(n // 2)

print(number(10))
```
- A) `18`
- B) `15`
- C) `16`
- D) `20`

**Q263. [H]** What does this print?
```python
def modify(n):
    if n == 0:
        return 0
    return 10 * modify(n // 10) + (n % 10) + 1

print(modify(123))
```
- A) `123`
- B) `234`
- C) `224`
- D) `345`

**Q264. [M]** What does this print?
```python
def collect(n):
    if n == 0:
        return 0
    if n % 3 == 0:
        return n + collect(n - 1)
    return collect(n - 1)

print(collect(10))
```
- A) `12`
- B) `15`
- C) `18`
- D) `21`

**Q265. [H]** What does this print?
```python
def sample(n):
    if n <= 1:
        return 1
    return sample(n - 1) + 2 * sample(n - 2)

print(sample(5))
```
- A) `15`
- B) `18`
- C) `24`
- D) `21`

**Q266. [H]** What does this print?
```python
def fun(n):
    if n <= 0:
        return 2
    if n % 2 == 0:
        return n + fun(n - 3)
    return n * fun(n - 2)

print(fun(6))
```
- A) `12`
- B) `10`
- C) `14`
- D) `18`

**Q267. [H]** What does this print?
```python
def solve(n):
    if n == 0:
        return 1
    if n % 3 == 0:
        return solve(n - 1) + n
    return solve(n - 1) + (n % 3)

print(solve(5))
```
- A) `8`
- B) `10`
- C) `9`
- D) `12`

**Q268. [H]** What does this print?
```python
def calc(n):
    if n < 10:
        return n
    if (n % 10) % 2 == 0:
        return calc(n // 10) + (n % 10)
    return calc(n // 10) - (n % 10)

print(calc(4825))
```
- A) `7`
- B) `8`
- C) `9`
- D) `10`

**Q269. [H]** What does this print?
```python
def process(a, b):
    if b == 0:
        return 0
    if b % 2 == 0:
        return a + process(a, b - 1)
    return process(a, b - 1) - a

print(process(3, 4))
```
- A) `-3`
- B) `3`
- C) `6`
- D) `0`

**Q270. [H]** What does this print?
```python
def compute(n):
    if n <= 1:
        return n + 1
    return compute(n - 1) + compute(n - 2) + 1

print(compute(4))
```
- A) `12`
- B) `9`
- C) `10`
- D) `15`

**Q271. [H]** What does this print?
```python
def check(n):
    if n == 0:
        return 0
    r = n % 10
    if r > 4:
        return r + check(n // 10)
    return check(n // 10) - r

print(check(5832))
```
- A) `6`
- B) `8`
- C) `7`
- D) `10`

**Q272. [H]** What does this print?
```python
def task(n):
    if n <= 0:
        return 1
    if n % 2 == 0:
        return task(n - 1) + task(n - 2)
    return task(n - 1) + 2

print(task(5))
```
- A) `9`
- B) `10`
- C) `12`
- D) `14`

**Q273. [M]** What does this print?
```python
def result(n):
    if n == 1:
        return 4
    return n * 2 + result(n - 1)

print(result(4))
```
- A) `18`
- B) `20`
- C) `24`
- D) `22`

**Q274. [H]** What does this print?
```python
def output(n):
    if n < 3:
        return n
    if n % 2 == 0:
        return output(n // 2) + output(n - 1)
    return output(n - 1) - output(n - 2)

print(output(6))
```
- A) `3`
- B) `2`
- C) `4`
- D) `5`

**Q275. [M]** What does this print?
```python
def value(n):
    if n == 0:
        return 0
    return (n % 10) * 2 + value(n // 10)

print(value(314))
```
- A) `12`
- B) `16`
- C) `14`
- D) `18`

**Q276. [H]** What does this print?
```python
def number(x):
    if x < 2:
        return 3
    return x + number(x // 2) - 1

print(number(20))
```
- A) `30`
- B) `33`
- C) `36`
- D) `40`

**Q277. [H]** What does this print?
```python
def modify(n):
    if n == 0:
        return 1
    if n % 2 == 0:
        return n * modify(n - 2)
    return n + modify(n - 1)

print(modify(5))
```
- A) `11`
- B) `12`
- C) `15`
- D) `13`

**Q278. [H]** What does this print?
```python
def logic(n):
    if n <= 1:
        return 1
    return logic(n - 1) * 2 + n

print(logic(4))
```
- A) `26`
- B) `20`
- C) `22`
- D) `24`

**Q279. [H]** What does this print?
```python
def count(n):
    if n < 10:
        return n
    last = n % 10
    rest = count(n // 10)
    if last > rest:
        return last
    return rest

print(count(90901))
```
- A) `1`
- B) `9`
- C) `0`
- D) `5`

**Q280. [H]** What does this print?
```python
def action(n):
    if n <= 0:
        return 0
    if n % 4 == 0:
        return n + action(n - 3)
    return action(n - 1) + 1

print(action(8))
```
- A) `10`
- B) `12`
- C) `14`
- D) `16`

**Q281. [H]** What does this print?
```python
def sample(n):
    if n == 0:
        return 0
    return sample(n // 10) * 10 + (n % 10) - 1

print(sample(456))
```
- A) `234`
- B) `456`
- C) `567`
- D) `345`

**Q282. [H]** What does this print?
```python
def test(n):
    if n <= 1:
        return 2
    if n % 2 == 0:
        return test(n - 1) + n
    return test(n - 2) + n

print(test(7))
```
- A) `17`
- B) `13`
- C) `15`
- D) `19`

**Q283. [H]** What does this print?
```python
def work(a, b):
    if a < b:
        return b - a
    return 1 + work(a - b, b)

print(work(17, 5))
```
- A) `4`
- B) `6`
- C) `5`
- D) `7`

**Q284. [M]** What does this print?
```python
def solve(n):
    if n <= 0:
        return 0
    return n % 5 + solve(n - 2)

print(solve(9))
```
- A) `8`
- B) `9`
- C) `10`
- D) `12`

**Q285. [H]** What does this print?
```python
def final(n):
    if n <= 2:
        return n
    return final(n - 1) + final(n - 2) - final(n - 3)

print(final(6))
```
- A) `4`
- B) `5`
- C) `7`
- D) `6`

---

*End of Batch 6 — Q246–Q285. Difficulty: 0 [E] · 12 [M] · 28 [H]. Every answer verified by executing the code.*