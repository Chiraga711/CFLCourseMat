# Platform Question Pool — Batch 4: Real-World Scenarios (46 Questions — Decimals Enabled)

**Conventions.** Inputs come one value per line — whole numbers are read with `int(input())`, float values with `float(input())`; no prompts. **Two-decimal outputs:** where a question asks for two decimal places, print with the fixed recipe `print(f"{ans:.2f}")`. That recipe is the only string feature used, and every expected output was generated with the same recipe, so matching is exact. Integer answers are printed plainly. All money is in rupees; every calculation is designed to be exact at two decimals (or rounded identically for everyone by the shared recipe).

---

## Section A — Direct Calculation

## Q1. Metro Fare
**Problem.** A metro ride costs a flat ₹10 plus ₹5 for every zone crossed.
**Task.** Read the number of zones `z`; print the fare.
**Input Format**
Line 1: integer `z`  (1 ≤ z ≤ 20)
**Output Format.** A single integer — the fare.
**Sample**
```
Input          Output
4              30
```

## Q2. Cyber Café Bill
**Problem.** A cyber café charges ₹30 for the first hour and ₹20 for each additional hour.
**Task.** Read the hours used `h`; print the bill.
**Input Format**
Line 1: integer `h`  (1 ≤ h ≤ 24)
**Output Format.** A single integer — the bill.
**Sample**
```
Input          Output
5              110
```

## Q3. Print Shop
**Problem.** A print shop charges ₹1.50 per black-and-white page and ₹9.75 per colour page.
**Task.** Read the black-and-white page count `p` and colour page count `c`; print the total.
**Input Format**
Line 1: integer `p`
Line 2: integer `c`  (0 ≤ p, c ≤ 10⁴)
**Output Format.** A single number with exactly two decimal places — the total.
**Sample**
```
Input          Output
12             47.25
3
```

## Q4. Tailor's Order
**Problem.** A tailor stitches a shirt for ₹350 and a pair of trousers for ₹500.
**Task.** Read the shirt count `s` and trouser count `t`; print the order total.
**Input Format**
Line 1: integer `s`
Line 2: integer `t`  (0 ≤ s, t ≤ 100)
**Output Format.** A single integer — the total.
**Sample**
```
Input          Output
3              2050
2
```

## Q5. Milk Bill
**Problem.** A family takes the same litres of milk every day for a whole billing period, at a float rate per litre.
**Task.** Read litres per day `l`, number of days `d`, and rate per litre `r`; print the bill.
**Input Format**
Line 1: integer `l`  (1 ≤ l ≤ 10)
Line 2: integer `d`  (1 ≤ d ≤ 31)
Line 3: float `r`  (e.g., 56.50)
**Output Format.** A single number with exactly two decimal places — the bill.
**Sample**
```
Input          Output
2              3390.00
30
56.50
```

## Q6. Piggy Bank
**Problem.** A piggy bank holds ₹1, ₹2, and ₹5 coins.
**Task.** Read the counts of ₹1, ₹2, and ₹5 coins; print the total money inside.
**Input Format**
Line 1: integer — count of ₹1 coins
Line 2: integer — count of ₹2 coins
Line 3: integer — count of ₹5 coins  (each 0 ≤ count ≤ 10⁴)
**Output Format.** A single integer — the total value.
**Sample**
```
Input          Output
12             53
8
5
```

## Q7. Zoo Entry
**Problem.** Zoo tickets cost ₹150 per adult and ₹80 per child, plus a flat ₹50 camera fee if a camera is brought.
**Task.** Read the adult count `a`, child count `c`, and a camera flag (1 = yes, 0 = no); print the total.
**Input Format**
Line 1: integer `a`
Line 2: integer `c`  (0 ≤ a, c ≤ 100)
Line 3: integer camera flag (0 or 1)
**Output Format.** A single integer — the total.
**Sample**
```
Input          Output
2              590
3
1
```

## Q8. Minimum Notes
**Problem.** A cashier pays any amount using notes of ₹500, ₹100, ₹50, ₹10, and ₹1, always using as few notes as possible.
**Task.** Read an amount; print the minimum number of notes needed.
**Input Format**
Line 1: integer amount  (1 ≤ amount ≤ 10⁶)
**Output Format.** A single integer — the note count.
**Sample**
```
Input          Output
3678           19
```

## Q9. Trek Fee Split
**Problem.** A trekking group splits the guide's fee equally; shares are paid to the paisa.
**Task.** Read the fee `F` and group size `p`; print each person's share.
**Input Format**
Line 1: float `F`  (1 ≤ F ≤ 10⁵)
Line 2: integer `p`  (1 ≤ p ≤ 50)
**Output Format.** A single number with exactly two decimal places — the share.
**Sample**
```
Input          Output
1750           291.67
6
```

## Q10. Token Wait
**Problem.** At a service counter, each customer takes exactly `t` minutes, served strictly in token order.
**Task.** Read your token number `k` and the minutes per customer `t`; print how many minutes you wait before your turn starts.
**Input Format**
Line 1: integer `k`  (1 ≤ k ≤ 10⁴)
Line 2: integer `t`  (1 ≤ t ≤ 60)
**Output Format.** A single integer — the waiting minutes.
**Sample**
```
Input          Output
8              28
4
```

---

## Section B — Slabs, Flags & Discounts

## Q11. Borewell Drilling
**Problem.** Drilling a borewell costs ₹80 per foot for the first 100 feet, ₹120 per foot for the next 100 feet, and ₹200 per foot beyond that — each slab charged only on the feet within it.
**Task.** Read the depth `d` in feet; print the drilling cost.
**Input Format**
Line 1: integer `d`  (1 ≤ d ≤ 1000)
**Output Format.** A single integer — the cost.
**Sample**
```
Input          Output
250            30000
```

## Q12. Gold Making Charges
**Problem.** A jeweller's making charge depends on the weight: up to 10 g it is a flat ₹300; up to 50 g it is ₹25.50 per gram; above 50 g it is ₹20.75 per gram. Weights can be floats.
**Task.** Read the weight `w` in grams; print the making charge.
**Input Format**
Line 1: float `w`  (0.1 ≤ w ≤ 500)
**Output Format.** A single number with exactly two decimal places — the charge.
**Sample**
```
Input          Output
12.5           318.75
```

## Q13. Cable TV Bill
**Problem.** A cable plan has a ₹150 base charge. Optional packs cost extra: sports ₹60, movies ₹80, kids ₹40.
**Task.** Read three flags (1 = taken, 0 = not) for sports, movies, and kids; print the monthly bill.
**Input Format**
Line 1: integer sports flag
Line 2: integer movies flag
Line 3: integer kids flag  (each 0 or 1)
**Output Format.** A single integer — the bill.
**Sample**
```
Input          Output
1              250
0
1
```

## Q14. School Van Fee
**Problem.** The monthly van fee depends on distance: up to 3 km it is ₹600; up to 7 km it is ₹900; beyond 7 km it is ₹900 plus ₹80 for every kilometre over 7.
**Task.** Read the distance `km`; print the fee.
**Input Format**
Line 1: integer `km`  (1 ≤ km ≤ 50)
**Output Format.** A single integer — the fee.
**Sample**
```
Input          Output
10             1140
```

## Q15. Turf Booking
**Problem.** A sports turf charges ₹800 per hour for the first 2 hours and ₹1200 per hour after that.
**Task.** Read the hours booked `h`; print the cost.
**Input Format**
Line 1: integer `h`  (1 ≤ h ≤ 12)
**Output Format.** A single integer — the cost.
**Sample**
```
Input          Output
5              5200
```

## Q16. Weekend Pricing
**Problem.** A shop adds a 20% weekend surcharge to its prices. Days are numbered 1 (Monday) to 7 (Sunday); days 6 and 7 are the weekend.
**Task.** Read the day number and the base price `b`; print the final price.
**Input Format**
Line 1: integer day  (1 ≤ day ≤ 7)
Line 2: integer `b`  (1 ≤ b ≤ 10⁵)
**Output Format.** A single number with exactly two decimal places — the final price.
**Sample**
```
Input          Output
6              543.60
453
```

## Q17. Coupon
**Problem.** A store coupon takes a flat ₹250 off any bill of ₹2000 or more; smaller bills get nothing.
**Task.** Read the bill `B`; print the amount payable.
**Input Format**
Line 1: float `B`  (1 ≤ B ≤ 10⁶)
**Output Format.** A single number with exactly two decimal places — the payable amount.
**Sample**
```
Input          Output
2599.50        2349.50
```

## Q18. Buy Three, Get One Free
**Problem.** A sweet stall runs a "buy 3, get 1 free" offer: for every 4 boxes ordered, only 3 are charged.
**Task.** Read the boxes ordered `q` and the price per box `r`; print the amount payable.
**Input Format**
Line 1: integer `q`  (1 ≤ q ≤ 1000)
Line 2: float `r`  (e.g., 89.50)
**Output Format.** A single number with exactly two decimal places — the amount payable.
**Sample**
```
Input          Output
10             716.00
89.50
```

## Q19. Coaching Combo
**Problem.** A coaching centre charges ₹1200 per subject, with 10% off the total for students taking 3 or more subjects (totals are always multiples of 10, so the discount is exact).
**Task.** Read the subject count `s`; print the fee.
**Input Format**
Line 1: integer `s`  (1 ≤ s ≤ 8)
**Output Format.** A single integer — the fee.
**Sample**
```
Input          Output
4              4320
```

## Q20. Security Shifts
**Problem.** A security guard earns ₹700 for a day shift and ₹900 for a night shift.
**Task.** Read the day-shift count `d` and night-shift count `n`; print the month's earnings.
**Input Format**
Line 1: integer `d`
Line 2: integer `n`  (0 ≤ d, n ≤ 31)
**Output Format.** A single integer — the earnings.
**Sample**
```
Input          Output
12             15600
8
```

---

## Section C — Grouping & Ceiling Division

## Q21. Exam Benches
**Problem.** An exam hall seats exactly 3 students per bench; a partly-filled bench still counts.
**Task.** Read the student count `n`; print the benches needed.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the bench count.
**Sample**
```
Input          Output
26             9
```

## Q22. Vaccine Vials
**Problem.** Each vial holds 10 doses; an opened vial is used for the day even if not emptied.
**Task.** Read the people to vaccinate `n`; print the vials needed.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁵)
**Output Format.** A single integer — the vial count.
**Sample**
```
Input          Output
94             10
```

## Q23. Cable Car Trips
**Problem.** A cable car carries at most 6 visitors per trip.
**Task.** Read the visitor count `n`; print the trips needed to carry everyone.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 10⁴)
**Output Format.** A single integer — the trip count.
**Sample**
```
Input          Output
27             5
```

## Q24. Tiling a Floor
**Problem.** A rectangular floor of `l` × `w` cm is covered with square tiles of side `a` cm. Tiles may be cut, but each started tile counts, along each direction.
**Task.** Read `l`, `w`, and `a`; print the tiles needed — (tiles along the length) × (tiles along the width).
**Input Format**
Line 1: integer `l`
Line 2: integer `w`  (1 ≤ l, w ≤ 10⁴)
Line 3: integer `a`  (1 ≤ a ≤ 100)
**Output Format.** A single integer — the tile count.
**Sample**
```
Input          Output
125            35
90
20
```

## Q25. Paint Cans
**Problem.** A wall of `l` × `h` metres needs two coats of paint. One can covers `c` square metres; a started can counts.
**Task.** Read `l`, `h`, and `c`; print the cans needed for both coats.
**Input Format**
Line 1: integer `l`
Line 2: integer `h`  (1 ≤ l, h ≤ 100)
Line 3: integer `c`  (1 ≤ c ≤ 100)
**Output Format.** A single integer — the can count.
**Sample**
```
Input          Output
10             6
4
15
```

## Q26. Loose Bottles
**Problem.** Water bottles are packed into crates of 12; whatever cannot fill a crate is left loose.
**Task.** Read the bottle count `b`; print how many bottles are left loose.
**Input Format**
Line 1: integer `b`  (1 ≤ b ≤ 10⁵)
**Output Format.** A single integer — the loose bottles (0–11).
**Sample**
```
Input          Output
94             10
```

## Q27. Badminton Slots
**Problem.** A badminton court is booked in 30-minute slots at ₹62.50 per slot; any started slot must be paid in full.
**Task.** Read the minutes of play `m`; print the booking cost.
**Input Format**
Line 1: integer `m`  (1 ≤ m ≤ 600)
**Output Format.** A single number with exactly two decimal places — the cost.
**Sample**
```
Input          Output
100            250.00
```

## Q28. Orchard Crates
**Problem.** An orchard has `t` mango trees, each yielding `y` mangoes. The harvest is packed into crates that hold `c` mangoes; a partly-filled crate is still used.
**Task.** Read `t`, `y`, and `c`; print the crates needed.
**Input Format**
Line 1: integer `t`  (1 ≤ t ≤ 1000)
Line 2: integer `y`  (1 ≤ y ≤ 1000)
Line 3: integer `c`  (1 ≤ c ≤ 1000)
**Output Format.** A single integer — the crate count.
**Sample**
```
Input          Output
18             9
45
100
```

---

## Section D — Growth & Repetition

## Q29. Newspaper Bill
**Problem.** A newspaper costs `r1` on weekdays and `r2` on Sundays (both can be floats). Day 1 of the month is a Monday, so every day number divisible by 7 is a Sunday.
**Task.** Read the days in the month `N` and the two rates; print the month's bill.
**Input Format**
Line 1: integer `N`  (1 ≤ N ≤ 31)
Line 2: float `r1`
Line 3: float `r2`  (e.g., 6.50)
**Output Format.** A single number with exactly two decimal places — the bill.
**Sample**
```
Input          Output
30             217.00
6.50
12.00
```

## Q30. Milkman's Odd Days
**Problem.** A milkman delivers only on the odd-numbered days of the month — `l` litres each delivery (litres can be floats, like 1.5) at ₹`r` per litre.
**Task.** Read the days in the month `N`, litres `l`, and rate `r`; print the month's bill.
**Input Format**
Line 1: integer `N`  (1 ≤ N ≤ 31)
Line 2: float `l`  (0.5 ≤ l ≤ 10)
Line 3: float `r`  (1 ≤ r ≤ 100)
**Output Format.** A single number with exactly two decimal places — the bill.
**Sample**
```
Input          Output
30             1440.00
1.5
64
```

## Q31. Tiffin Service
**Problem.** A tiffin service delivers on weekdays only. Day 1 is a Monday, so days where the day number leaves remainder 6 or 0 when divided by 7 are the weekend. Each tiffin costs ₹`p`.
**Task.** Read the number of days `N` and the price `p`; print the total for all weekday tiffins.
**Input Format**
Line 1: integer `N`  (1 ≤ N ≤ 31)
Line 2: integer `p`  (1 ≤ p ≤ 200)
**Output Format.** A single integer — the total.
**Sample**
```
Input          Output
14             800
80
```

## Q32. Plant Growth
**Problem.** A sapling of height `h` cm grows exactly `g` cm every week (measurements can be floats).
**Task.** Read `h`, `g`, and a target height `H`; print how many weeks until the plant's height is at least `H`.
**Input Format**
Line 1: float `h`
Line 2: float `g`  (0.5 ≤ g ≤ 100)
Line 3: float `H`  (h < H ≤ 10⁵)
**Output Format.** A single integer — the weeks needed.
**Sample**
```
Input          Output
15.5           5
7.25
50
```

## Q33. Candle Burn
**Problem.** A candle of length `L` mm burns `b` mm every hour. Once shorter than `s` mm it can no longer hold a flame.
**Task.** Read `L`, `b`, and `s`; print how many full hours the candle burns before its length first drops below `s`.
**Input Format**
Line 1: integer `L`
Line 2: integer `b`  (1 ≤ b ≤ 100)
Line 3: integer `s`  (1 ≤ s ≤ L ≤ 10⁵)
**Output Format.** A single integer — the hours burned.
**Sample**
```
Input          Output
100            6
12
30
```

## Q34. Battery Drain
**Problem.** A phone starts at 100% charge and loses `d` percent every hour of use. It shows a warning once the charge is 20 or less.
**Task.** Read the drain rate `d`; print after how many hours the warning first appears.
**Input Format**
Line 1: integer `d`  (1 ≤ d ≤ 80)
**Output Format.** A single integer — the hours.
**Sample**
```
Input          Output
13             7
```

## Q35. Push-up Challenge
**Problem.** On day 1 you do `n` push-ups, and each day you do 2 more than the day before.
**Task.** Read `n` and a goal `G`; print on which day your total push-ups first reach at least `G`.
**Input Format**
Line 1: integer `n`  (1 ≤ n ≤ 100)
Line 2: integer `G`  (n ≤ G ≤ 10⁶)
**Output Format.** A single integer — the day number.
**Sample**
```
Input          Output
10             7
100
```

## Q36. Game Levels
**Problem.** Reaching level 2 needs 100 XP, and each next level needs double the previous requirement (200, 400, …). A player spends XP level by level.
**Task.** Read the total XP earned `X`; print the level reached (players start at level 1).
**Input Format**
Line 1: integer `X`  (0 ≤ X ≤ 10⁹)
**Output Format.** A single integer — the level.
**Sample**
```
Input          Output
750            4
```

## Q37. Town Population
**Problem.** A town of `p` people grows by `r` percent each year, always rounded down (each year: p = p + p × r // 100).
**Task.** Read `p`, `r`, and the years `y`; print the population after `y` years.
**Input Format**
Line 1: integer `p`  (1 ≤ p ≤ 10⁶)
Line 2: integer `r`  (1 ≤ r ≤ 50)
Line 3: integer `y`  (1 ≤ y ≤ 50)
**Output Format.** A single integer — the final population.
**Sample**
```
Input          Output
1000           1224
7
3
```

## Q38. Frog in a Well
**Problem.** A frog at the bottom of an `H`-metre well climbs `a` metres each hour but slips back `b` metres before the next hour begins. Once it reaches the top it is out and slips no more.
**Task.** Read `H`, `a`, and `b` (a > b); print the hour in which the frog gets out.
**Input Format**
Line 1: integer `H`  (1 ≤ H ≤ 10⁵)
Line 2: integer `a`
Line 3: integer `b`  (0 ≤ b < a ≤ 100)
**Output Format.** A single integer — the hour.
**Sample**
```
Input          Output
30             6
7
2
```

---

## Section E — Scenario Streams

## Q39. Chess Rating
**Problem.** A player's rating rises 25 points for a win and falls 15 for a loss.
**Task.** Read the starting rating, then `T`, then `T` results (1 = win, 0 = loss); print the final rating.
**Input Format**
Line 1: integer starting rating  (1 ≤ rating ≤ 3000)
Line 2: integer `T`  (1 ≤ T ≤ 1000)
Next `T` lines: 1 or 0
**Output Format.** A single integer — the final rating.
**Sample**
```
Input          Output
1200           1245
5
1
0
1
1
0
```

## Q40. Marks Moderation
**Problem.** The board adds `m` grace marks to every student's score, but no score may exceed 100.
**Task.** Read `T` and `m`, then `T` scores; print the sum of all scores after moderation.
**Input Format**
Line 1: integer `T`  (1 ≤ T ≤ 1000)
Line 2: integer `m`  (1 ≤ m ≤ 20)
Next `T` lines: one score each  (0 ≤ score ≤ 100)
**Output Format.** A single integer — the moderated total.
**Sample**
```
Input          Output
4              374
8
95
70
88
97
```

## Q41. Attendance Percent
**Problem.** A register records 1 for a present day and 0 for an absent day. The attendance percentage is (present days × 100) divided by total days.
**Task.** Read `N`, then `N` entries of 1/0; print the attendance percentage.
**Input Format**
Line 1: integer `N`  (1 ≤ N ≤ 366)
Next `N` lines: 1 or 0
**Output Format.** A single number with exactly two decimal places — the percentage.
**Sample**
```
Input          Output
8              75.00
1
1
0
1
1
1
0
1
```

## Q42. Delivery Rider
**Problem.** A rider earns ₹22.50 per order, plus a ₹200 daily bonus on any day with 15 or more orders.
**Task.** Read the days `D`, then each day's order count; print the total earnings.
**Input Format**
Line 1: integer `D`  (1 ≤ D ≤ 31)
Next `D` lines: one order count each  (0 ≤ orders ≤ 100)
**Output Format.** A single number with exactly two decimal places — the earnings.
**Sample**
```
Input          Output
3              1367.50
12
16
15
```

## Q43. Loss Days
**Problem.** A shop's daily profit can be a float, and negative (a loss).
**Task.** Read `T`, then `T` daily profits (floats, possibly negative); print how many days were losses.
**Input Format**
Line 1: integer `T`  (1 ≤ T ≤ 366)
Next `T` lines: one float each  (−10⁵ ≤ profit ≤ 10⁵)
**Output Format.** A single integer — the loss-day count.
**Sample**
```
Input          Output
6              3
500.75
-200.50
300
-50.25
-10
400
```

## Q44. Mess Bill Cap
**Problem.** A hostel mess charges ₹42.50 per meal but caps the monthly bill at ₹3000.
**Task.** Read the days `N`, then each day's meal count; print the month's bill (capped).
**Input Format**
Line 1: integer `N`  (1 ≤ N ≤ 31)
Next `N` lines: one meal count each  (0 ≤ meals ≤ 5)
**Output Format.** A single number with exactly two decimal places — the bill.
**Sample**
```
Input          Output
5              552.50
3
2
3
3
2
```

## Q45. Stamp Ledger
**Problem.** A collector starts with some stamps; each trade adds or removes some (positive or negative), and a 0 ends the ledger.
**Task.** Read the starting count, then trades one per line until 0; print the final stamp count.
**Input Format**
Line 1: integer starting count  (0 ≤ start ≤ 10⁴)
Following lines: one integer per trade, ending with 0
**Output Format.** A single integer — the final count.
**Sample**
```
Input          Output
40             38
5
-12
8
-3
0
```

## Q46. Hoopla Stall
**Problem.** At a hoopla stall you throw until you miss (a 0). Each throw's landed rings are recorded, and every ring is worth 15 points.
**Task.** Keep reading rings-landed per throw until 0; print the total points.
**Input Format**
One integer per line, ending with 0  (0 ≤ rings ≤ 10)
**Output Format.** A single integer — the points.
**Sample**
```
Input          Output
2              150
3
1
4
0
```

---

*End of Batch 4 (revised) — 46 questions; every sample output generated by a verified reference solution, with all two-decimal outputs produced by `print(f"{ans:.2f}")`.*
