# Test: Classic Number Problems

*Loops in Python series · Test for Lesson 6*

**Instructions**
- Part A has 5 multiple-choice questions. Choose the single best answer.
- Part B has 5 coding problems. Write and run your code.
- These problems use `%` and `//` with `for` and `while` loops.
- Recall the two patterns: peel digits with `n % 10` and `n // 10`, and test divisors with `n % i == 0`.
- Read whole-number input with `int(input(...))`.
- The answer key is in a separate file: `answer-keys/answers-06-classic-number-problems.md`.

**Total: 10 questions**

---

## Part A — Multiple Choice (5)

**Q1.** What is `246 // 10`?
- A) `6`
- B) `24`
- C) `246`
- D) `2`

**Q2.** The condition `n % 3 == 0` is true exactly when:
- A) `n` is divisible by 3
- B) `n` ends in the digit 3
- C) `n` is odd
- D) `n` is greater than 3

**Q3.** How many divisors does a **prime** number have?
- A) `1`
- B) `0`
- C) Depends on the number
- D) `2`

**Q4.** What does this print?
```python
total = 0
n = 123
while n > 0:
    total = total + n % 10
    n = n // 10
print(total)
```
- A) `6`
- B) `123`
- C) `321`
- D) `3`

**Q5.** This loop reverses a number with `rev = rev * 10 + n % 10`. Starting from `n = 123`, what is `rev` at the end?
- A) `123`
- B) `6`
- C) `321`
- D) `32`

---

## Part B — Coding Problems (5)

**P1 — Count Primes.**
Ask the user for a number `N`, then print how many prime numbers there are between 1 and `N`.

**P2 — Greatest Common Divisor.**
Ask the user for two whole numbers and print their greatest common divisor (the largest number that divides both of them evenly).

**P3 — Power Without `**`.**
Ask the user for two whole numbers, a base and an exponent, and print the base raised to that exponent — using a loop with multiplication, **not** the `**` operator. (For example, base 2 and exponent 5 gives 32.)

**P4 — Digital Root.**
Ask the user for a whole number, then repeatedly add up its digits until only a single digit remains, and print that digit. (For example, 1234 → 1+2+3+4 = 10 → 1+0 = 1.)

**P5 — Perfect Numbers in a Range.**
Ask the user for a number `N`, then print every perfect number between 1 and `N` (a perfect number equals the sum of its divisors below itself — 6 and 28 are the first two).

---

*End of test. Check your work against the separate answer key.*
