# Platform Question Pool — Batch 3: Streams & Statistics (34 Questions)

**Conventions.** All inputs are integers, one per line, read with `int(input())` — no prompts. Print exactly what the output format asks. Every answer is a computed number, and every question is solvable in a **single pass** over the values (no storing needed). Unless stated otherwise, values satisfy 1 ≤ value ≤ 10⁹ and 1 ≤ T ≤ 1000.

---

## Section A — One-Pass Statistics

## Q1. Stream Sum
**Problem.** Values arrive one at a time.
**Task.** Read an integer `T`, then `T` values; print their sum.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              25
4
9
2
7
3
```

## Q2. Largest Value
**Problem.** One of the readings is the biggest.
**Task.** Read `T`, then `T` values; print the largest.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the maximum.
**Sample**
```
Input          Output
5              9
4
9
2
7
3
```

## Q3. Smallest Value
**Problem.** One of the readings is the smallest.
**Task.** Read `T`, then `T` values; print the smallest.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the minimum.
**Sample**
```
Input          Output
5              3
8
3
11
5
6
```

## Q4. Value Range
**Problem.** The range of a set of readings is largest minus smallest.
**Task.** Read `T`, then `T` values; print (maximum − minimum).
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the range.
**Sample**
```
Input          Output
5              16
12
4
9
20
7
```

## Q5. Floor Average
**Problem.** The floor average of some values is their sum divided by their count, keeping only the whole part (integer division).
**Task.** Read `T`, then `T` values; print the floor average.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — sum // T.
**Sample**
```
Input          Output
4              8
10
7
9
6
```

## Q6. Count Above a Threshold
**Problem.** Some readings rise above a given level.
**Task.** Read a threshold `x`, then `T`, then `T` values; print how many values are strictly greater than `x`.
**Input Format**
Line 1: integer `x`
Line 2: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
50             3
5
30
60
55
20
80
```

## Q7. Even Count
**Problem.** Some readings are even.
**Task.** Read `T`, then `T` values; print how many are even.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
6              3
3
8
12
7
6
9
```

## Q8. Position of the First Maximum
**Problem.** The biggest value first appears at some position (positions start at 1).
**Task.** Read `T`, then `T` values; print the position where the maximum **first** appears.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the 1-based position.
**Sample**
```
Input          Output
6              2
4
9
2
9
5
1
```

## Q9. Position of the Last Minimum
**Problem.** The smallest value may appear more than once.
**Task.** Read `T`, then `T` values; print the position where the minimum **last** appears (positions start at 1).
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the 1-based position.
**Sample**
```
Input          Output
6              4
4
1
6
1
5
8
```

## Q10. Second Largest
**Problem.** Behind the largest value stands a second-largest **distinct** value.
**Task.** Read `T`, then `T` values; print the second-largest distinct value. (At least two distinct values are guaranteed; duplicates of the maximum do not count.)
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the second-largest distinct value.
**Sample**
```
Input          Output
5              30
12
45
7
45
30
```

## Q11. Count of the Maximum
**Problem.** The biggest value can appear several times.
**Task.** Read `T`, then `T` values; print how many times the maximum appears.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
6              3
5
9
3
9
2
9
```

## Q12. Even Sum Minus Odd Sum
**Problem.** The readings split into evens and odds.
**Task.** Read `T`, then `T` values; print (sum of the even values − sum of the odd values). The result may be negative.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the difference.
**Sample**
```
Input          Output
5              12
4
7
10
3
8
```

## Q13. Multiples in the Stream
**Problem.** Some readings are multiples of `k`.
**Task.** Read `k`, then `T`, then `T` values; print how many values are divisible by `k`.
**Input Format**
Line 1: integer `k`  (2 ≤ k ≤ 100)
Line 2: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
4              3
6
8
5
12
9
16
7
```

## Q14. Largest Even Value
**Problem.** Among the readings there is a largest even one.
**Task.** Read `T`, then `T` values; print the largest even value. (At least one even value is guaranteed.)
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the largest even value.
**Sample**
```
Input          Output
5              22
7
14
3
22
9
```

## Q15. Smallest Value Above x
**Problem.** Among the readings greater than `x`, one is smallest.
**Task.** Read `x`, then `T`, then `T` values; print the smallest value that is strictly greater than `x`. (At least one such value is guaranteed.)
**Input Format**
Line 1: integer `x`
Line 2: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the smallest value above `x`.
**Sample**
```
Input          Output
10             11
5
8
25
12
40
11
```

---

## Section B — Previous-Value Patterns

## Q16. Count the Increases
**Problem.** A reading counts as an increase when it is strictly greater than the reading just before it.
**Task.** Read `T`, then `T` values; print how many increases occur.
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the count of increases.
**Sample**
```
Input          Output
6              3
3
5
4
8
8
10
```

## Q17. Count the Decreases
**Problem.** A reading counts as a decrease when it is strictly smaller than the one before it.
**Task.** Read `T`, then `T` values; print how many decreases occur.
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the count of decreases.
**Sample**
```
Input          Output
6              3
9
4
6
2
2
1
```

## Q18. Largest Jump
**Problem.** Between consecutive readings there is a gap, measured without sign.
**Task.** Read `T`, then `T` values; print the largest gap between two consecutive readings.
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the largest gap.
**Sample**
```
Input          Output
5              11
10
4
15
12
20
```

## Q19. Equal Neighbours
**Problem.** Sometimes a reading repeats the one just before it.
**Task.** Read `T`, then `T` values; print how many readings equal their immediate predecessor.
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
7              3
2
2
5
7
7
7
1
```

## Q20. Longest Rising Run
**Problem.** A rising run is a stretch of readings where each is strictly greater than the one before; its length is counted in readings (a single reading is a run of 1).
**Task.** Read `T`, then `T` values; print the length of the longest rising run.
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the longest run length.
**Sample**
```
Input          Output
7              4
1
5
2
4
6
9
3
```

## Q21. Longest Even Streak
**Problem.** A streak of evens is a stretch of consecutive even readings.
**Task.** Read `T`, then `T` values; print the length of the longest streak of even values (print 0 if there are none).
**Input Format**
Line 1: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the longest streak.
**Sample**
```
Input          Output
8              4
1
4
6
3
8
2
4
6
```

## Q22. Peak Count
**Problem.** A reading is a peak when it is strictly greater than both its neighbours (the first and last readings cannot be peaks).
**Task.** Read `T`, then `T` values; print how many peaks there are.
**Input Format**
Line 1: integer `T`  (T ≥ 3)
Next `T` lines: one integer each
**Output Format.** A single integer — the peak count.
**Sample**
```
Input          Output
7              3
1
5
2
8
3
9
4
```

## Q23. First Position Above x
**Problem.** At some point a reading first rises above `x`.
**Task.** Read `x`, then `T`, then `T` values; print the 1-based position of the first value strictly greater than `x`. (Guaranteed to exist.)
**Input Format**
Line 1: integer `x`
Line 2: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the position.
**Sample**
```
Input          Output
20             4
6
5
12
8
25
30
2
```

## Q24. Parity Switches
**Problem.** A parity switch happens when a reading's evenness differs from the previous reading's (even after odd, or odd after even).
**Task.** Read `T`, then `T` values; print how many parity switches occur.
**Input Format**
Line 1: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the count of switches.
**Sample**
```
Input          Output
6              3
3
8
5
7
2
4
```

---

## Section C — Sentinel Streams

## Q25. Sum until Zero
**Problem.** Values arrive until a 0 marks the end (the 0 is not data).
**Task.** Keep reading integers until 0; print the sum of the values before it.
**Input Format**
One integer per line, ending with 0
**Output Format.** A single integer — the sum.
**Sample**
```
Input          Output
5              10
3
2
0
```

## Q26. Positives before the First Negative
**Problem.** The stream ends the moment a negative value appears.
**Task.** Keep reading integers until a negative one; print how many values came before it.
**Input Format**
One integer per line; the stream ends at the first negative value
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
7              3
3
9
-2
```

## Q27. Maximum until Zero
**Problem.** Values arrive until a 0 marks the end.
**Task.** Keep reading integers until 0; print the largest value seen. (At least one value comes before the 0.)
**Input Format**
One integer per line, ending with 0
**Output Format.** A single integer — the maximum.
**Sample**
```
Input          Output
6              14
14
3
9
0
```

## Q28. Multiples of Five until Zero
**Problem.** Values arrive until a 0 marks the end.
**Task.** Keep reading integers until 0; print how many of the values were divisible by 5.
**Input Format**
One integer per line, ending with 0
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
10             3
3
15
8
20
0
```

## Q29. Floor Average until Zero
**Problem.** Values arrive until a 0 marks the end.
**Task.** Keep reading integers until 0; print the floor average (sum // count) of the values. (At least one value is guaranteed.)
**Input Format**
One integer per line, ending with 0
**Output Format.** A single integer — the floor average.
**Sample**
```
Input          Output
9              7
4
8
0
```

## Q30. Readings to Beat a Target
**Problem.** A running total climbs with each value until it passes a target.
**Task.** Read a target `S`, then keep reading values; print how many values it took for the running total to become strictly greater than `S`. (Guaranteed to happen.)
**Input Format**
Line 1: integer `S`  (1 ≤ S ≤ 10⁹)
Following lines: one integer per line
**Output Format.** A single integer — the number of values read.
**Sample**
```
Input          Output
20             4
6
8
3
9
```

## Q31. Odds before the First Even
**Problem.** The stream ends the moment an even value appears.
**Task.** Keep reading integers until an even one; print how many odd values came before it.
**Input Format**
One integer per line; the stream ends at the first even value
**Output Format.** A single integer — the count.
**Sample**
```
Input          Output
5              3
9
3
8
```

## Q32. First Immediate Repeat
**Problem.** Eventually a value arrives that equals the one just before it.
**Task.** Keep reading integers; the first time a value equals its immediate predecessor, print that value and stop. (Guaranteed to happen.)
**Input Format**
One integer per line
**Output Format.** A single integer — the repeated value.
**Sample**
```
Input          Output
4              3
7
3
3
```

---

## Section D — Streaks & Swings

## Q33. Longest Streak at or above x
**Problem.** A qualifying streak is a stretch of consecutive readings that are all ≥ `x`.
**Task.** Read `x`, then `T`, then `T` values; print the length of the longest streak of values ≥ `x` (0 if none).
**Input Format**
Line 1: integer `x`
Line 2: integer `T`
Next `T` lines: one integer each
**Output Format.** A single integer — the longest streak.
**Sample**
```
Input          Output
10             3
8
5
12
14
9
11
16
13
2
```

## Q34. Big Swings
**Problem.** A big swing happens when a reading differs from the previous one by more than `d` (ignoring sign).
**Task.** Read `d`, then `T`, then `T` values; print how many big swings occur.
**Input Format**
Line 1: integer `d`  (1 ≤ d ≤ 10⁹)
Line 2: integer `T`  (T ≥ 2)
Next `T` lines: one integer each
**Output Format.** A single integer — the count of big swings.
**Sample**
```
Input          Output
5              2
6
10
12
20
22
9
11
```

---

*End of Batch 3 — 34 questions, every sample output generated by a verified reference solution.*
