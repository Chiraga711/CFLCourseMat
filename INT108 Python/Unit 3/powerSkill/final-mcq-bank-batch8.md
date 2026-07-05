# Functions & Recursion — Final MCQ Bank, Batch 8 (Q308–Q328)

*Bonus set: Code Arrangement. Each question gives the lines of a short program.*
*Each program's lines are shown **flush-left with the indentation removed and in scrambled order** — you must work out both the correct sequence **and** the correct indentation (nesting) from the logic. The option gives the order of the numbered lines.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch8-answers.md`.*

---

**Q308. [M]** Arrange the lines to make a program that prints `6`.
```
1. return s
2. print(find_sum(3))
3. s = s + i
4. def find_sum(n):
5. for i in range(1, n + 1):
6. s = 0
```
- A) 4, 6, 5, 3, 1, 2
- B) 4, 5, 6, 3, 1, 2
- C) 6, 4, 5, 3, 1, 2
- D) 4, 6, 3, 5, 1, 2

**Q309. [E]** Arrange the lines to make a program that prints `24`.
```
1. print(multiply(c=4, a=2, b=3))
2. def multiply(a, b, c):
3. return a * b * c
```
- A) 1, 2, 3
- B) 2, 3, 1
- C) 3, 1, 2
- D) 2, 1, 3

**Q310. [H]** Arrange the lines to make a program that prints `3`.
```
1. count = 0
2. print(count_even(6))
3. def count_even(n):
4. for i in range(1, n + 1):
5. count = count + 1
6. if i % 2 == 0:
7. return count
```
- A) 3, 4, 1, 6, 5, 7, 2
- B) 1, 3, 4, 6, 5, 7, 2
- C) 3, 1, 4, 6, 5, 7, 2
- D) 3, 1, 6, 4, 5, 7, 2

**Q311. [M]** Arrange the lines to make a program that prints `Greater`.
```
1. if a > b:
2. print(compare(9, 4))
3. def compare(a, b):
4. return "Greater"
5. else:
6. return "Smaller"
```
- A) 1, 4, 5, 6, 3, 2
- B) 3, 5, 6, 1, 4, 2
- C) 2, 3, 1, 4, 5, 6
- D) 3, 1, 4, 5, 6, 2

**Q312. [H]** Arrange the lines to make a program that prints `10`.
```
1. for i in range(1, n + 1):
2. print(nested_sum(3))
3. total = total + j
4. total = 0
5. for j in range(1, i + 1):
6. return total
7. def nested_sum(n):
```
- A) 7, 4, 1, 5, 3, 6, 2
- B) 7, 1, 5, 4, 3, 6, 2
- C) 4, 7, 1, 5, 3, 6, 2
- D) 7, 4, 5, 1, 3, 6, 2

**Q313. [E]** Arrange the lines to make a program that prints `12`.
```
1. print(area(4))
2. def area(a, b=3):
3. return a * b
```
- A) 3, 2, 1
- B) 2, 3, 1
- C) 2, 1, 3
- D) 1, 2, 3

**Q314. [M]** Arrange the lines to make a program that prints `24`.
```
1. return 1
2. def fact(n):
3. if n == 0:
4. return n * fact(n - 1)
5. print(fact(4))
```
- A) 2, 1, 3, 4, 5
- B) 3, 1, 4, 2, 5
- C) 2, 3, 1, 4, 5
- D) 2, 3, 4, 1, 5

**Q315. [M]** Arrange the lines to make a program that prints `8`.
```
1. print(max_two(3, 8))
2. def max_two(a, b):
3. if a > b:
4. return a
5. return b
```
- A) 2, 4, 3, 5, 1
- B) 2, 3, 5, 4, 1
- C) 3, 2, 4, 5, 1
- D) 2, 3, 4, 5, 1

**Q316. [M]** Arrange the lines to make a program that prints `78.54`.
```
1. return math.pi * r * r
2. import math
3. print(round(area(5), 2))
4. def area(r):
```
- A) 2, 4, 1, 3
- B) 4, 2, 1, 3
- C) 2, 1, 4, 3
- D) 2, 4, 3, 1

**Q317. [H]** Arrange the lines to make a program that prints `9`.
```
1. c = c + 1
2. return c
3. c = 0
4. for i in range(n):
5. print(grid(3))
6. for j in range(n):
7. def grid(n):
```
- A) 7, 4, 3, 6, 1, 2, 5
- B) 7, 3, 4, 6, 1, 2, 5
- C) 7, 3, 6, 4, 1, 2, 5
- D) 7, 3, 4, 1, 6, 2, 5

**Q318. [M]** Arrange the lines to make a program that prints `15`.
```
1. if n == 0:
2. print(sum_to(5))
3. return 0
4. return n + sum_to(n - 1)
5. def sum_to(n):
```
- A) 5, 3, 1, 4, 2
- B) 5, 1, 4, 3, 2
- C) 5, 1, 3, 4, 2
- D) 1, 5, 3, 4, 2

**Q319. [H]** Arrange the lines to make a program that prints `8`.
```
1. return r
2. r = 1
3. print(power(2, 3))
4. for i in range(e):
5. def power(b, e=2):
6. r = r * b
```
- A) 5, 4, 2, 6, 1, 3
- B) 5, 2, 6, 4, 1, 3
- C) 5, 2, 4, 1, 6, 3
- D) 5, 2, 4, 6, 1, 3

**Q320. [E]** Arrange the lines to make a program that prints `4`.
```
1. return a // b
2. def divide(a, b):
3. print(divide(b=3, a=12))
```
- A) 2, 1, 3
- B) 1, 2, 3
- C) 2, 3, 1
- D) 3, 2, 1

**Q321. [E]** Arrange the lines to make a program that prints `20`.
```
1. n = n * 2
2. return n
3. print(double(10))
4. def double(n):
```
- A) 4, 2, 1, 3
- B) 4, 1, 2, 3
- C) 1, 4, 2, 3
- D) 4, 1, 3, 2

**Q322. [M]** Arrange the lines to make a program that prints `5`.
```
1. def boxes(items, cap):
2. print(boxes(23, 5))
3. import math
4. return math.ceil(items / cap)
```
- A) 1, 3, 4, 2
- B) 3, 4, 1, 2
- C) 3, 1, 4, 2
- D) 3, 1, 2, 4

**Q323. [H]** Arrange the lines to make a program that prints `6`.
```
1. return total
2. total = total + 1
3. total = 0
4. for i in range(1, n + 1):
5. for j in range(1, i + 1):
6. def tri(n):
7. print(tri(3))
```
- A) 6, 4, 3, 5, 2, 1, 7
- B) 6, 3, 5, 4, 2, 1, 7
- C) 6, 3, 4, 5, 1, 2, 7
- D) 6, 3, 4, 5, 2, 1, 7

**Q324. [M]** Arrange the lines to make a program that prints `6`.
```
1. return n % 10 + dsum(n // 10)
2. def dsum(n):
3. print(dsum(123))
4. return 0
5. if n == 0:
```
- A) 2, 5, 4, 1, 3
- B) 2, 4, 5, 1, 3
- C) 2, 5, 1, 4, 3
- D) 5, 2, 4, 1, 3

**Q325. [M]** Arrange the lines to make a program that prints `Even`.
```
1. if n % 2 == 0:
2. return "Odd"
3. print(label(8))
4. def label(n):
5. return "Even"
```
- A) 4, 5, 1, 2, 3
- B) 4, 1, 5, 2, 3
- C) 4, 1, 2, 5, 3
- D) 1, 4, 5, 2, 3

**Q326. [H]** Arrange the lines to make a program that prints `4321`.
```
1. def rev(n):
2. while n > 0:
3. r = r * 10 + n % 10
4. print(rev(1234))
5. r = 0
6. return r
7. n = n // 10
```
- A) 1, 2, 5, 3, 7, 6, 4
- B) 1, 5, 3, 2, 7, 6, 4
- C) 1, 5, 2, 3, 7, 6, 4
- D) 1, 5, 2, 7, 3, 6, 4

**Q327. [H]** Arrange the lines to make a program that prints `6`.
```
1. def gcd(a, b):
2. return gcd(b, a % b)
3. print(gcd(48, 18))
4. if b == 0:
5. return a
```
- A) 1, 5, 4, 2, 3
- B) 1, 4, 2, 5, 3
- C) 4, 1, 5, 2, 3
- D) 1, 4, 5, 2, 3

**Q328. [M]** Arrange the lines to make a program that prints `11`.
```
1. return a + b * c
2. print(calc(c=2, a=3, b=4))
3. def calc(a, b, c):
```
- A) 3, 1, 2
- B) 1, 3, 2
- C) 3, 2, 1
- D) 2, 3, 1

---

*End of Batch 8 — Q308–Q328. Difficulty: 4 [E] · 10 [M] · 7 [H]. Every answer verified by executing the code.*