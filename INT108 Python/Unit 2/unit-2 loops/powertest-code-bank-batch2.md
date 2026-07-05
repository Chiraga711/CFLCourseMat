# Platform Question Pool — Batch 2: Series & Math Computation (38 Questions)

**Conventions.** All inputs are integers, one per line, read with `int(input())` — no prompts. Print exactly what the output format asks. Every answer is a computed number; all constraints allow simple loop solutions. Ranges include both ends.

---

## Section A — Factorials & Powers

## Q1. Factorial
**Problem.** The factorial of `n` is the product 1 × 2 × … × n.
**Task.** Read an integer `n` and print `n!`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 15)
**Output Format.** A single integer — the factorial.
**Sample**
```
Input          Output
6              720
```

## Q2. Sum of Factorials
**Problem.** Each number from 1 to `n` has a factorial.
**Task.** Read an integer `n` and print the sum 1! + 2! + … + n!.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 12)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              153
```

## Q3. Power Without `**`
**Problem.** A power is repeated multiplication.
**Task.** Read integers `a` and `b`; print `a` raised to the power `b`, computed with a loop (b = 0 gives 1).
**Input Format**
Line 1: integer `a`  (1 ≤ a ≤ 20)
Line 2: integer `b`  (0 ≤ b ≤ 12)
**Output Format.** A single integer — the power.
**Sample**
```
Input          Output
2              1024
10
```

## Q4. Sum of Powers
**Problem.** The powers of `x` grow quickly.
**Task.** Read integers `x` and `n`; print the sum x¹ + x² + … + xⁿ.
**Input Format**
Line 1: integer `x`  (1 ≤ x ≤ 5)
Line 2: integer `n`  (1 ≤ n ≤ 15)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
3              120
4
```

## Q5. Trailing Zeros of a Factorial
**Problem.** Factorials end in a run of zeros: 10! = 3628800 ends in two.
**Task.** Read an integer `n`; compute `n!` and print how many zeros it ends with.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 500)
**Output Format.** A single integer — the count of trailing zeros.
**Sample**
```
Input          Output
10             2
```

## Q6. Last Digit of a Power
**Problem.** Even a huge power has just one last digit.
**Task.** Read integers `a` and `b`; print the last digit of `a` raised to the power `b`.
**Input Format**
Line 1: integer `a`  (2 ≤ a ≤ 9)
Line 2: integer `b`  (1 ≤ b ≤ 1000)
**Output Format.** A single integer (0–9) — the last digit.
**Sample**
```
Input          Output
7              3
3
```

## Q7. Double Factorial
**Problem.** The double factorial `n!!` multiplies every second number going down: 7!! = 7 × 5 × 3 × 1.
**Task.** Read an integer `n` and print `n!!`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 20)
**Output Format.** A single integer — the double factorial.
**Sample**
```
Input          Output
7              105
```

## Q8. Product of a Range
**Problem.** Consecutive integers can be multiplied together.
**Task.** Read integers `a` and `b`; print the product a × (a+1) × … × b.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 20)
**Output Format.** A single integer — the product.
**Sample**
```
Input          Output
3              360
6
```

---

## Section B — Series Sums

## Q9. Sum to n
**Problem.** The natural numbers can be added one by one.
**Task.** Read an integer `n`; print 1 + 2 + … + n.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁶)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
100            5050
```

## Q10. Sum of Squares
**Problem.** Each number contributes its square.
**Task.** Read an integer `n`; print 1² + 2² + … + n².
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
10             385
```

## Q11. Sum of Cubes
**Problem.** Each number contributes its cube.
**Task.** Read an integer `n`; print 1³ + 2³ + … + n³.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              225
```

## Q12. Sum of the First k Odd Numbers
**Problem.** The odd numbers are 1, 3, 5, 7, …
**Task.** Read an integer `k`; print the sum of the first `k` odd numbers.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁶)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              25
```

## Q13. Sum of the First k Even Numbers
**Problem.** The even numbers are 2, 4, 6, 8, …
**Task.** Read an integer `k`; print the sum of the first `k` even numbers.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁶)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              30
```

## Q14. Alternating Sum
**Problem.** In an alternating series, the sign flips each term: 1 − 2 + 3 − 4 + …
**Task.** Read an integer `k`; print the value of the series after `k` terms.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁶)
**Output Format.** A single integer — the value (it may be negative).
**Sample**
```
Input          Output
5              3
```

## Q15. Alternating Even Sum
**Problem.** The even numbers with flipping signs: 2 − 4 + 6 − 8 + …
**Task.** Read an integer `k`; print the value of the series after `k` terms.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁶)
**Output Format.** A single integer — the value (it may be negative).
**Sample**
```
Input          Output
4              -4
```

## Q16. Staircase Sum
**Problem.** The staircase series adds growing blocks: (1) + (1+2) + (1+2+3) + …
**Task.** Read an integer `n`; print the total of the first `n` blocks.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the total.
**Sample**
```
Input          Output
4              20
```

## Q17. Sum of Odd Squares
**Problem.** The odd numbers 1, 3, 5, … each have a square.
**Task.** Read an integer `k`; print the sum of the squares of the first `k` odd numbers.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
3              35
```

## Q18. Sum of Powers of Two
**Problem.** The powers of two are 1, 2, 4, 8, …
**Task.** Read an integer `k`; print the sum of the first `k` powers of two (starting from 1).
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 50)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              31
```

## Q19. Pronic Series Sum
**Problem.** Each term is a product of neighbours: 1·2 + 2·3 + 3·4 + …
**Task.** Read an integer `n`; print the sum of the first `n` terms.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
4              40
```

## Q20. Sum of Multiples
**Problem.** The multiples of `k` are k, 2k, 3k, …
**Task.** Read integers `k` and `n`; print the sum of all multiples of `k` that are ≤ `n`.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 100)
Line 2: integer `n`  (1 ≤ n ≤ 10⁶)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
3              63
20
```

---

## Section C — Divisibility, GCD & Divisors

## Q21. Divisible Sum in a Range
**Problem.** Some numbers in a range divide evenly by `d`.
**Task.** Read integers `a`, `b`, `d`; print the sum of the numbers from `a` to `b` that are divisible by `d`.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
Line 3: integer `d`  (1 ≤ d ≤ 100)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
10             100
30
4
```

## Q22. Divisible by One, Not the Other
**Problem.** A number can be divisible by `x` yet not by `y`.
**Task.** Read integers `a`, `b`, `x`, `y`; count the numbers from `a` to `b` divisible by `x` but **not** by `y`, and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
Line 3: integer `x`
Line 4: integer `y`  (2 ≤ x, y ≤ 100)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              5
30
3
2
```

## Q23. Divisible by Both
**Problem.** A number can be divisible by two values at once.
**Task.** Read integers `a`, `b`, `x`, `y`; count the numbers from `a` to `b` divisible by **both** `x` and `y`, and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
Line 3: integer `x`
Line 4: integer `y`  (2 ≤ x, y ≤ 100)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              8
100
4
6
```

## Q24. Neither Three nor Five
**Problem.** Some numbers avoid being divisible by 3 and by 5.
**Task.** Read an integer `n`; print the sum of the numbers from 1 to `n` divisible by **neither** 3 nor 5.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
10             22
```

## Q25. First Common Multiple at or after a
**Problem.** Somewhere at or beyond `a` lies a number divisible by both `x` and `y`.
**Task.** Read integers `a`, `x`, `y`; print the smallest number ≥ `a` divisible by both `x` and `y`.
**Input Format**
Line 1: integer `a`  (1 ≤ a ≤ 10⁵)
Line 2: integer `x`
Line 3: integer `y`  (2 ≤ x, y ≤ 50)
**Output Format.** A single integer — the smallest such number.
**Sample**
```
Input          Output
50             72
6
8
```

## Q26. Last Multiple up to b
**Problem.** Below any limit there is a largest multiple of `x`.
**Task.** Read integers `b` and `x`; print the largest number ≤ `b` divisible by `x`.
**Input Format**
Line 1: integer `b`
Line 2: integer `x`  (2 ≤ x ≤ 100, x ≤ b ≤ 10⁶)
**Output Format.** A single integer — the largest such number.
**Sample**
```
Input          Output
100            98
7
```

## Q27. Greatest Common Divisor
**Problem.** The GCD of two numbers is the largest number dividing both.
**Task.** Read integers `a` and `b`; print their GCD.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a, b ≤ 10⁹)
**Output Format.** A single integer — the GCD.
**Sample**
```
Input          Output
48             12
36
```

## Q28. Least Common Multiple
**Problem.** The LCM of two numbers is the smallest number divisible by both.
**Task.** Read integers `a` and `b`; print their LCM.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a, b ≤ 10⁴)
**Output Format.** A single integer — the LCM.
**Sample**
```
Input          Output
12             36
18
```

## Q29. GCD of Three Numbers
**Problem.** Three numbers also share a greatest common divisor.
**Task.** Read integers `a`, `b`, `c`; print the GCD of all three.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`
Line 3: integer `c`  (1 ≤ a, b, c ≤ 10⁹)
**Output Format.** A single integer — the GCD.
**Sample**
```
Input          Output
24             12
36
60
```

## Q30. Common Divisor Count
**Problem.** Two numbers can share several divisors.
**Task.** Read integers `a` and `b`; count the numbers that divide both, and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a, b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
12             4
18
```

## Q31. Common Divisor Sum
**Problem.** The shared divisors of two numbers can be added.
**Task.** Read integers `a` and `b`; print the sum of the numbers that divide both.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a, b ≤ 10⁵)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
12             12
18
```

## Q32. Divisor Count
**Problem.** Every number has a certain number of divisors.
**Task.** Read an integer `n`; print how many divisors it has (including 1 and `n`).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the divisor count.
**Sample**
```
Input          Output
36             9
```

## Q33. Smallest Prime Factor
**Problem.** Every number ≥ 2 has a smallest factor greater than 1, and it is always prime.
**Task.** Read an integer `n`; print its smallest factor greater than 1.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the smallest prime factor.
**Sample**
```
Input          Output
91             7
```

## Q34. Largest Prime Factor
**Problem.** Breaking a number into prime factors reveals a largest one (84 = 2 × 2 × 3 × 7).
**Task.** Read an integer `n`; print its largest prime factor.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the largest prime factor.
**Sample**
```
Input          Output
84             7
```

## Q35. Prime Factor Count
**Problem.** Counting prime factors includes repeats: 60 = 2 × 2 × 3 × 5 has four.
**Task.** Read an integer `n`; print how many prime factors it has, counted with repetition.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
60             4
```

---

## Section D — Nested Computation

## Q36. Multiplication Grid Total
**Problem.** An n × n multiplication grid holds i × j in each cell.
**Task.** Read an integer `n`; print the sum of all the cells of the grid.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 200)
**Output Format.** A single integer — the grid total.
**Sample**
```
Input          Output
3              36
```

## Q37. Table Total
**Problem.** A multiplication table lists k × 1 up to k × m.
**Task.** Read integers `k` and `m`; print the sum of the table's entries.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 100)
Line 2: integer `m`  (1 ≤ m ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
7              385
10
```

## Q38. Pair Count
**Problem.** Pairs (i, j) with i < j can be tested one by one.
**Task.** Read integers `n` and `k`; count the pairs with 1 ≤ i < j ≤ n whose sum i + j is divisible by `k`, and print the count.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 300)
Line 2: integer `k`  (2 ≤ k ≤ 50)
**Output Format.** A single integer — the pair count.
**Sample**
```
Input          Output
6              5
3
```

---

*End of Batch 2 — 38 questions, every sample output generated by a verified reference solution.*
