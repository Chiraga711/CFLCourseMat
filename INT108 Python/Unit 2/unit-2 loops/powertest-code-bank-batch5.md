# Platform Question Pool — Batch 5: Harder Tier (30 Questions)

**Conventions.** Inputs come one value per line — whole numbers via `int(input())`, float values via `float(input())`; no prompts. Where a question asks for **two decimal places**, print with the fixed recipe `print(f"{ans:.2f}")`; all expected outputs were generated with the same recipe. Integer answers print plainly. Constraints allow simple loop solutions (nested where the problem demands it).

---

## Section A — Digit Manipulation, Round 2

## Q1. Unique Digits
**Problem.** A digit of a number is *unique* if it appears exactly once in it.
**Task.** Read an integer `n`; print how many of the digits 0–9 appear exactly once in `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the count of unique digits.
**Sample**
```
Input          Output
122338         2
```

## Q2. Repeated Digits
**Problem.** A digit is *repeated* if it appears two or more times in the number.
**Task.** Read an integer `n`; print how many of the digits 0–9 appear at least twice in `n`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the count of repeated digits.
**Sample**
```
Input          Output
122338         2
```

## Q3. Most Frequent Digit
**Problem.** One digit occurs more often than any other; on a tie, the smaller digit wins.
**Task.** Read an integer `n`; print the digit that appears most often in `n` (smallest digit on a tie).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer (0–9) — the most frequent digit.
**Sample**
```
Input          Output
373735         3
```

## Q4. Swap First and Last Digit
**Problem.** Swapping the first and last digits of a number produces a new number (a single-digit number stays itself).
**Task.** Read an integer `n`; print the number formed by swapping its first and last digits.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the swapped number.
**Sample**
```
Input          Output
12345          52341
```

## Q5. To Binary
**Problem.** Every number has a binary form made of 0s and 1s (13 in binary is 1101).
**Task.** Read an integer `n`; print its binary form (as a number of 0/1 digits).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 1023)
**Output Format.** A single integer made of binary digits.
**Sample**
```
Input          Output
13             1101
```

## Q6. From Binary
**Problem.** A number written with only 0/1 digits can be read as binary.
**Task.** Read a number `b` whose digits are all 0 or 1; print its decimal value.
**Input Format**
Line 1: integer `b`  (binary digits only, at most 10 of them)
**Output Format.** A single integer — the decimal value.
**Sample**
```
Input          Output
1101           13
```

## Q7. Lucky Ticket
**Problem.** A 6-digit ticket is *lucky* by degree: the difference between the digit sum of its first three digits and its last three.
**Task.** Read a 6-digit ticket number; print the absolute difference between the two half-sums (0 means perfectly lucky).
**Input Format**
Line 1: integer ticket  (100000 ≤ ticket ≤ 999999)
**Output Format.** A single integer — the absolute difference.
**Sample**
```
Input          Output
385274         3
```

## Q8. Remove the Zeros
**Problem.** Deleting every 0 digit from a number leaves a shorter number (30506 becomes 356).
**Task.** Read an integer `n`; print the number formed by removing all of its zero digits.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the zero-free number.
**Sample**
```
Input          Output
30506          356
```

---

## Section B — Two-Decimal Computation

## Q9. True Average
**Problem.** The average of a set of readings is their sum divided by their count.
**Task.** Read `T`, then `T` float values; print their average.
**Input Format**
Line 1: integer `T`  (1 ≤ T ≤ 1000)
Next `T` lines: one float each
**Output Format.** A single number with exactly two decimal places — the average.
**Sample**
```
Input          Output
4              9.81
12.5
7.25
10
9.5
```

## Q10. Exam Percentage
**Problem.** A student's percentage is marks obtained × 100 divided by the maximum marks.
**Task.** Read the marks obtained and the maximum marks; print the percentage.
**Input Format**
Line 1: integer marks obtained
Line 2: integer maximum marks  (1 ≤ obtained ≤ maximum ≤ 10⁴)
**Output Format.** A single number with exactly two decimal places — the percentage.
**Sample**
```
Input          Output
434            72.33
600
```

## Q11. Better Unit Price
**Problem.** Two pack sizes of the same product compete: the better buy has the lower price per gram.
**Task.** Read the weight and price of pack 1, then of pack 2; print the lower price per gram.
**Input Format**
Line 1: integer weight 1 (grams)
Line 2: integer price 1
Line 3: integer weight 2 (grams)
Line 4: integer price 2  (all 1 ≤ value ≤ 10⁵)
**Output Format.** A single number with exactly two decimal places — the lower per-gram price.
**Sample**
```
Input          Output
250            0.23
60
400
92
```

## Q12. Average Speed
**Problem.** Speed is distance divided by time.
**Task.** Read the distance in km and the time in hours (both floats); print the speed in km/h.
**Input Format**
Line 1: float distance
Line 2: float time  (time > 0)
**Output Format.** A single number with exactly two decimal places — the speed.
**Sample**
```
Input          Output
245.5          70.14
3.5
```

## Q13. Price before GST
**Problem.** A printed price already includes 18% GST, so the base price is the printed price × 100 ⁄ 118.
**Task.** Read the printed price; print the base price.
**Input Format**
Line 1: float printed price  (1 ≤ price ≤ 10⁶)
**Output Format.** A single number with exactly two decimal places — the base price.
**Sample**
```
Input          Output
2596           2200.00
```

## Q14. Trip Average Speed
**Problem.** A trip has several legs; the average speed is the total distance divided by the total time.
**Task.** Read the number of legs `T`, then for each leg its distance (km) and time (hours); print the trip's average speed.
**Input Format**
Line 1: integer `T`  (1 ≤ T ≤ 100)
Then for each leg, two lines: float distance, float time
**Output Format.** A single number with exactly two decimal places — the average speed.
**Sample**
```
Input          Output
2              37.50
60
1.5
90
2.5
```

## Q15. Density
**Problem.** Density is mass divided by volume.
**Task.** Read the mass in grams and the volume in cm³ (floats); print the density in g/cm³.
**Input Format**
Line 1: float mass
Line 2: float volume  (volume > 0)
**Output Format.** A single number with exactly two decimal places — the density.
**Sample**
```
Input          Output
350            8.75
40
```

---

## Section C — Nested-Loop Counting

## Q16. Factor Pairs
**Problem.** A number can be written as i × j in several ways with i ≤ j (36 = 1×36 = 2×18 = 3×12 = 4×9 = 6×6).
**Task.** Read an integer `n`; count the pairs (i, j) with i ≤ j and i × j = n, and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the pair count.
**Sample**
```
Input          Output
36             5
```

## Q17. Triangle Triples
**Problem.** Three sides a ≤ b ≤ c form a triangle exactly when a + b > c.
**Task.** Read an integer `n`; count the triples (a, b, c) with 1 ≤ a ≤ b ≤ c ≤ n that form a triangle, and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 50)
**Output Format.** A single integer — the triple count.
**Sample**
```
Input          Output
10             125
```

## Q18. Anti-Diagonal Sum
**Problem.** In an n × n multiplication grid (cell (i, j) holds i × j), the anti-diagonal is the cells where i + j = n + 1.
**Task.** Read an integer `n`; print the sum of the anti-diagonal cells.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
4              20
```

## Q19. Coprime Pairs
**Problem.** Two numbers are coprime when their greatest common divisor is 1.
**Task.** Read an integer `n`; count the pairs (i, j) with 1 ≤ i < j ≤ n that are coprime, and print the count.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 100)
**Output Format.** A single integer — the coprime pair count.
**Sample**
```
Input          Output
5              9
```

## Q20. Ways to Pay
**Problem.** An amount can be paid with ₹1, ₹2, and ₹5 coins in many combinations (what matters is how many of each coin, not their order).
**Task.** Read an amount `A`; count the different combinations of coins that pay exactly `A`, and print the count.
**Input Format**
Line 1: integer `A`  (1 ≤ A ≤ 2000)
**Output Format.** A single integer — the number of ways.
**Sample**
```
Input          Output
10             10
```

## Q21. Pythagorean Triples
**Problem.** A Pythagorean triple has a < b < c with a² + b² = c² (like 3, 4, 5).
**Task.** Read an integer `n`; count the Pythagorean triples with c ≤ n, and print the count.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 100)
**Output Format.** A single integer — the triple count.
**Sample**
```
Input          Output
20             6
```

## Q22. Square-Sum Pairs
**Problem.** Some pairs of numbers add up to a perfect square (1 + 3 = 4, 2 + 7 = 9).
**Task.** Read an integer `n`; count the pairs (i, j) with 1 ≤ i < j ≤ n whose sum is a perfect square, and print the count.
**Input Format**
Line 1: integer `n`  (2 ≤ n ≤ 300)
**Output Format.** A single integer — the pair count.
**Sample**
```
Input          Output
10             7
```

---

## Section D — Capstones

## Q23. Positional Checksum
**Problem.** A checksum weights each digit by its position counted from the right (rightmost digit × 1, next × 2, and so on) and adds them up.
**Task.** Read an integer `n`; print the checksum.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the checksum.
**Sample**
```
Input          Output
4728           49
```

## Q24. Alternating Digit Sum
**Problem.** Starting from the rightmost digit with a plus, digits are added and subtracted alternately (this is the divisibility-by-11 test).
**Task.** Read an integer `n`; print the alternating sum (it may be negative).
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁹)
**Output Format.** A single integer — the alternating sum.
**Sample**
```
Input          Output
725384         -11
```

## Q25. Grain Silo with a Leak
**Problem.** A silo of capacity `C` kg starts empty. Each minute the conveyor adds `a` kg. If the total has reached `C`, the silo is full and everything stops; otherwise, if the total is above `t`, a leak drains `b` kg before the next minute.
**Task.** Read `C`, `a`, `b`, `t` (a > b); print in which minute the silo becomes full.
**Input Format**
Line 1: integer `C`  (1 ≤ C ≤ 10⁵)
Line 2: integer `a`
Line 3: integer `b`  (0 ≤ b < a ≤ 1000)
Line 4: integer `t`  (1 ≤ t < C)
**Output Format.** A single integer — the minute.
**Sample**
```
Input          Output
100            13
10
4
50
```

## Q26. Catch the Runner
**Problem.** Runner A runs at `a` metres per minute and starts `h` minutes early. Runner B then starts on the same track at `b` metres per minute (b > a).
**Task.** Read `a`, `h`, `b`; print how many minutes after B starts B first catches up with A (is at or past A's position).
**Input Format**
Line 1: integer `a`
Line 2: integer `h`  (1 ≤ h ≤ 100)
Line 3: integer `b`  (1 ≤ a < b ≤ 1000)
**Output Format.** A single integer — the minutes.
**Sample**
```
Input          Output
200            12
6
300
```

## Q27. Compound Interest
**Problem.** A deposit grows by `r` percent every year, on the running balance (compound growth).
**Task.** Read the principal `P`, the yearly rate `r` (a float, like 7.5), and the years `y`; print the final amount.
**Input Format**
Line 1: float `P`  (1 ≤ P ≤ 10⁷)
Line 2: float `r`  (0.1 ≤ r ≤ 50)
Line 3: integer `y`  (1 ≤ y ≤ 50)
**Output Format.** A single number with exactly two decimal places — the final amount.
**Sample**
```
Input          Output
10000          12422.97
7.5
3
```

## Q28. Clock Angle
**Problem.** At H hours and M minutes, the hour hand sits at 30·H + M/2 degrees and the minute hand at 6·M degrees; the angle between them is the smaller of the two ways around (at most 180°).
**Task.** Read `H` and `M`; print the angle between the hands.
**Input Format**
Line 1: integer `H`  (1 ≤ H ≤ 12)
Line 2: integer `M`  (0 ≤ M ≤ 59)
**Output Format.** A single number with exactly two decimal places — the angle in degrees.
**Sample**
```
Input          Output
3              75.00
30
```

## Q29. Leap Years in a Range
**Problem.** A year is a leap year if it is divisible by 4 — except century years (divisible by 100), which are leap years only when divisible by 400.
**Task.** Read years `a` and `b`; count the leap years from `a` to `b` and print the count.
**Input Format**
Line 1: integer `a`
Line 2: integer `b`  (1 ≤ a ≤ b ≤ 10⁴)
**Output Format.** A single integer — the leap-year count.
**Sample**
```
Input          Output
1990           9
2025
```

## Q30. The 6174 Routine
**Problem.** Kaprekar's routine: take a 4-digit number (not all digits the same), arrange its digits in descending and ascending order, subtract the smaller from the larger, and repeat with the result (treated as 4 digits, keeping leading zeros). Every such number reaches 6174.
**Task.** Read a 4-digit number; print how many subtraction steps it takes to reach 6174 (the number 6174 itself needs 0 steps).
**Input Format**
Line 1: integer `n`  (1000 ≤ n ≤ 9999, digits not all identical)
**Output Format.** A single integer — the step count.
**Sample**
```
Input          Output
3524           3
```

---

*End of Batch 5 — 30 questions, every sample output generated by a verified reference solution.*
