# Test 1 — Function Fundamentals

**Unit 3 · Functions and Recursion — covers Topics 01–03 (Why Functions, Built-in Functions, User-Defined Functions)**

*Section A: 10 multiple-choice questions (1 mark each).*
*Section B: 10 coding problems (3 marks each).*
*Total: 40 marks. Answer key in the separate file `test-01-function-fundamentals-answers.md`.*

---

## Section A — Multiple Choice (10 × 1 = 10 marks)

**A1.** A programmer fixes one line inside a function, and every place that calls the function is instantly corrected. Which advantage of functions does this show?
- A) Code reusability
- B) Easy debugging
- C) Faster execution
- D) Better readability

**A2.** What is `int(9.8)`?
- A) `9`
- B) `9.8`
- C) `10`
- D) An error

**A3.** What does `print(type(input()))` show when the user types `50`?
- A) `<class 'int'>`
- B) `<class 'float'>`
- C) `<class 'str'>`
- D) `50`

**A4.** What is `max(2, 7, 7, 1)`?
- A) `2`
- B) `17`
- C) `1`
- D) `7`

**A5.** What does this print?
```python
def a():
    print("a")

def b():
    print("b")

b()
a()
```
- A) `a b`
- B) `b a`
- C) `a a`
- D) An error

**A6.** What is `round(4.5)`? (Remember Python's rounding rule for exact halves.)
- A) `4`
- B) `4.5`
- C) `5`
- D) An error

**A7.** Which of these is a **valid** function name?
- A) `2marks`
- B) `total marks`
- C) `_score2`
- D) `total-marks`

**A8.** What happens when this runs?
```python
f()

def f():
    print("hi")
```
- A) It prints `hi`
- B) It prints nothing
- C) It prints `hi` twice
- D) An error — `f` is called before it is defined

**A9.** What is `sum([2, 4, 6, 8])`?
- A) `2468`
- B) `20`
- C) An error
- D) `[20]`

**A10.** Defining a function (without calling it) runs its body:
- A) Once
- B) Once per line
- C) Twice
- D) Never

---

## Section B — Coding (10 × 3 = 30 marks)

*Platform-judge format: exact-match output. Read input with `input()`; where a whole number is expected, convert with `int()`. Where a problem names a **Required function**, you must define that function with the exact name and signature given and call it — this will be checked when your code is reviewed. Problems without a named function (B1, B2, B3, B6) may be solved directly with built-in functions.*

---

### B1 — Sum of Two, Rounded

**Task:** Read two floats, one per line, and print their sum rounded to 2 decimal places.

**Input Format:** Two floats, each on its own line.

**Output Format:** The sum of the two values, rounded to 2 decimal places.

**Sample Input:**
```
2.5
3.75
```
**Sample Output:**
```
6.25
```

---

### B2 — Smallest of Four

**Task:** Read four integers, one per line, and print the smallest.

**Input Format:** Four integers, each on its own line.

**Output Format:** A single integer — the smallest of the four.

**Sample Input:**
```
14
9
23
6
```
**Sample Output:**
```
6
```

---

### B3 — Last Digit

**Task:** Read an integer and print its last (units) digit.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the last digit of `n`.

**Sample Input:**
```
80425
```
**Sample Output:**
```
5
```

---

### B4 — Print Hello N Times

**Task:** Define a function that prints `Hello`, then call it `n` times.

**Required function:** Define `greet()` (no parameters) that prints `Hello`, and call it `n` times.

**Input Format:** A single integer `n` (1 ≤ n ≤ 50).

**Output Format:** `Hello` printed on `n` separate lines.

**Sample Input:**
```
3
```
**Sample Output:**
```
Hello
Hello
Hello
```

---

### B5 — Sum From 1 to N

**Task:** Read an integer `n` and print the sum 1 + 2 + … + n.

**Required function:** Define `total(n)` that computes and prints the sum, and call it with the value read from input.

**Input Format:** A single integer `n` (1 ≤ n ≤ 10000).

**Output Format:** A single integer — the sum from 1 to `n`.

**Sample Input:**
```
10
```
**Sample Output:**
```
55
```

---

### B6 — Minutes and Seconds

**Task:** Read a whole number of seconds and print how many whole minutes and leftover seconds it makes, separated by a space.

**Input Format:** A single integer `t` (0 ≤ t ≤ 100000), a number of seconds.

**Output Format:** Two integers separated by a space: the whole minutes, then the leftover seconds.

**Sample Input:**
```
200
```
**Sample Output:**
```
3 20
```

---

### B7 — Count Multiples of Three

**Task:** Read an integer `n` and print how many numbers from 1 to `n` (inclusive) are multiples of 3.

**Required function:** Define `count_mult(n)` that computes and prints the count, and call it with the value read from input.

**Input Format:** A single integer `n` (1 ≤ n ≤ 10000).

**Output Format:** A single integer — the count of multiples of 3 from 1 to `n`.

**Sample Input:**
```
20
```
**Sample Output:**
```
6
```

---

### B8 — Square of Stars

**Task:** Read an integer `n` and print an `n × n` square of stars. Each row has `n` stars separated by single spaces.

**Required function:** Define `square(n)` that prints the grid, and call it with the value read from input.

**Input Format:** A single integer `n` (1 ≤ n ≤ 50).

**Output Format:** `n` lines, each containing `n` stars separated by single spaces.

**Sample Input:**
```
3
```
**Sample Output:**
```
* * *
* * *
* * *
```

---

### B9 — Factorial

**Task:** Read an integer `n` and print `n!` (the product 1 × 2 × … × n).

**Required function:** Define `fact(n)` that computes and prints the factorial, and call it with the value read from input.

**Input Format:** A single integer `n` (1 ≤ n ≤ 12).

**Output Format:** A single integer — the factorial of `n`.

**Sample Input:**
```
5
```
**Sample Output:**
```
120
```

---

### B10 — Reverse a Number

**Task:** Read an integer `n` and print it with its digits reversed. (Leading zeros in the result naturally disappear — reversing 1230 gives 321.)

**Required function:** Define `reverse(n)` that computes and prints the reversed number, and call it with the value read from input.

**Input Format:** A single integer `n` (0 ≤ n ≤ 1000000).

**Output Format:** A single integer — the digits of `n` reversed.

**Sample Input:**
```
1230
```
**Sample Output:**
```
321
```

---

*End of Test 1. Section A: 10 marks · Section B: 30 marks · Total: 40 marks.*
