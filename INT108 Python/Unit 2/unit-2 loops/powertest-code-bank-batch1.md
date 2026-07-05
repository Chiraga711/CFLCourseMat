# Platform Question Pool — Batch 1: Special Numbers (47 Questions)

**Conventions (apply to every question).** All inputs are integers, one per line, read with `int(input())` — no prompts. Print exactly what the output format asks, nothing more. Every answer is a computed number, and all constraints allow simple loop solutions. Ranges are always inclusive of both ends.

---

## Section A — Digit Fundamentals

## Q1. Digit Sum
**Problem.** Every number is made of digits.
**Task.** Read an integer `n` and print the sum of its digits.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the digit sum.
**Sample**
```
Input          Output
4728           21
```

## Q2. Reverse the Number
**Problem.** Reversing a number writes its digits in the opposite order.
**Task.** Read an integer `n` and print its reverse. (Trailing zeros vanish: 4708 → 8074.)
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the reversed number.
**Sample**
```
Input          Output
4708           8074
```

## Q3. Product of Non-Zero Digits
**Problem.** Zeros would wipe out a product, so they are skipped.
**Task.** Read an integer `n` and print the product of its non-zero digits.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the product.
**Sample**
```
Input          Output
2053           30
```

## Q4. Even Digit Count
**Problem.** A digit is even if it is 0, 2, 4, 6, or 8.
**Task.** Read an integer `n` and print how many of its digits are even.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
482716         4
```

## Q5. Count a Digit
**Problem.** A digit may appear in a number several times.
**Task.** Read an integer `n` and a digit `d` (0–9); print how many times `d` appears in `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
Line 2: integer `d`  (0 ≤ d ≤ 9)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
282828         3
8
```

## Q6. Digit Spread
**Problem.** The spread of a number is the difference between its largest and smallest digit.
**Task.** Read an integer `n` and print (largest digit − smallest digit).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the spread.
**Sample**
```
Input          Output
3941           8
```

## Q7. Digit Sum of the Square
**Problem.** Squaring a number produces new digits (this is the building block of neon numbers).
**Task.** Read an integer `n`, square it, and print the digit sum of the square.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the digit sum of `n × n`.
**Sample**
```
Input          Output
13             16
```

## Q8. Sum of Proper Divisors
**Problem.** The proper divisors of `n` are its divisors excluding `n` itself (this is the building block of perfect numbers).
**Task.** Read an integer `n` and print the sum of its proper divisors.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
36             55
```

## Q9. Digit Factorial Sum
**Problem.** Each digit has a factorial: 5! = 120, 0! = 1 (this is the building block of strong numbers).
**Task.** Read an integer `n` and print the sum of the factorials of its digits.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁷)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
145            145
```

## Q10. Digital Root
**Problem.** Repeatedly replace a number with its digit sum until a single digit remains — that digit is the digital root.
**Task.** Read an integer `n` and print its digital root.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer (0–9) — the digital root.
**Sample**
```
Input          Output
9875           2
```

---

## Section B — Counting and Summing over Ranges

## Q11. Palindrome Count in a Range
**Problem.** A number is a palindrome if it reads the same forwards and backwards (every single-digit number is a palindrome).
**Task.** Read integers `a` and `b`; count the palindromes from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             9
100
```

## Q12. Palindrome Sum in a Range
**Problem.** A number is a palindrome if it equals its own reverse.
**Task.** Read integers `a` and `b`; print the sum of all palindromes from `a` to `b`.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
10             66
40
```

## Q13. Prime Count in a Range
**Problem.** A prime number has exactly two divisors: 1 and itself.
**Task.** Read integers `a` and `b`; count the primes from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 1000)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             11
50
```

## Q14. Prime Sum in a Range
**Problem.** A prime number has exactly two divisors.
**Task.** Read integers `a` and `b`; print the sum of all primes from `a` to `b`.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 1000)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
1              77
20
```

## Q15. Armstrong Count in a Range
**Problem.** An Armstrong number equals the sum of its digits each raised to the power of the digit count (153 = 1³ + 5³ + 3³; every single-digit number qualifies).
**Task.** Read integers `a` and `b`; count the Armstrong numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              13
500
```

## Q16. Happy Count in a Range
**Problem.** A number is happy if repeatedly replacing it with the sum of the squares of its digits eventually reaches 1 (unhappy numbers instead fall into a cycle that passes through 4).
**Task.** Read integers `a` and `b`; count the happy numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁴)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              11
50
```

## Q17. Harshad Count in a Range
**Problem.** A Harshad number is divisible by its own digit sum (18 → 1 + 8 = 9, and 18 % 9 = 0).
**Task.** Read integers `a` and `b`; count the Harshad numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             8
30
```

## Q18. Spy Count in a Range
**Problem.** A spy number's digit sum equals its digit product (1124 → sum 8, product 8).
**Task.** Read integers `a` and `b`; count the spy numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (10 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             3
150
```

## Q19. Automorphic Count up to n
**Problem.** An automorphic number's square ends with the number itself (76² = 5776).
**Task.** Read an integer `n`; count the automorphic numbers from 1 to `n` and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
100            5
```

## Q20. Kaprekar Count up to n
**Problem.** For a Kaprekar number with `d` digits, splitting its square into a right part of `d` digits and a left part gives two pieces that add back to the number (45² = 2025 → 20 + 25 = 45). The right part must be greater than 0.
**Task.** Read an integer `n`; count the Kaprekar numbers from 1 to `n` and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
100            5
```

## Q21. Perfect Count up to n
**Problem.** A perfect number equals the sum of its proper divisors (6 = 1 + 2 + 3).
**Task.** Read an integer `n`; count the perfect numbers from 1 to `n` and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 5000)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1000           3
```

## Q22. Abundant Count in a Range
**Problem.** A number is abundant if the sum of its proper divisors is greater than the number (12 → 1+2+3+4+6 = 16 > 12).
**Task.** Read integers `a` and `b`; count the abundant numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 2000)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              9
50
```

## Q23. Pronic Count up to n
**Problem.** A pronic number is the product of two consecutive integers, x × (x + 1): 2, 6, 12, 20, …
**Task.** Read an integer `n`; count the pronic numbers that are ≤ `n` and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
50             6
```

## Q24. Sunny Count in a Range
**Problem.** A number `k` is sunny if `k + 1` is a perfect square (3 is sunny because 4 = 2²).
**Task.** Read integers `a` and `b`; count the sunny numbers from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁴)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
1              4
30
```

## Q25. Perfect Squares in a Range
**Problem.** A perfect square is i × i for some whole number i.
**Task.** Read integers `a` and `b`; count the perfect squares from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁹)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             7
100
```

## Q26. Fibonacci Terms up to n
**Problem.** The Fibonacci series starts 0, 1, and every later term is the sum of the two before it: 0, 1, 1, 2, 3, 5, 8, …
**Task.** Read an integer `n`; print how many terms of the series are ≤ `n` (the two 1s count as separate terms).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the number of terms.
**Sample**
```
Input          Output
100            12
```

## Q27. Odd Digit-Sum Count
**Problem.** Every number has a digit sum, which is either odd or even.
**Task.** Read integers `a` and `b`; count the numbers from `a` to `b` whose digit sum is odd, and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁵)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             5
20
```

## Q28. Strong Sum up to n
**Problem.** A strong number equals the sum of the factorials of its digits (145 = 1! + 4! + 5!).
**Task.** Read an integer `n`; print the sum of all strong numbers from 1 to `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
1000           148
```

## Q29. Palindrome-Prime Count
**Problem.** Some numbers are both palindromes and primes (11, 101, 131, …).
**Task.** Read integers `a` and `b`; count the numbers from `a` to `b` that are both palindrome and prime, and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 1000)
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             6
200
```

---

## Section C — Find the Next, the k-th, the Closest

## Q30. Next Palindrome
**Problem.** A palindrome equals its own reverse.
**Task.** Read an integer `n`; print the smallest palindrome strictly greater than `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the next palindrome.
**Sample**
```
Input          Output
123            131
```

## Q31. The k-th Prime
**Problem.** The primes in order are 2, 3, 5, 7, 11, …
**Task.** Read an integer `k`; print the k-th prime number.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 100)
**Output Format.** A single integer — the k-th prime.
**Sample**
```
Input          Output
10             29
```

## Q32. Largest Prime up to n
**Problem.** A prime has exactly two divisors.
**Task.** Read an integer `n`; print the largest prime that is ≤ `n`.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the largest prime ≤ `n`.
**Sample**
```
Input          Output
100            97
```

## Q33. Next Armstrong Number
**Problem.** An Armstrong number equals the sum of its digits raised to the power of the digit count.
**Task.** Read an integer `n`; print the smallest Armstrong number strictly greater than `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the next Armstrong number.
**Sample**
```
Input          Output
100            153
```

## Q34. The k-th Happy Number
**Problem.** A number is happy if repeated sum-of-squared-digits reaches 1. The happy numbers in order are 1, 7, 10, 13, 19, …
**Task.** Read an integer `k`; print the k-th happy number.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 200)
**Output Format.** A single integer — the k-th happy number.
**Sample**
```
Input          Output
5              19
```

## Q35. Next Harshad Number
**Problem.** A Harshad number is divisible by its digit sum.
**Task.** Read an integer `n`; print the smallest Harshad number strictly greater than `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the next Harshad number.
**Sample**
```
Input          Output
25             27
```

## Q36. Next Trimorphic Number
**Problem.** A trimorphic number's cube ends with the number itself (4³ = 64; 24³ = 13824).
**Task.** Read an integer `n`; print the smallest trimorphic number strictly greater than `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the next trimorphic number.
**Sample**
```
Input          Output
10             24
```

## Q37. The k-th Fibonacci Term
**Problem.** The Fibonacci series starts 0, 1, and each later term is the sum of the two before it (term 1 is 0, term 2 is 1).
**Task.** Read an integer `k`; print the k-th term of the series.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 45)
**Output Format.** A single integer — the k-th term.
**Sample**
```
Input          Output
8              13
```

## Q38. Closest Prime
**Problem.** Every number has a prime nearest to it.
**Task.** Read an integer `n`; print the prime closest to `n`. If `n` itself is prime, print `n`. If two primes are equally close, print the smaller one.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the closest prime.
**Sample**
```
Input          Output
20             19
```

## Q39. Palindrome-Harshad Search
**Problem.** Some numbers are both palindromes and Harshad numbers (divisible by their digit sum).
**Task.** Read an integer `n`; print the smallest number strictly greater than `n` that is both a palindrome and a Harshad number.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the smallest such number.
**Sample**
```
Input          Output
100            111
```

---

## Section D — Sequence Processes

## Q40. Happy Steps
**Problem.** A happy number reaches 1 by repeatedly being replaced with the sum of the squares of its digits (19 → 82 → 68 → 100 → 1).
**Task.** Read a happy number `n`; print how many replacement steps it takes to reach 1. (The input is guaranteed to be a happy number.)
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴, guaranteed happy)
**Output Format.** A single integer — the number of steps.
**Sample**
```
Input          Output
19             4
```

## Q41. Additive Persistence
**Problem.** Replacing a number with its digit sum, again and again, eventually leaves a single digit.
**Task.** Read an integer `n`; print how many digit-sum steps it takes to reach a single digit. (A single-digit input needs 0 steps.)
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the number of steps.
**Sample**
```
Input          Output
9875           3
```

## Q42. Multiplicative Persistence
**Problem.** Replacing a number with its digit **product**, again and again, eventually leaves a single digit (39 → 27 → 14 → 4).
**Task.** Read an integer `n`; print how many digit-product steps it takes to reach a single digit.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the number of steps.
**Sample**
```
Input          Output
39             3
```

## Q43. Collatz Steps
**Problem.** The Collatz rule: if the number is even, halve it; if odd, replace it with 3 × number + 1. Repeating this always reaches 1.
**Task.** Read an integer `n`; print how many steps the Collatz process takes to reach 1.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the number of steps.
**Sample**
```
Input          Output
6              8
```

## Q44. Collatz Peak
**Problem.** On its way to 1, a Collatz sequence can climb above where it started (6 → 3 → 10 → 5 → 16 → 8 → 4 → 2 → 1).
**Task.** Read an integer `n`; print the largest value that appears in the Collatz sequence starting at `n` (including `n` itself).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the peak value.
**Sample**
```
Input          Output
6              16
```

## Q45. Collatz Even Count
**Problem.** A Collatz sequence mixes even and odd values on its way to 1.
**Task.** Read an integer `n`; print how many even numbers appear in the Collatz sequence from `n` to 1 (counting `n` itself if it is even).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the count of even values.
**Sample**
```
Input          Output
6              6
```

---

## Section E — Streams of Numbers

## Q46. Primes in a Batch
**Problem.** A prime has exactly two divisors.
**Task.** Read an integer `T`, then `T` numbers (one per line); print how many of the `T` numbers are prime.
**Input Format**
Line 1: integer `T`  (1 ≤ T ≤ 50)
Next `T` lines: one integer each  (1 ≤ value ≤ 10⁴)
**Output Format.** A single integer — the count of primes.
**Sample**
```
Input          Output
5              2
4
7
10
13
15
```

## Q47. Palindromes until Zero
**Problem.** Numbers arrive one at a time until a 0 signals the end.
**Task.** Keep reading integers until you read 0; print how many of the entered numbers (not counting the 0) were palindromes.
**Input Format**
One integer per line, ending with 0  (each value ≤ 10⁵)
**Output Format.** A single integer — the count of palindromes.
**Sample**
```
Input          Output
121            3
45
33
7
10
0
```

---

*End of Batch 1 — 47 questions, every sample output generated by a verified reference solution.*
