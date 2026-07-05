# Coding Bank — Batch 1: Scenario & Word Problems (1–20)

*Unit 3 · Functions and Recursion. Judge-format problems: read input with `input()`/`int()` in the exact order given (no prompt text), produce exact-match output. Each names a **Required function** you must define. Money is handled in whole units (paise/cents) internally and shown to 2 decimals with `f"{value:.2f}"` — note that `round()` drops trailing zeros and will fail the judge, so use the f-string form.*

*Difficulty: [E] easy · [M] medium · [H] hard. Reference solutions in `coding-bank-01-scenario-solutions.md`.*

---

## 1 — Lemonade Pitchers  [M]

A pitcher of lemonade needs a fixed number of teaspoons of sugar and a fixed number of lemons. Given how much sugar and how many lemons are available, find how many **full** pitchers can be made, and how much of each ingredient is left over.

**Required function:** `pitchers(sugar_per, lemons_per, sugar_have, lemons_have)` returning the number of full pitchers.

**Input Format:** Four integers, each on its own line — sugar per pitcher, lemons per pitcher, sugar available, lemons available (all 1–100000).

**Output Format:** Three integers separated by single spaces: pitchers, leftover sugar, leftover lemons.

**Sample Input:**
```
3
2
20
8
```
**Sample Output:**
```
4 8 0
```

---

## 2 — Restaurant Overlap  [H]

Anna and Bob each arrive at and leave a restaurant, given as minutes after midnight. Determine whether they were there at the same time, and if so for how many minutes. If one leaves exactly as the other arrives, they did **not** overlap.

**Required function:** `overlap(a_in, a_out, b_in, b_out)` returning the number of overlapping minutes (0 if none).

**Input Format:** Four integers, each on its own line — Anna in, Anna out, Bob in, Bob out (0 ≤ each ≤ 1440, each person's out > in).

**Output Format:** If they overlapped, `Yes` and the number of minutes separated by a space. Otherwise `No`.

**Sample Input:**
```
720
800
600
740
```
**Sample Output:**
```
Yes 20
```

---

## 3 — Cereal Bulk Pricing  [H]

Two companies price cereal boxes in three tiers: the first 100 boxes at one price, the next 1000 at a second price, and all further boxes at a third price. Given both companies' three prices and the number of boxes wanted, print which company is cheaper (1 or 2) and the total cost. If the costs tie, print company 1. Prices are given in **cents** (whole numbers); print the cost in dollars to 2 decimals.

**Required function:** `cost(p1, p2, p3, n)` returning the total cost in cents for buying `n` boxes at tier prices `p1`, `p2`, `p3`.

**Input Format:** Seven integers, each on its own line — company 1's three tier prices (cents), company 2's three tier prices (cents), then the number of boxes `n` (1 ≤ n ≤ 1000000).

**Output Format:** The chosen company number and the cost to 2 decimals, separated by a space.

**Sample Input:**
```
299
199
150
250
225
175
2000
```
**Sample Output:**
```
1 3639.00
```

---

## 4 — Planet C Leap Year  [M]

On planet C a year is a leap year if it is divisible by 7, **except** when it is also divisible by 35 or by 77 (those are not leap years). Print whether the given year is a leap year.

**Required function:** `is_leap(y)` returning `True` if `y` is a leap year on planet C.

**Input Format:** A single positive integer `y` (1 ≤ y ≤ 1000000).

**Output Format:** `Leap` if it is a leap year, otherwise `Not`.

**Sample Input:**
```
49
```
**Sample Output:**
```
Leap
```

---

## 5 — Making Change  [M]

A vending machine returns change using quarters (25), dimes (10), nickels (5) and pennies (1), using as few coins as possible (greedy from the largest coin down). Given an amount in cents, print how many of each coin are returned.

**Required function:** `change(cents)` returning four values — quarters, dimes, nickels, pennies.

**Input Format:** A single integer `cents` (0 ≤ cents ≤ 100000).

**Output Format:** Four integers separated by single spaces: quarters, dimes, nickels, pennies.

**Sample Input:**
```
99
```
**Sample Output:**
```
3 2 0 4
```

---

## 6 — Seating Rows  [E]

A hall seats a fixed number of people per row. Given the number of people and seats per row, print how many rows are completely full and how many people sit in the last, partly-filled row.

**Required function:** `seating(people, per_row)` returning two values — full rows and people in the last partial row.

**Input Format:** Two integers, each on its own line — people, then seats per row (1 ≤ each ≤ 100000).

**Output Format:** Two integers separated by a space: full rows, then people in the partial row (0 if the last row is exactly full).

**Sample Input:**
```
23
5
```
**Sample Output:**
```
4 3
```

---

## 7 — Age in Days  [E]

Using a simple calendar where every year is 365 days and every month is 30 days, convert an age given in years, months and days into a total number of days.

**Required function:** `to_days(years, months, days)` returning the total number of days.

**Input Format:** Three integers, each on its own line — years, months, days (0 ≤ each ≤ 1000).

**Output Format:** A single integer — the total number of days.

**Sample Input:**
```
1
2
3
```
**Sample Output:**
```
428
```

---

## 8 — Income Tax  [H]

Income (in cents) is taxed in bands: the first 1000 (i.e. 100000 cents) is tax-free; the part from 1000 up to 5000 is taxed at 10%; anything above 5000 is taxed at 20%. Print the total tax owed, in whole currency units to 2 decimals.

**Required function:** `tax(income)` returning the tax in cents.

**Input Format:** A single integer `income` in cents (0 ≤ income ≤ 100000000).

**Output Format:** The tax to 2 decimals.

**Sample Input:**
```
700000
```
**Sample Output:**
```
800.00
```

---

## 9 — Trip Fuel Cost  [M]

A car travels a distance at a known mileage (km per litre). Given the fuel price per litre in cents, print the total fuel cost to 2 decimals.

**Required function:** `fuel_cost(distance, mileage, price)` returning the cost in cents (may be fractional).

**Input Format:** Three integers, each on its own line — distance in km, mileage in km/litre, price per litre in cents (all 1–1000000).

**Output Format:** The fuel cost to 2 decimals.

**Sample Input:**
```
300
15
10000
```
**Sample Output:**
```
2000.00
```

---

## 10 — Digital Clock  [M]

Given a number of minutes after midnight, print the time on a 24-hour digital clock as `HH:MM`, with both fields zero-padded to two digits.

**Required function:** `hm(minutes)` returning two values — hours and minutes.

**Input Format:** A single integer `minutes` (0 ≤ minutes ≤ 1439).

**Output Format:** The time as `HH:MM` (two digits each).

**Sample Input:**
```
125
```
**Sample Output:**
```
02:05
```

---

## 11 — Bulk Discount  [M]

A shop gives 10% off the whole bill when 100 or more units are bought. Given the quantity and the unit price in cents, print the final bill to 2 decimals.

**Required function:** `discounted_bill(qty, price)` returning the final bill in cents (use integer arithmetic: `total - total * 10 // 100`).

**Input Format:** Two integers, each on its own line — quantity, then unit price in cents (1 ≤ each ≤ 1000000).

**Output Format:** The final bill to 2 decimals.

**Sample Input:**
```
100
500
```
**Sample Output:**
```
450.00
```

---

## 12 — Elevator Trips  [M]

An elevator carries a fixed number of people per trip. Given the number of people waiting and the capacity, print how many trips are needed so everyone is carried (a partly-full final trip still counts).

**Required function:** `trips(people, capacity)` returning the number of trips.

**Input Format:** Two integers, each on its own line — people, then capacity (1 ≤ each ≤ 1000000).

**Output Format:** A single integer — the number of trips.

**Sample Input:**
```
95
20
```
**Sample Output:**
```
5
```

---

## 13 — Filling a Tank  [H]

Water flows into a tank at a fill rate and leaks out at a drain rate (both litres per minute). Given the tank's capacity, print how many whole minutes until it is full. If the drain rate is at least the fill rate, it never fills — print `-1`.

**Required function:** `fill_time(fill, drain, capacity)` returning the minutes to fill, or −1 if it never fills.

**Input Format:** Three integers, each on its own line — fill rate, drain rate, capacity (1 ≤ each ≤ 1000000).

**Output Format:** A single integer — the whole minutes to fill (rounded up), or `-1`.

**Sample Input:**
```
10
4
60
```
**Sample Output:**
```
10
```

---

## 14 — Drop the Lowest  [M]

A student has four test scores. The lowest score is dropped and the average of the remaining three is taken. Print that average to 2 decimals.

**Required function:** `avg_best3(a, b, c, d)` returning the average of the best three scores.

**Input Format:** Four integers, each on its own line — the four scores (0 ≤ each ≤ 100).

**Output Format:** The average of the best three, to 2 decimals.

**Sample Input:**
```
60
70
80
90
```
**Sample Output:**
```
80.00
```

---

## 15 — Two Trains Meet  [M]

Two trains start a given distance apart and move toward each other at their own speeds (km/h). Print how many hours until they meet, to 2 decimals.

**Required function:** `meet(distance, speed1, speed2)` returning the time in hours.

**Input Format:** Three integers, each on its own line — distance in km, speed1, speed2 (all 1–100000).

**Output Format:** The meeting time in hours, to 2 decimals.

**Sample Input:**
```
300
40
60
```
**Sample Output:**
```
3.00
```

---

## 16 — Family Ticket  [M]

A cinema charges 500 cents per adult and 250 cents per child. If the total number of people is 4 or more, the whole bill gets 10% off. Print the final cost to 2 decimals.

**Required function:** `total_cost(adults, kids)` returning the final cost in cents.

**Input Format:** Two integers, each on its own line — adults, then children (0 ≤ each ≤ 1000).

**Output Format:** The final cost to 2 decimals.

**Sample Input:**
```
2
2
```
**Sample Output:**
```
13.50
```

---

## 17 — Time Difference  [H]

Two events are given as seconds after midnight. Print the time between them as `HH:MM:SS`, each field zero-padded, regardless of which event is earlier.

**Required function:** `diff(t1, t2)` returning three values — hours, minutes, seconds of the gap.

**Input Format:** Two integers, each on its own line — the two times in seconds (0 ≤ each ≤ 86400).

**Output Format:** The gap as `HH:MM:SS` (two digits each).

**Sample Input:**
```
3600
7325
```
**Sample Output:**
```
01:02:05
```

---

## 18 — Paint Cans  [E]

One can of paint covers a fixed area. Given a wall's area and the coverage per can, print how many cans are needed (a partly-used can still counts as one).

**Required function:** `cans(area, coverage)` returning the number of cans.

**Input Format:** Two integers, each on its own line — wall area, then coverage per can (1 ≤ each ≤ 1000000).

**Output Format:** A single integer — the cans needed.

**Sample Input:**
```
50
12
```
**Sample Output:**
```
5
```

---

## 19 — Purchase Discount Tiers  [H]

A purchase amount (in cents) earns a discount: over 20000 (i.e. 2000000 cents) gets 20% off; over 10000 gets 10% off; otherwise no discount. Print the final amount to 2 decimals.

**Required function:** `final_amt(amount)` returning the final amount in cents.

**Input Format:** A single integer `amount` in cents (0 ≤ amount ≤ 100000000).

**Output Format:** The final amount to 2 decimals.

**Sample Input:**
```
2500000
```
**Sample Output:**
```
20000.00
```

---

## 20 — Bus Boarding  [E]

Passengers board buses of a fixed capacity. Given the total passengers and the capacity, print how many buses leave completely full and how many passengers are left waiting.

**Required function:** `buses(passengers, capacity)` returning two values — full buses and passengers left waiting.

**Input Format:** Two integers, each on its own line — passengers, then capacity (1 ≤ each ≤ 1000000).

**Output Format:** Two integers separated by a space: full buses, then passengers waiting.

**Sample Input:**
```
130
40
```
**Sample Output:**
```
3 10
```

---

*End of Batch 1 — 20 scenario problems. Every reference solution verified against the sample and additional edge cases.*
