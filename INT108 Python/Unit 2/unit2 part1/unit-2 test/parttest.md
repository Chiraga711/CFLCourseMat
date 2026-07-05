code problems
Python Conditionals — 50 Coding Questions
A scenario-based question bank combining maths/formulas with `if-elif` and nested conditionals
Instructions for students
Solve each problem by reading the inputs, doing the calculation, and printing the result described.
Read decimal values with `float(input(...))` and whole numbers with `int(input(...))`.
Currency is shown as ₹; you only need to print the numbers.
Each problem needs a calculation combined with a decision (`if-elif` and/or nested `if`s). The scenario gives you the rules — translate them into code.
The problems get harder as you go: Section A is single-level decisions, Section B adds multi-step calculations, and Section C is nested logic.
---
Section A — Formula + `if-elif` (Q1–Q20)
1. Taxi Fare.
A taxi charges a base fare of ₹50.00 plus ₹12.00 per kilometre. A time-of-day surcharge is added to the fare: night adds 30%, evening adds 15%, day adds nothing.
Task: Read the distance in km and the time of day (`day`/`evening`/`night`). Calculate and print the final fare.
2. Fuel Trip Cost.
The fuel needed for a trip is the distance divided by the car's mileage (km per litre), and the cost is that many litres times the price per litre. Then label the trip: cost ≤ ₹500 → `Cheap`, ≤ ₹1500 → `Moderate`, otherwise → `Expensive`.
Task: Read the distance, the mileage, and the price per litre. Print the cost and the label.
3. Electricity Bill.
Electricity is billed per unit, and the rate depends on usage: up to 100 units → ₹5 per unit, up to 300 units → ₹7 per unit, above 300 → ₹10 per unit. The bill is units × rate.
Task: Read the number of units used. Calculate and print the bill.
4. Parking Fee.
A car park charges by time: up to 1 hour → ₹30, up to 3 hours → ₹60, up to 6 hours → ₹100, more than 6 hours → ₹150.
Task: Read the number of hours parked. Print the fee.
5. Movie Ticket.
A cinema's base price depends on the show: matinee → ₹100, evening → ₹150, night → ₹200. Children under 12 pay half price.
Task: Read the show type (`matinee`/`evening`/`night`) and the viewer's age. Calculate and print the ticket price.
6. BMI Calculator.
Body Mass Index is weight divided by height squared (height in metres). The category is: below 18.5 → `Underweight`, below 25 → `Normal`, below 30 → `Overweight`, otherwise → `Obese`.
Task: Read the weight (kg) and height (m). Print the BMI and the category.
7. Exam Division.
A student's percentage is their marks divided by the total, times 100. The division is: 60% or above → `First`, 45% or above → `Second`, 33% or above → `Third`, below 33% → `Fail`.
Task: Read the marks scored and the total marks. Print the percentage and the division.
8. Water Bill.
Water usage is billed as: up to 10 units → free, up to 25 units → ₹3 per unit, above 25 → ₹5 per unit.
Task: Read the number of units used. Calculate and print the bill.
9. Currency Exchange.
US dollars convert to rupees at ₹83 per dollar. A service fee is then subtracted: up to $100 → ₹200, up to $1000 → ₹500, above $1000 → ₹1000.
Task: Read the amount in dollars. Calculate and print the net amount in rupees after the fee.
10. Weekly Wage.
A worker is paid their hourly rate for up to 40 hours. Any hours beyond 40 are paid at 1.5 times the rate.
Task: Read the hours worked and the hourly rate. Calculate and print the total pay.
11. Pizza Order.
A pizza's base price depends on size: small → ₹150, medium → ₹250, large → ₹350. Each topping costs ₹30 extra.
Task: Read the size and the number of toppings. Calculate and print the total price.
12. Internet Plan.
A provider recommends a plan from the monthly data need: up to 50 GB → `Basic` (₹300), up to 200 GB → `Standard` (₹600), above 200 GB → `Premium` (₹1000).
Task: Read the data need in GB. Print the plan name and its cost.
13. Pet Food Portion.
A dog's daily food portion in grams is its weight (kg) times 25. The size group is: below 5 kg → `Small`, below 20 kg → `Medium`, otherwise → `Large`.
Task: Read the dog's weight in kg. Print the portion in grams and the size group.
14. Temperature Converter.
Celsius converts to Fahrenheit with `C × 9 / 5 + 32`. Then give advice: below 0 → `Freezing`, below 15 → `Cold`, below 30 → `Pleasant`, otherwise → `Hot`.
Task: Read a temperature in Celsius. Print the Fahrenheit value and the advice.
15. Step Tracker.
A fitness band estimates calories burned as steps × 0.04. The status is: 10000 or more → `Goal met`, 5000 or more → `Almost there`, otherwise → `Keep going`.
Task: Read the number of steps. Print the calories burned and the status.
16. Net Salary.
From a gross monthly salary, 12% is deducted as Provident Fund. The remaining (taxable) amount is taxed: up to ₹20000 → no tax, up to ₹50000 → 10% of taxable, above ₹50000 → 20%. Net salary is gross minus PF minus tax.
Task: Read the gross salary. Calculate and print the net salary.
17. Simple Interest.
The interest rate depends on the principal: up to ₹10000 → 5%, up to ₹50000 → 7%, above ₹50000 → 9%. Simple interest is `principal × rate × time / 100`.
Task: Read the principal and the time in years. Calculate and print the interest.
18. Insurance Premium.
The base premium depends on age: below 25 → ₹5000, below 40 → ₹7000, below 60 → ₹10000, otherwise → ₹15000. Smokers pay 50% more.
Task: Read the age and whether the person smokes (`yes`/`no`). Calculate and print the premium.
19. Required Run Rate.
In cricket, the required run rate is the runs needed divided by the overs remaining. Describe the chase: rate ≤ 6 → `Comfortable`, ≤ 10 → `Challenging`, ≤ 15 → `Difficult`, otherwise → `Nearly impossible`.
Task: Read the runs needed and the overs remaining. Print the run rate and the description.
20. Card Reward Points.
A credit card awards points as a percentage of the amount spent: up to ₹1000 → 1%, up to ₹5000 → 2%, above ₹5000 → 3%. Points = `spend × rate / 100`.
Task: Read the amount spent. Calculate and print the points earned.
---
Section B — Multi-step Calculations + Conditionals (Q21–Q35)
21. Hotel Bill.
The room cost is nights × rate per night. A seasonal surcharge is added to that cost: peak → 30%, festival → 50%, normal → none. Then 12% tax is added on top. The total is cost + surcharge + tax.
Task: Read the number of nights, the rate per night, and the season. Calculate and print the total.
22. Courier Charge.
A courier costs ₹40.00 plus ₹15.00 per kilogram. Delivery speed adds a fee: express → ₹100, standard → ₹50, economy → nothing. Finally, if the charge is more than ₹500, a 10% discount is applied to the whole charge.
Task: Read the package weight (kg) and the delivery speed. Calculate and print the final charge.
23. Car Rental.
A car rents for ₹1500 per day. Insurance adds a per-day amount: basic → ₹0, standard → ₹200, premium → ₹500.
Task: Read the number of days and the insurance type. Calculate and print the total cost.
24. Excess Baggage.
The first 15 kg of luggage is free. For each kilogram above 15, the rate depends on the class: economy → ₹500, business → ₹300, first → ₹0.
Task: Read the luggage weight (kg) and the travel class. Calculate and print the excess-baggage fee.
25. Loan EMI.
The total repayable is the principal plus one year of simple interest at the given rate. The monthly EMI is the total divided by the number of months. Then label it: EMI above ₹20000 → `High`, above ₹10000 → `Moderate`, otherwise → `Affordable`.
Task: Read the principal, the interest rate (%), and the number of months. Print the EMI and the label.
26. GPA Result.
A GPA maps to a class: 9 or above → `Outstanding`, 7.5 or above → `Distinction`, 6 or above → `First`, 5 or above → `Pass`, otherwise → `Fail`. Separately, a student with GPA 8 or above and family income below ₹200000 is scholarship-eligible.
Task: Read the GPA and the family income. Print the class and whether the student gets a scholarship.
27. Daily Calorie Needs.
A person's base metabolic rate is weight (kg) × 24. An activity multiplier is applied: sedentary → 1.2, moderate → 1.5, active → 1.8. Needs = BMR × multiplier.
Task: Read the weight and the activity level. Calculate and print the daily calorie needs.
28. Heart-Rate Zone.
Maximum heart rate is `220 − age`. The current heart rate as a percentage of the maximum gives the zone: below 50% → `Resting`, below 70% → `Fat burn`, below 85% → `Cardio`, otherwise → `Peak`.
Task: Read the age and the current heart rate. Print the percentage and the zone.
29. Water Intake.
The recommended daily water in litres is weight (kg) × 0.033. The need level is: below 50 kg → `Low`, below 80 kg → `Normal`, otherwise → `High`.
Task: Read the weight. Print the recommended litres and the need level.
30. Loyalty Discount.
A flat discount is given based on loyalty points: up to 100 → ₹0, up to 500 → ₹50, up to 1000 → ₹100, above 1000 → ₹200. The final amount is the bill minus the discount.
Task: Read the loyalty points and the bill amount. Calculate and print the final amount.
31. Surge Pricing.
A ride's fare is the base fare times a demand multiplier: low → 1.0, medium → 1.5, high → 2.0.
Task: Read the demand level and the base fare. Calculate and print the fare.
32. Gas Cylinder Delivery.
A cylinder costs ₹1000, plus a delivery fee by distance: up to 5 km → ₹0, up to 15 km → ₹50, above 15 km → ₹100.
Task: Read the delivery distance in km. Calculate and print the total cost.
33. Bulk Purchase.
The per-unit price falls with quantity: fewer than 10 → ₹100, fewer than 50 → ₹90, fewer than 100 → ₹80, otherwise → ₹70. The total is quantity × unit price.
Task: Read the quantity. Calculate and print the total cost.
34. Subscription Cost.
A plan's base monthly price is: basic → ₹200, standard → ₹400, premium → ₹800. With annual billing you pay for 12 months but get 20% off; with monthly billing you pay the base price.
Task: Read the tier and the billing type (`monthly`/`annual`). Calculate and print the cost.
35. Traffic Fine.
The base fine depends on the violation: speeding → ₹1000, signal jump → ₹500, parking → ₹300. A repeat offender pays 50% more.
Task: Read the violation type and whether the driver is a repeat offender (`yes`/`no`). Calculate and print the fine.
---
Section C — Nested Conditionals + Calculations (Q36–Q50)
36. Scholarship Award.
The course fee is ₹100000. Only students scoring 60 or more qualify for a scholarship; for them, the waiver depends on family income: below ₹150000 → 50% of the fee, below ₹300000 → 25%, otherwise → nothing. Students scoring below 60 get no scholarship.
Task: Read the marks and the family income. Calculate and print the scholarship amount.
37. Personal Loan.
An applicant must earn at least ₹30000 a month to be eligible. If eligible, the interest rate depends on their credit score: 750 or above → 8%, 650 or above → 12%, otherwise → 18%. The total repayable is the loan amount plus one year's interest, and the EMI is that total divided by 12. If not eligible, report it instead.
Task: Read the monthly salary, the loan amount, and the credit score. Print the EMI, or `Not eligible`.
38. Amusement Park Ticket.
Children under 5 enter free. Ages 5 to 17 pay ₹300. For adults (18 and over), seniors aged 60 or more pay ₹200, while other adults pay ₹500.
Task: Read the visitor's age. Calculate and print the ticket price.
39. Swimming Pool Fee.
Members pay ₹50 at peak times and ₹30 off-peak. Non-members pay ₹100 at peak times and ₹70 off-peak.
Task: Read whether the visitor is a member (`yes`/`no`) and the time (`peak`/`off-peak`). Print the fee.
40. Room Allocation.
A room is allocated only if the booking is confirmed. For confirmed bookings, the room depends on loyalty tier: gold → `Suite`, silver → `Deluxe`, none → `Standard`. If the booking isn't confirmed, report `Booking not confirmed`.
Task: Read whether the booking is confirmed (`yes`/`no`) and the loyalty tier. Print the room type or the message.
41. Tax — Two Regimes.
Under the old regime: up to ₹250000 → 0%, up to ₹500000 → 5%, above → 20%. Under the new regime: up to ₹300000 → 0%, up to ₹600000 → 10%, above → 15%. Each rate applies to the whole income (a simplified model).
Task: Read the regime (`old`/`new`) and the income. Calculate and print the tax.
42. Grace Marks.
The pass mark is 40. A student scoring 40 or more passes. A student scoring below 40 but within 3 marks of passing (that is, 37 to 39) passes with grace marks; anyone lower fails.
Task: Read the marks. Print `Pass`, `Pass with grace marks`, or `Fail`.
43. Salary Appraisal.
Only employees rated 4 or 5 receive a hike: a rating of 5 gives a 20% raise, a rating of 4 gives 10%. The new salary is the current salary plus the raise. Anyone rated below 4 keeps their current salary.
Task: Read the performance rating and the current salary. Calculate and print the new salary.
44. Shipping & Customs.
An international shipment adds customs duty based on its value: up to ₹5000 → 5%, up to ₹20000 → 10%, above → 20%; the total is value + duty. A domestic shipment simply adds a flat ₹50.
Task: Read the shipment type (`international`/`domestic`) and the value. Calculate and print the total.
45. Event Ticket.
For VIP tickets, early-bird buyers pay ₹4000 and others ₹5000. For non-VIP tickets, early-bird buyers pay ₹1500 and others ₹2000.
Task: Read whether the ticket is VIP (`yes`/`no`) and whether it's an early-bird purchase (`yes`/`no`). Print the price.
46. Ride Cancellation.
If a ride is cancelled, a fee applies based on how many minutes before pickup it was cancelled: under 5 minutes → ₹100, under 15 minutes → ₹50, otherwise → ₹0. If the ride isn't cancelled, print `Enjoy your ride!`.
Task: Read whether the ride was cancelled (`yes`/`no`) and the minutes before pickup. Print the cancellation fee or the message.
47. Medical Bill.
An insured patient's coverage depends on their plan: basic → 60%, standard → 80%, premium → 100%; the patient pays whatever isn't covered. An uninsured patient pays the full bill.
Task: Read whether the patient is insured (`yes`/`no`), the plan, and the bill amount. Calculate and print what the patient pays.
48. Flight Fare.
The base fare depends on class: economy → ₹5000, business → ₹15000. If fewer than 10 seats remain, a 20% surge is added to the fare.
Task: Read the class and the number of seats remaining. Calculate and print the fare.
49. Tenure Bonus.
Only employees with at least 5 years of service get a bonus, calculated from their salary: under 10 years → 10%, under 20 years → 15%, otherwise → 20%. Employees with fewer than 5 years get no bonus.
Task: Read the years of service and the salary. Calculate and print the bonus.
50. Bookstore Checkout (capstone).
The subtotal is quantity × price per book. Members get a discount based on the subtotal: below ₹1000 → 5%, below ₹5000 → 10%, otherwise → 15%. Non-members get: below ₹5000 → 0%, otherwise → 5%. Apply the discount, and then — if the amount is still below ₹500 — add ₹50 for shipping.
Task: Read the quantity, the price per book, and whether the customer is a member (`yes`/`no`). Calculate and print the final total.
---


MCQ problems
Q26. What will be the output of the following code?
marks = 82

if marks >= 60:
    print("C Grade")
elif marks >= 75:
    print("B Grade")
elif marks >= 90:
    print("A Grade")
else:
    print("Fail")

A) C Grade
B) B Grade
C) A Grade
D) Fail
Correct Answer: A
Verified: Yes — the first true condition marks >= 60 executes, and later elif blocks are skipped.
Explanation:
Step 1: 82 >= 60 is true.
Step 2: Python enters the first if block immediately.
Final: It prints C Grade.
Common Mistake: Thinking Python will choose the “best matching” grade instead of the first true condition.
Quick Check: Why should grade conditions usually be written from highest to lowest?

Q27. What will be the output of the following code?
temperature = 30

if temperature > 30:
    print("Hot")
if temperature >= 30:
    print("Warm")
else:
    print("Cool")

A) Hot
B) Warm
C) Cool
D) Hot Warm
Correct Answer: B
Verified: Yes — the first if is false, the second if is true, so only Warm prints.
Explanation:
Step 1: temperature > 30 is false.
Step 2: temperature >= 30 is true.
Final: Python prints Warm.
Common Mistake: Thinking the else belongs to the first if; it belongs to the second if.
Quick Check: Which if is connected with the else here?

Q28. What will be the output of the following code?
num = 0

if num >= 0:
    if num > 0:
        print("Positive")
    else:
        print("Zero")
else:
    print("Negative")

A) Positive
B) Negative
C) Zero
D) No output
Correct Answer: C
Verified: Yes — num >= 0 is true, but num > 0 is false.
Explanation:
Step 1: 0 >= 0 is true, so Python enters the outer if.
Step 2: 0 > 0 is false, so the inner else executes.
Final: It prints Zero.
Common Mistake: Treating zero as positive.
Quick Check: Is 0 > 0 true or false?

Q29. What will be the output of the following code?
age = 17

if not age >= 18:
    print("Minor")
else:
    print("Adult")

A) Adult
B) 17
C) No output
D) Minor
Correct Answer: D
Verified: Yes — age >= 18 is false, and not False becomes true.
Explanation:
Step 1: 17 >= 18 is false.
Step 2: not False becomes true.
Final: Python prints Minor.
Common Mistake: Ignoring the effect of not before the condition.
Quick Check: What is the result of not True?

Q30. What will be the output of the following code?
has_fees_due = True

if has_fees_due == False:
    print("Admit Card Allowed")
else:
    print("Admit Card Hold")

A) Admit Card Hold
B) Admit Card Allowed
C) True
D) False
Correct Answer: A
Verified: Yes — True == False is false, so the else block executes.
Explanation:
Step 1: has_fees_due is True.
Step 2: The condition checks whether it is equal to False.
Final: Since the condition is false, Admit Card Hold is printed.
Common Mistake: Reading the variable name but not checking the actual condition.
Quick Check: What will happen if has_fees_due = False?

Q31. What will be the output of the following code?
score = 75

if 60 <= score < 75:
    print("Grade C")
elif 75 <= score < 90:
    print("Grade B")
else:
    print("Other Grade")

A) Grade C
B) Grade B
C) Other Grade
D) No output
Correct Answer: B
Verified: Yes — 75 <= score < 90 is true when score is 75.
Explanation:
Step 1: 60 <= 75 < 75 is false because 75 < 75 is false.
Step 2: 75 <= 75 < 90 is true.
Final: Python prints Grade B.
Common Mistake: Forgetting that < 75 does not include 75.
Quick Check: Which range includes exactly 75?

Q32. What will happen when this code is executed?
x = 3

if x > 5:
    print("A")
print("B")
else:
    print("C")

A) A B
B) B C
C) Syntax error
D) C only
Correct Answer: C
Verified: Yes — the else has no matching if at the same indentation level.
Explanation:
Step 1: The line print("B") ends the if block.
Step 2: After that, else appears without a matching if.
Final: Python gives a syntax error.
Common Mistake: Thinking else can appear after any statement.
Quick Check: Must else directly match an if at the same indentation level?

Q33. What will be the output of the following code?
balance = 1000

if balance >= 500:
    print("Basic")
if balance >= 1000:
    print("Premium")
if balance > 2000:
    print("Gold")
else:
    print("Standard")

A) Premium Standard
B) Basic Gold
C) Basic Premium
D) Basic Premium Standard
Correct Answer: D
Verified: Yes — first two independent if conditions are true, and the third if is false, so its else runs.
Explanation:
Step 1: balance >= 500 is true, so Basic prints.
Step 2: balance >= 1000 is true, so Premium prints.
Step 3: balance > 2000 is false, so the last else prints Standard.
Final: Output is Basic Premium Standard.
Common Mistake: Thinking the final else belongs to all previous if statements.
Quick Check: Which if is connected to the final else?

Q34. Which condition correctly checks whether x is outside the range 10 to 20 inclusive?
x = 25

if ______:
    print("Outside Range")
else:
    print("Inside Range")

A) x < 10 or x > 20
B) x >= 10 and x <= 20
C) x > 10 and x < 20
D) x == 10 or x == 20
Correct Answer: A
Verified: Yes — outside the inclusive range means less than 10 or greater than 20.
Explanation:
Step 1: Inside range means 10 <= x <= 20.
Step 2: Outside means x < 10 or x > 20.
Final: The correct condition is x < 10 or x > 20.
Common Mistake: Using and for outside range, which cannot work here.
Quick Check: Is 25 inside or outside 10 to 20?

Q35. What will be the output of the following code?
age = 16
accompanied_by_adult = True

if age >= 18 or accompanied_by_adult:
    print("Entry Allowed")
else:
    print("Entry Denied")

A) Entry Denied
B) Entry Allowed
C) True
D) 16
Correct Answer: B
Verified: Yes — one part of the or condition is true.
Explanation:
Step 1: age >= 18 is false.
Step 2: accompanied_by_adult is true.
Final: Since or needs only one true condition, Entry Allowed is printed.
Common Mistake: Treating or like and.
Quick Check: With or, how many conditions must be true?

Q36. What will be the output of the following code?
speed = 60

if speed > 60:
    print("Over Speed")
elif speed == 60:
    print("At Limit")
else:
    print("Below Limit")

A) Over Speed
B) Below Limit
C) At Limit
D) 60
Correct Answer: C
Verified: Yes — speed == 60 is true.
Explanation:
Step 1: speed > 60 is false.
Step 2: speed == 60 is true.
Final: Python prints At Limit.
Common Mistake: Thinking 60 is over the limit when condition is strictly > 60.
Quick Check: What condition would include 60 as over speed?

Q37. What will be the output of the following code?
status = "blocked"

if status == "active" or "pending":
    print("Allowed")
else:
    print("Denied")

A) Denied
B) blocked
C) No output
D) Allowed
Correct Answer: D
Verified: Yes — "pending" is a non-empty string, so it behaves as true.
Explanation:
Step 1: status == "active" is false.
Step 2: "pending" is a non-empty string, so it is treated as true.
Final: False or True becomes true, so Allowed is printed.
Common Mistake: Writing status == "active" or "pending" instead of comparing status both times.
Quick Check: What is the better condition: status == "active" or status == "pending"?

Q38. What is the error in the following code?
x = 10

if x > 5
    print("Greater")
else:
    print("Smaller")

A) Missing colon after if x > 5
B) else cannot be used with if
C) print() is written incorrectly
D) x > 5 is not a valid condition
Correct Answer: A
Verified: Yes — Python requires a colon : after an if condition.
Explanation:
Step 1: The if statement must end with :.
Step 2: Here, the colon is missing after if x > 5.
Final: Python gives a syntax error.
Common Mistake: Forgetting the colon after if, elif, or else.
Quick Check: Does else also need a colon?

Q39. What will be the output of the following code?
has_card = False
cash = 50

if not has_card and cash >= 100:
    print("Can Buy")
else:
    print("Cannot Buy")

A) Can Buy
B) Cannot Buy
C) False
D) 50
Correct Answer: B
Verified: Yes — not has_card is true, but cash >= 100 is false.
Explanation:
Step 1: has_card is false, so not has_card becomes true.
Step 2: cash >= 100 means 50 >= 100, which is false.
Final: True and False becomes false, so Cannot Buy is printed.
Common Mistake: Stopping after the first true part of an and condition.
Quick Check: For and, what happens if one condition is false?

Q40. What will be the output of the following code?
marks = 88
income = 300000

if marks >= 85:
    if income <= 250000:
        print("Full Scholarship")
    else:
        print("Partial Scholarship")
else:
    print("No Scholarship")

A) Full Scholarship
B) No Scholarship
C) Partial Scholarship
D) 300000
Correct Answer: C
Verified: Yes — marks condition is true, but income condition is false.
Explanation:
Step 1: marks >= 85 is true.
Step 2: income <= 250000 is false because income is 300000.
Final: The inner else prints Partial Scholarship.
Common Mistake: Checking only marks and ignoring the nested income condition.
Quick Check: What will print if income is 200000?

Q41. What will be the output of the following code?
password = "abc123"

if password != "admin":
    print("User Password")
else:
    print("Default Password")

A) Default Password
B) admin
C) abc123
D) User Password
Correct Answer: D
Verified: Yes — "abc123" != "admin" is true.
Explanation:
Step 1: The condition checks whether password is not equal to "admin".
Step 2: "abc123" is different from "admin".
Final: Python prints User Password.
Common Mistake: Reading != as equal to.
Quick Check: What does != mean in Python?

Q42. What will be the output of the following code?
n = 15

if n % 5 == 0:
    print("Divisible by 5")
elif n % 3 == 0:
    print("Divisible by 3")
elif n % 15 == 0:
    print("Divisible by 15")
else:
    print("Not Divisible")

A) Divisible by 5
B) Divisible by 3
C) Divisible by 15
D) Not Divisible
Correct Answer: A
Verified: Yes — the first condition is true, so later elif blocks are skipped.
Explanation:
Step 1: 15 % 5 == 0 is true.
Step 2: Python executes the first true block.
Final: It prints Divisible by 5.
Common Mistake: Expecting Divisible by 15 because it is mathematically more specific.
Quick Check: Should the most specific condition usually come first?

Q43. What will be the output of the following code?
num = -8

if num < 0 and num % 2 == 0:
    print("Negative Even")
elif num < 0 and num % 2 != 0:
    print("Negative Odd")
else:
    print("Non-negative")

A) Negative Odd
B) Negative Even
C) Non-negative
D) Even
Correct Answer: B
Verified: Yes — -8 < 0 is true and -8 % 2 == 0 is also true.
Explanation:
Step 1: num < 0 checks whether the number is negative.
Step 2: num % 2 == 0 checks whether it is even.
Final: Both are true, so Negative Even is printed.
Common Mistake: Thinking negative numbers cannot be even.
Quick Check: Is -6 even or odd?

Q44. Which condition correctly checks whether marks are invalid if they are below 0 or above 100?
marks = 105

if ______:
    print("Invalid Marks")
else:
    print("Valid Marks")

A) marks >= 0 and marks <= 100
B) marks > 0 and marks < 100
C) marks < 0 or marks > 100
D) marks == 0 or marks == 100
Correct Answer: C
Verified: Yes — invalid marks are outside the valid range 0 to 100.
Explanation:
Step 1: Valid marks are from 0 to 100.
Step 2: Invalid marks are less than 0 or greater than 100.
Final: The correct condition is marks < 0 or marks > 100.
Common Mistake: Writing the condition for valid marks when the question asks invalid marks.
Quick Check: Is 100 valid or invalid?

Q45. What will be the output of the following code?
x = 2

if x > 5:
    print("Greater")
else:
    print("Not Greater")

print("Done")

A) Greater
B) Done
C) Greater Done
D) Not Greater Done
Correct Answer: D
Verified: Yes — the else block runs, and print("Done") runs after the conditional.
Explanation:
Step 1: 2 > 5 is false.
Step 2: The else block prints Not Greater.
Step 3: print("Done") is outside the conditional, so it always runs.
Final: Output is Not Greater followed by Done.
Common Mistake: Thinking Done is part of the else block.
Quick Check: How can you identify whether a line is inside or outside an if-else block?

Q46. What will be the output of the following code?
marks = 39
passed = marks >= 40

if passed:
    print("Pass")
else:
    print("Fail")

A) Fail
B) Pass
C) True
D) 39
Correct Answer: A
Verified: Yes — marks >= 40 becomes false, so passed stores False.
Explanation:
Step 1: 39 >= 40 is false.
Step 2: Therefore, passed becomes False.
Final: The else block executes and prints Fail.
Common Mistake: Thinking passed is automatically true because of its name.
Quick Check: What value will passed store if marks = 40?

Q47. Which condition correctly checks whether a person is eligible only if age is at least 18 and citizenship is confirmed?
age = 20
is_citizen = True

if ______:
    print("Eligible")
else:
    print("Not Eligible")

A) age >= 18 or is_citizen
B) age >= 18 and is_citizen
C) age < 18 and is_citizen
D) age >= 18 and not is_citizen
Correct Answer: B
Verified: Yes — the word “only if” requires both conditions to be true.
Explanation:
Step 1: Age must be at least 18.
Step 2: Citizenship must also be confirmed.
Final: Both conditions are required, so use and.
Common Mistake: Using or, which allows eligibility even if only one condition is true.
Quick Check: Should a 20-year-old non-citizen be eligible?

Q48. What will happen when this code is executed?
x = 10

if x > 10:
    print("Greater")
else:
    print("Not Greater")
elif x == 10:
    print("Equal")

A) Equal
B) Not Greater
C) Syntax error
D) Greater
Correct Answer: C
Verified: Yes — elif cannot appear after else.
Explanation:
Step 1: In Python, the order must be if, then optional elif, then optional else.
Step 2: Here, else appears before elif.
Final: Python gives a syntax error.
Common Mistake: Placing elif after else.
Quick Check: Which comes first: elif or else?

Q49. What will be the output of the following code?
amount = 700
is_member = False

if amount >= 500:
    if is_member:
        print("Extra Discount")
    else:
        print("Normal Discount")
else:
    print("No Discount")

A) Extra Discount
B) No Discount
C) 700
D) Normal Discount
Correct Answer: D
Verified: Yes — amount condition is true, but is_member is false.
Explanation:
Step 1: amount >= 500 is true, so Python enters the outer if.
Step 2: is_member is false, so the inner else runs.
Final: It prints Normal Discount.
Common Mistake: Assuming every purchase above 500 gets extra discount.
Quick Check: What will print if is_member = True?

Q50. What will be the output of the following code?
rating = 3

if rating == 5:
    print("Excellent")
elif rating != 1:
    print("Valid Rating")
else:
    print("Poor")

A) Valid Rating
B) Excellent
C) Poor
D) No output
Correct Answer: A
Verified: Yes — rating == 5 is false, but rating != 1 is true.
Explanation:
Step 1: rating == 5 is false because rating is 3.
Step 2: rating != 1 is true because 3 is not equal to 1.
Final: Python prints Valid Rating.
Common Mistake: Thinking elif rating != 1 only checks high ratings.
Quick Check: What will print if rating = 1?
Q51. What will be the output of the following code?
marks = 82
attendance = 74

if marks >= 80:
    if attendance >= 75:
        print("Honors")
    else:
        print("Merit")
else:
    print("Regular")

A) Honors
B) Merit
C) Regular
D) Attendance Short
Correct Answer: B
Verified: Yes — marks >= 80 is true, but attendance >= 75 is false.
Explanation:
Step 1: 82 >= 80 is true, so Python enters the outer if.
Step 2: 74 >= 75 is false, so the inner else runs.
Final: Merit is printed.
Common Mistake: Checking only marks and ignoring attendance.
Quick Check: What will print if attendance is 75?

Q52. What will be the output of the following code?
temperature = 29
humidity = 80

if temperature >= 30:
    if humidity > 70:
        print("Hot and Humid")
    else:
        print("Hot")
else:
    if humidity > 75:
        print("Humid Day")
    else:
        print("Pleasant")

A) Humid Day
B) Hot and Humid
C) Hot
D) Pleasant
Correct Answer: A
Verified: Yes — temperature condition is false, but humidity condition inside else is true.
Explanation:
Step 1: 29 >= 30 is false, so Python goes to the outer else.
Step 2: 80 > 75 is true.
Final: Humid Day is printed.
Common Mistake: Assuming humidity is checked only when temperature is high.
Quick Check: What will print if temperature is 31 and humidity is 80?

Q53. What will be the output of the following code?
x = 8
y = 3
z = 5

if x > y:
    if y + z == x:
        print("Balanced")
    else:
        print("Unbalanced")
else:
    print("Invalid")

A) Invalid
B) Unbalanced
C) Balanced
D) x is Greater
Correct Answer: C
Verified: Yes — x > y is true and 3 + 5 == 8 is also true.
Explanation:
Step 1: 8 > 3 is true.
Step 2: y + z == x becomes 3 + 5 == 8, which is true.
Final: Balanced is printed.
Common Mistake: Forgetting to evaluate the arithmetic expression before comparison.
Quick Check: What is the value of y + z here?

Q54. What will be the output of the following code?
age = 19
score = 68

if age >= 18:
    if score >= 70 and score <= 100:
        print("Eligible")
    else:
        print("Need Higher Score")
else:
    print("Too Young")

A) Eligible
B) Too Young
C) Invalid Score
D) Need Higher Score
Correct Answer: D
Verified: Yes — age condition is true, but score condition is false.
Explanation:
Step 1: 19 >= 18 is true.
Step 2: score >= 70 and score <= 100 becomes 68 >= 70 and 68 <= 100.
Final: Since one part of and is false, Need Higher Score is printed.
Common Mistake: Thinking score <= 100 alone is enough for eligibility.
Quick Check: For and, what happens if one condition is false?

Q55. Which condition should replace the blank to check whether the student qualifies for scholarship inside the income condition?
marks = 88
attendance = 78
family_income = 250000

if family_income <= 300000:
    if ______:
        print("Scholarship Approved")
    else:
        print("Academic Criteria Not Met")
else:
    print("Income Criteria Not Met")

Rule: Scholarship is approved only if marks are at least 85 and attendance is at least 75.
A) marks >= 85 and attendance >= 75
B) marks >= 85 or attendance >= 75
C) marks > 85 and attendance > 75
D) marks <= 85 and attendance <= 75
Correct Answer: A
Verified: Yes — both minimum conditions must be true and equality is included.
Explanation:
Step 1: Marks must be at least 85, so use marks >= 85.
Step 2: Attendance must be at least 75, so use attendance >= 75.
Final: Since both are required, use and.
Common Mistake: Using or, which approves scholarship even if only one condition is satisfied.
Quick Check: Should marks 85 and attendance 75 qualify?

Q56. What will be the output of the following code?
x = 4
y = 9

if x > 5:
    if y > 5:
        print("A")
    else:
        print("B")
else:
    print("C")

A) A
B) C
C) B
D) A B
Correct Answer: B
Verified: Yes — the outer condition x > 5 is false, so the outer else executes.
Explanation:
Step 1: 4 > 5 is false.
Step 2: Python does not check the inner if.
Final: The outer else prints C.
Common Mistake: Checking y > 5 even though the outer condition failed.
Quick Check: Will the inner if run if the outer if is false?

Q57. What will be the output of the following code?
num = 10

if 5 < num <= 10:
    if num == 10:
        print("Upper Boundary")
    else:
        print("Inside Range")
else:
    print("Outside Range")

A) Inside Range
B) Outside Range
C) Lower Boundary
D) Upper Boundary
Correct Answer: D
Verified: Yes — 5 < 10 <= 10 is true and num == 10 is also true.
Explanation:
Step 1: 5 < num <= 10 checks whether num is greater than 5 and at most 10.
Step 2: Since num is exactly 10, the inner if is true.
Final: Upper Boundary is printed.
Common Mistake: Thinking <= 10 excludes 10.
Quick Check: Does <= include equality?

Q58. What will be the output of the following code?
is_registered = True
fee_paid = False

if is_registered:
    if not fee_paid:
        print("Payment Pending")
    else:
        print("Access Granted")
else:
    print("Register First")

A) Access Granted
B) Payment Pending
C) Register First
D) Fee Paid
Correct Answer: B
Verified: Yes — is_registered is true and not fee_paid becomes true.
Explanation:
Step 1: is_registered is True, so Python enters the outer if.
Step 2: fee_paid is False, so not fee_paid is True.
Final: Payment Pending is printed.
Common Mistake: Forgetting that not False becomes True.
Quick Check: What is the value of not fee_paid here?

Q59. What will be the output of the following code?
a = 12
b = 4

if a % b == 0:
    if a // b == 3:
        print("Exact Triple")
    else:
        print("Divisible")
else:
    print("Not Divisible")

A) Exact Triple
B) Divisible
C) Not Divisible
D) Remainder Zero
Correct Answer: A
Verified: Yes — 12 % 4 == 0 and 12 // 4 == 3 are both true.
Explanation:
Step 1: 12 % 4 gives remainder 0, so the outer condition is true.
Step 2: 12 // 4 gives 3, so the inner condition is true.
Final: Exact Triple is printed.
Common Mistake: Confusing % remainder with // integer division.
Quick Check: What is 12 // 4?

Q60. What will be the output of the following code?
units = 120

if units <= 100:
    print("Low Usage")
else:
    if units <= 200:
        print("Medium Usage")
    else:
        print("High Usage")

A) Low Usage
B) High Usage
C) Medium Usage
D) Invalid Usage
Correct Answer: C
Verified: Yes — units <= 100 is false, but units <= 200 is true.
Explanation:
Step 1: 120 <= 100 is false.
Step 2: Python enters the outer else.
Step 3: 120 <= 200 is true.
Final: Medium Usage is printed.
Common Mistake: Thinking every value greater than 100 is high usage.
Quick Check: Which category should 200 belong to?

Q61. What will be the output of the following code?
pin_correct = True
balance = 400

if pin_correct:
    if balance >= 500:
        print("Withdraw Allowed")
    else:
        print("Low Balance")
else:
    print("Wrong PIN")

A) Low Balance
B) Withdraw Allowed
C) Wrong PIN
D) PIN Correct
Correct Answer: A
Verified: Yes — PIN is correct, but balance is less than 500.
Explanation:
Step 1: pin_correct is True, so Python enters the outer if.
Step 2: balance >= 500 means 400 >= 500, which is false.
Final: The inner else prints Low Balance.
Common Mistake: Assuming correct PIN is enough for withdrawal.
Quick Check: What balance is needed for withdrawal here?

Q62. What will be the output of the following code?
n = 45

if n % 3 == 0:
    if n % 5 == 0:
        print("Divisible by 3 and 5")
    else:
        print("Divisible by 3 only")
else:
    print("Not Divisible by 3")

A) Divisible by 3 only
B) Not Divisible by 3
C) Divisible by 3 and 5
D) Divisible by 5 only
Correct Answer: C
Verified: Yes — 45 is divisible by both 3 and 5.
Explanation:
Step 1: 45 % 3 == 0 is true.
Step 2: 45 % 5 == 0 is also true.
Final: Divisible by 3 and 5 is printed.
Common Mistake: Checking only divisibility by 3 and missing the nested condition.
Quick Check: Is 45 divisible by 5?

Q63. Which condition correctly checks whether a number is a two-digit positive number inside the positive-number block?
num = 56

if num > 0:
    if ______:
        print("Two Digit Positive")
    else:
        print("Positive but Not Two Digit")
else:
    print("Not Positive")

A) num > 10 and num < 99
B) num >= 10 and num <= 99
C) num <= 10 or num >= 99
D) num > 0 and num < 10
Correct Answer: B
Verified: Yes — two-digit positive numbers range from 10 to 99 inclusive.
Explanation:
Step 1: A two-digit positive number starts from 10.
Step 2: It ends at 99.
Final: The correct condition is num >= 10 and num <= 99.
Common Mistake: Using > and <, which wrongly exclude 10 and 99.
Quick Check: Is 10 a two-digit number?

Q64. What will be the output of the following code?
x = 7
y = 7

if x >= y:
    if x == y:
        print("Equal")
    else:
        print("x is Greater")
else:
    print("y is Greater")

A) x is Greater
B) y is Greater
C) Equal
D) Greater or Equal
Correct Answer: C
Verified: Yes — x >= y is true and x == y is also true.
Explanation:
Step 1: 7 >= 7 is true.
Step 2: 7 == 7 is true.
Final: Python prints Equal.
Common Mistake: Thinking >= always means strictly greater.
Quick Check: Does >= include equality?

Q65. What will be the output of the following code?
code = 404

if code >= 400:
    if code < 500:
        print("Client Error")
    else:
        print("Server Error")
else:
    print("Success or Redirect")

A) Success or Redirect
B) Server Error
C) Client Error
D) Invalid Code
Correct Answer: C
Verified: Yes — 404 is at least 400 and less than 500.
Explanation:
Step 1: 404 >= 400 is true.
Step 2: 404 < 500 is also true.
Final: Client Error is printed.
Common Mistake: Treating all values above 400 as server errors.
Quick Check: What will print for code = 503?

Q66. What will be the output of the following code?
maths = 40
science = 39

if maths >= 40:
    if science >= 40:
        print("Pass in Both")
    else:
        print("Science Reappear")
else:
    print("Maths Reappear")

A) Science Reappear
B) Pass in Both
C) Maths Reappear
D) Fail in Both
Correct Answer: A
Verified: Yes — maths condition is true, but science condition is false.
Explanation:
Step 1: maths >= 40 is true because maths is exactly 40.
Step 2: science >= 40 is false because science is 39.
Final: Science Reappear is printed.
Common Mistake: Forgetting that exactly 40 is passing.
Quick Check: Is science passing if marks are 40?

Q67. What will be the output of the following code?
x = 15

if x > 10:
    if x % 2 == 0 or x % 5 == 0:
        print("Special")
    else:
        print("Normal")
else:
    print("Small")

A) Normal
B) Small
C) Special
D) Even Only
Correct Answer: C
Verified: Yes — x > 10 is true, and x % 5 == 0 is true.
Explanation:
Step 1: 15 > 10 is true.
Step 2: 15 % 2 == 0 is false, but 15 % 5 == 0 is true.
Final: Since or needs only one true condition, Special is printed.
Common Mistake: Thinking both conditions around or must be true.
Quick Check: Is 15 divisible by 5?

Q68. What will be the output of the following code?
amount = 999
coupon = True

if amount >= 1000:
    if coupon:
        print("Big Discount")
    else:
        print("Standard Discount")
else:
    print("Small Discount")

A) Big Discount
B) Standard Discount
C) Coupon Applied
D) Small Discount
Correct Answer: D
Verified: Yes — amount >= 1000 is false, so the nested coupon check is skipped.
Explanation:
Step 1: 999 >= 1000 is false.
Step 2: Python directly goes to the outer else.
Final: Small Discount is printed.
Common Mistake: Checking coupon even when the amount condition fails.
Quick Check: Will the inner if coupon run for amount 999?

Q69. What will be the output of the following code?
a = 6
b = 2
c = 3

if a == b * c:
    if a / b == c:
        print("Both True")
    else:
        print("Only Multiplication True")
else:
    print("First False")

A) First False
B) Only Multiplication True
C) Both True
D) Division Error
Correct Answer: C
Verified: Yes — 6 == 2 * 3 is true and 6 / 2 == 3 is also true.
Explanation:
Step 1: b * c is 2 * 3 = 6.
Step 2: a == b * c is true.
Step 3: a / b == c becomes 6 / 2 == 3, which is true.
Final: Both True is printed.
Common Mistake: Not evaluating multiplication/division before comparison.
Quick Check: What is 6 / 2 in Python?

Q70. Which condition should replace the blank to check whether a character is a lowercase vowel inside the alphabet block?
ch = "e"

if ch >= "a" and ch <= "z":
    if ______:
        print("Lowercase Vowel")
    else:
        print("Lowercase Consonant")
else:
    print("Not Lowercase Alphabet")

A) ch == "a" and ch == "e" and ch == "i"
B) ch == "a" or ch == "e" or ch == "i" or ch == "o" or ch == "u"
C) ch != "a" or ch != "e"
D) ch >= "a" and ch <= "u"
Correct Answer: B
Verified: Yes — a vowel check needs equality with any one vowel using or.
Explanation:
Step 1: The outer condition checks lowercase alphabet range.
Step 2: A character can be only one vowel at a time.
Final: Use or between vowel comparisons.
Common Mistake: Using and between vowel checks; one character cannot be "a" and "e" at the same time.
Quick Check: Should vowel conditions use and or or?

Q71. What will be the output of the following code?
salary = 50000
experience = 2

if salary >= 40000:
    if experience >= 3:
        print("Senior Package")
    else:
        print("Junior Package")
else:
    print("Entry Package")

A) Senior Package
B) Entry Package
C) Junior Package
D) Salary Low
Correct Answer: C
Verified: Yes — salary condition is true, but experience condition is false.
Explanation:
Step 1: 50000 >= 40000 is true.
Step 2: 2 >= 3 is false.
Final: The inner else prints Junior Package.
Common Mistake: Assuming salary alone decides senior package.
Quick Check: What minimum experience is required for senior package?

Q72. What will be the output of the following code?
x = 5
y = 10

if x < y:
    if x * 2 == y:
        print("Double")
    else:
        print("Less")
else:
    print("Greater or Equal")

A) Less
B) Greater or Equal
C) Double
D) Equal
Correct Answer: C
Verified: Yes — 5 < 10 is true and 5 * 2 == 10 is also true.
Explanation:
Step 1: x < y means 5 < 10, which is true.
Step 2: x * 2 == y means 10 == 10, which is true.
Final: Python prints Double.
Common Mistake: Stopping after x < y and selecting Less without checking inner condition.
Quick Check: What is x * 2 here?

Q73. What will be the output of the following code?
age = 21
has_ticket = True
has_id = False

if age >= 18:
    if has_ticket and has_id:
        print("Entry Confirmed")
    else:
        print("Documents Missing")
else:
    print("Underage")

A) Entry Confirmed
B) Underage
C) Documents Missing
D) Ticket Missing
Correct Answer: C
Verified: Yes — age condition is true, but has_ticket and has_id is false.
Explanation:
Step 1: 21 >= 18 is true.
Step 2: has_ticket and has_id becomes True and False.
Final: Since and requires both true, Documents Missing is printed.
Common Mistake: Thinking one document is enough when and is used.
Quick Check: What does True and False evaluate to?

Q74. What will be the output of the following code?
p = 10
q = 20

if p != q:
    if p + q > 25:
        print("Different and Large Sum")
    else:
        print("Different and Small Sum")
else:
    print("Same Values")

A) Different and Small Sum
B) Same Values
C) Different and Large Sum
D) Large Only
Correct Answer: C
Verified: Yes — p != q is true and p + q > 25 is also true.
Explanation:
Step 1: 10 != 20 is true.
Step 2: p + q is 30.
Step 3: 30 > 25 is true.
Final: Different and Large Sum is printed.
Common Mistake: Misreading != as equality.
Quick Check: What does != mean?

Q75. What will be the output of the following code?
number = 101

if number > 0:
    if number % 10 == 0:
        print("Positive Multiple of 10")
    else:
        print("Positive but Not Multiple of 10")
else:
    print("Not Positive")

A) Positive Multiple of 10
B) Not Positive
C) Positive Number
D) Positive but Not Multiple of 10
Correct Answer: D
Verified: Yes — number > 0 is true, but 101 % 10 == 0 is false.
Explanation:
Step 1: 101 > 0 is true.
Step 2: 101 % 10 gives remainder 1.
Final: Since the inner condition is false, Positive but Not Multiple of 10 is printed.
Common Mistake: Thinking all numbers greater than 100 are multiples of 10.
Quick Check: What is the remainder when 101 is divided by 10?

Q76. What will be the output of the following code?
a = 7
b = 3
c = 2

if a + b * c > 12:
    if (a - b) % c == 0:
        print("Alpha")
    else:
        print("Beta")
else:
    print("Gamma")

A) Alpha
B) Beta
C) Gamma
D) Alpha Beta
Correct Answer: A
Verified: Yes — b * c is evaluated first, so 7 + 6 > 12 is true; (7 - 3) % 2 == 0 is also true.
Explanation: Multiplication has higher precedence than addition, and parentheses are evaluated first.
Common Mistake: Calculating a + b * c as (a + b) * c.

Q77. What will be the output of the following code?
x = 18
y = 4

if x // y == 4:
    if x % y > 1:
        print("Remainder High")
    else:
        print("Remainder Low")
else:
    print("Quotient Different")

A) Quotient Different
B) Remainder High
C) Remainder Low
D) Division Error
Correct Answer: B
Verified: Yes — 18 // 4 is 4 and 18 % 4 is 2, which is greater than 1.
Explanation: // gives integer quotient and % gives remainder.
Common Mistake: Confusing // with %.

Q78. What will be the output of the following code?
m = 5
n = 2
p = 3

if m * n + p == 13:
    if m + n * p == 11:
        print("Both Match")
    else:
        print("First Match")
else:
    print("No Match")

A) First Match
B) No Match
C) Both Match
D) Second Match
Correct Answer: C
Verified: Yes — 5 * 2 + 3 = 13 and 5 + 2 * 3 = 11.
Explanation: Multiplication is done before addition in both expressions.
Common Mistake: Evaluating expressions from left to right without considering precedence.

Q79. What will be the output of the following code?
x = 9

if x % 2 == 0:
    print("Even")
else:
    if x % 3 == 0 and x > 5:
        print("Odd Multiple")
    else:
        print("Odd Other")

A) Even
B) Odd Other
C) Multiple Only
D) Odd Multiple
Correct Answer: D
Verified: Yes — 9 is not even, but 9 % 3 == 0 and 9 > 5 are both true.
Explanation: Since the outer if fails, Python checks the nested condition inside else.
Common Mistake: Ignoring the nested condition after the outer else.

Q80. What will be the output of the following code?
price = 200
tax = 18

if price + price * tax // 100 >= 236:
    if tax * 2 < 40:
        print("Bill OK")
    else:
        print("High Tax")
else:
    print("Low Bill")

A) Bill OK
B) High Tax
C) Low Bill
D) Tax Error
Correct Answer: A
Verified: Yes — price * tax // 100 is 36, so total is 236; 18 * 2 < 40 is true.
Explanation: Multiplication and integer division happen before addition.
Common Mistake: Adding price + price before applying tax.

Q81. What will be the output of the following code?
a = 10
b = 5
c = 2

if a / b == c:
    if a // c == b:
        print("Double Check")
    else:
        print("Only First")
else:
    print("Failed")

A) Only First
B) Double Check
C) Failed
D) First Failed
Correct Answer: B
Verified: Yes — 10 / 5 is 2.0, which equals 2, and 10 // 2 is 5.
Explanation: / gives float division, but 2.0 == 2 is true in Python.
Common Mistake: Thinking 2.0 and 2 are unequal in comparison.

Q82. What will be the output of the following code?
units = 75

if units * 2 > 100:
    if units % 10 == 5 or units < 50:
        print("Check Meter")
    else:
        print("Normal")
else:
    print("Low Units")

A) Normal
B) Low Units
C) Check Meter
D) Meter Error
Correct Answer: C
Verified: Yes — 75 * 2 > 100 is true, and 75 % 10 == 5 is true.
Explanation: With or, only one condition needs to be true.
Common Mistake: Treating or as if both sides must be true.

Q83. What will be the output of the following code?
score = 64
bonus = 6

if score + bonus >= 70:
    if score >= 70 or bonus >= 10:
        print("Direct Pass")
    else:
        print("Grace Passed")
else:
    print("Fail")

A) Direct Pass
B) Fail
C) Bonus Failed
D) Grace Passed
Correct Answer: D
Verified: Yes — 64 + 6 >= 70 is true, but score >= 70 or bonus >= 10 is false.
Explanation: The outer condition passes due to total score, but the inner condition fails.
Common Mistake: Assuming outer success automatically means inner success.

Q84. What will be the output of the following code?
x = 4
y = 6

if not x * y < 20:
    if x + y == 10:
        print("Valid Sum")
    else:
        print("Invalid Sum")
else:
    print("Small Product")

A) Valid Sum
B) Invalid Sum
C) Small Product
D) Product Error
Correct Answer: A
Verified: Yes — x * y is 24; 24 < 20 is false; not False is true.
Explanation: Arithmetic is evaluated before comparison, and not reverses the Boolean result.
Common Mistake: Applying not to x only instead of the whole comparison.

Q85. What will be the output of the following code?
a = 3
b = 4
c = 5

if a * a + b * b == c * c:
    if c > a + b:
        print("Long Side")
    else:
        print("Right Triangle")
else:
    print("Not Right")

A) Long Side
B) Right Triangle
C) Not Right
D) Equal Sides
Correct Answer: B
Verified: Yes — 3*3 + 4*4 = 25 and 5*5 = 25; 5 > 7 is false.
Explanation: The first condition is true, but the nested condition is false.
Common Mistake: Thinking a true outer condition means the first inner branch will also run.

Q86. What will be the output of the following code?
num = 28

if num % 4 == 0:
    if num % 7 == 0:
        print("Divisible by 4 and 7")
    else:
        print("Divisible by 4 only")
else:
    print("Not Divisible by 4")

A) Divisible by 4 only
B) Not Divisible by 4
C) Divisible by 4 and 7
D) Divisible by 7 only
Correct Answer: C
Verified: Yes — 28 % 4 == 0 and 28 % 7 == 0.
Explanation: Both divisibility checks are true.
Common Mistake: Checking only the outer divisibility condition.

Q87. What will be the output of the following code?
x = 12
y = 3

if x - y * 2 > 5:
    if (x - y) * 2 > 15:
        print("Parentheses Matter")
    else:
        print("Only First")
else:
    print("First Failed")

A) First Failed
B) Only First
C) Arithmetic Error
D) Parentheses Matter
Correct Answer: D
Verified: Yes — 12 - 3 * 2 = 6, and (12 - 3) * 2 = 18.
Explanation: Parentheses change the order of calculation.
Common Mistake: Treating x - y * 2 and (x - y) * 2 as the same.

Q88. What will be the output of the following code?
p = 8
q = 2
r = 5

if p // q + r == 9:
    if p % (q + r) == 1:
        print("Case A")
    else:
        print("Case B")
else:
    print("Case C")

A) Case A
B) Case B
C) Case C
D) Case D
Correct Answer: A
Verified: Yes — 8 // 2 + 5 = 9, and 8 % 7 = 1.
Explanation: Parentheses make q + r evaluate before modulo.
Common Mistake: Calculating p % q + r instead of p % (q + r).

Q89. What will be the output of the following code?
marks = 71
penalty = 2

if marks - penalty >= 70:
    print("Clear Pass")
else:
    if marks >= 70:
        print("Penalty Changed Result")
    else:
        print("Fail")

A) Clear Pass
B) Penalty Changed Result
C) Fail
D) Penalty Ignored
Correct Answer: B
Verified: Yes — 71 - 2 = 69, so outer if fails; original marks are still >= 70.
Explanation: The penalty changes the result after subtraction.
Common Mistake: Checking original marks only.

Q90. What will be the output of the following code?
a = 14
b = 5

if a % b == 4:
    if a // b == 2 and a - b > 8:
        print("Both True")
    else:
        print("Only Remainder")
else:
    print("Different Remainder")

A) Only Remainder
B) Different Remainder
C) Both True
D) Quotient Error
Correct Answer: C
Verified: Yes — 14 % 5 = 4, 14 // 5 = 2, and 14 - 5 > 8 is true.
Explanation: The nested and condition has both sides true.
Common Mistake: Forgetting to check both sides of and.

Q91. What will be the output of the following code?
x = 6
y = 2
z = 3

if x == y * z:
    if x / y == z and z + 1 == 4:
        print("Exact Relation")
    else:
        print("Partial Relation")
else:
    print("No Relation")

A) No Relation
B) Partial Relation
C) Multiplication Only
D) Exact Relation
Correct Answer: D
Verified: Yes — 6 == 2 * 3, 6 / 2 == 3, and 3 + 1 == 4.
Explanation: Both the outer and inner conditions are true.
Common Mistake: Missing the second condition joined with and.

Q92. What will be the output of the following code?
n = 27

if n % 2 != 0:
    if n % 3 == 0 and n % 9 == 0:
        print("Odd and Multiple of 9")
    else:
        print("Odd Only")
else:
    print("Even")

A) Odd and Multiple of 9
B) Odd Only
C) Even
D) Multiple of 3 Only
Correct Answer: A
Verified: Yes — 27 is odd and divisible by both 3 and 9.
Explanation: != 0 checks that the number is not even.
Common Mistake: Thinking odd numbers cannot be multiples of 9.

Q93. What will be the output of the following code?
a = 5
b = 2
c = 11

if a * b + 1 == c:
    if c // b == 5 and c % b == 1:
        print("Quotient and Remainder")
    else:
        print("Only Product")
else:
    print("Mismatch")

A) Only Product
B) Quotient and Remainder
C) Mismatch
D) Product Error
Correct Answer: B
Verified: Yes — 5 * 2 + 1 = 11, 11 // 2 = 5, and 11 % 2 = 1.
Explanation: The code checks both multiplication-based expression and division result.
Common Mistake: Mixing quotient and remainder values.

Q94. What will be the output of the following code?
x = 20

if x > 10:
    if not x < 20:
        print("At Least 20")
    else:
        print("Between 11 and 19")
else:
    print("10 or Less")

A) Between 11 and 19
B) 10 or Less
C) At Least 20
D) Greater Than 10
Correct Answer: C
Verified: Yes — x > 10 is true, and not x < 20 means not False, which is true.
Explanation: not x < 20 is equivalent to saying x >= 20.
Common Mistake: Reading not x < 20 as x < 20.

Q95. What will be the output of the following code?
a = 9
b = 6

if a > b:
    if a - b * 2 > 0:
        print("Far Greater")
    else:
        print("Only Greater")
else:
    print("Not Greater")

A) Far Greater
B) Not Greater
C) Equal
D) Only Greater
Correct Answer: D
Verified: Yes — 9 > 6 is true, but 9 - 6 * 2 = -3, so the inner condition is false.
Explanation: Multiplication happens before subtraction.
Common Mistake: Calculating (a - b) * 2.

Q96. What will be the output of the following code?
wallet = 150
item = 120
fee = 30

if wallet >= item + fee:
    if wallet - item - fee == 0:
        print("Exact Payment")
    else:
        print("Money Left")
else:
    print("Not Enough")

A) Exact Payment
B) Money Left
C) Not Enough
D) Fee Missing
Correct Answer: A
Verified: Yes — item + fee is 150, and 150 - 120 - 30 is 0.
Explanation: The wallet exactly covers both item cost and fee.
Common Mistake: Checking only item price and ignoring fee.

Q97. What will be the output of the following code?
x = 3
y = 7
z = 10

if x + y == z:
    if z % y == x:
        print("Remainder Match")
    else:
        print("Sum Match")
else:
    print("No Match")

A) Sum Match
B) Remainder Match
C) No Match
D) Remainder Error
Correct Answer: B
Verified: Yes — 3 + 7 == 10, and 10 % 7 == 3.
Explanation: Both the sum and remainder relationships are true.
Common Mistake: Thinking 10 % 7 gives 7.

Q98. What will be the output of the following code?
n = 44

if n % 11 == 0:
    if n // 11 > 3:
        print("Above Three Elevens")
    else:
        print("Three or Less Elevens")
else:
    print("Not Multiple of 11")

A) Three or Less Elevens
B) Not Multiple of 11
C) Above Three Elevens
D) Eleven Error
Correct Answer: C
Verified: Yes — 44 % 11 == 0, and 44 // 11 == 4, which is greater than 3.
Explanation: The quotient tells how many times 11 fits into 44.
Common Mistake: Checking only the remainder and not the quotient.

Q99. What will be the output of the following code?
a = 13
b = 4
c = 1

if a // b == 3:
    if a % b == c:
        print("Division Pattern")
    else:
        print("Quotient Only")
else:
    print("Different Quotient")

A) Quotient Only
B) Different Quotient
C) Remainder Only
D) Division Pattern
Correct Answer: D
Verified: Yes — 13 // 4 == 3, and 13 % 4 == 1.
Explanation: Both quotient and remainder match the expected values.
Common Mistake: Confusing integer division result with normal division.

Q100. What will be the output of the following code?
score = 49
extra = 1

if score + extra >= 50:
    if score >= 50:
        print("Passed Directly")
    else:
        print("Passed With Extra")
else:
    print("Failed")

A) Passed With Extra
B) Passed Directly
C) Failed
D) Extra Ignored
Correct Answer: A
Verified: Yes — 49 + 1 >= 50 is true, but original score 49 >= 50 is false.
Explanation: The extra mark helps the student pass.
Common Mistake: Looking only at the original score.
Q101. What will be the output of the following code?
x = 2
y = 3
z = 4

if x + y * z == 14:
    if (x + y) * z == 20:
        print("Both Expressions")
    else:
        print("First Expression")
else:
    print("No Expression")

A) First Expression
B) Both Expressions
C) No Expression
D) Expression Error
Correct Answer: B
Verified: Yes — 2 + 3 * 4 = 14, and (2 + 3) * 4 = 20.
Explanation: Parentheses change the result of the expression.
Common Mistake: Treating both expressions as equal.

Q102. What will be the output of the following code?
n = 100

if n / 10 == 10:
    if n // 30 == 3 and n % 30 == 10:
        print("Mixed Division")
    else:
        print("Simple Division")
else:
    print("Not Ten Times")

A) Simple Division
B) Not Ten Times
C) Mixed Division
D) Division Failed
Correct Answer: C
Verified: Yes — 100 / 10 == 10, 100 // 30 == 3, and 100 % 30 == 10.
Explanation: The code combines normal division, integer division, and modulo.
Common Mistake: Thinking /, //, and % produce the same type of result.

Q103. What will be the output of the following code?
a = 6
b = 8

if a * b > 50:
    print("Large Product")
else:
    if a + b == 14:
        print("Sum Saves")
    else:
        print("Small Values")

A) Large Product
B) Small Values
C) Product Saves
D) Sum Saves
Correct Answer: D
Verified: Yes — 6 * 8 = 48, so outer if fails; 6 + 8 == 14 is true.
Explanation: The nested condition inside else is checked after product condition fails.
Common Mistake: Assuming product is greater than 50 without calculating.

Q104. What will be the output of the following code?
x = 16
y = 4

if x // y == y:
    if x % y == 0 and y * 3 < x:
        print("Square Like")
    else:
        print("Only Division")
else:
    print("Different")

A) Square Like
B) Only Division
C) Different
D) Remainder Found
Correct Answer: A
Verified: Yes — 16 // 4 == 4, 16 % 4 == 0, and 4 * 3 < 16.
Explanation: All conditions in the nested and expression are true.
Common Mistake: Forgetting to check the y * 3 < x part.

Q105. What will be the output of the following code?
num = 35

if num % 5 == 0:
    if num % 2 == 0 or num % 7 == 0:
        print("Special Multiple")
    else:
        print("Only Multiple of 5")
else:
    print("Not Multiple of 5")

A) Only Multiple of 5
B) Special Multiple
C) Not Multiple of 5
D) Even Multiple
Correct Answer: B
Verified: Yes — 35 % 5 == 0, and 35 % 7 == 0, so the or condition is true.
Explanation: Only one side of or needs to be true.
Common Mistake: Ignoring the second side of or.

Q106. What will be the output of the following code?
m = 7
n = 7

if m != n:
    print("Different")
else:
    if m * n == 49:
        print("Equal Product")
    else:
        print("Equal Only")

A) Different
B) Equal Only
C) Equal Product
D) Product Error
Correct Answer: C
Verified: Yes — m != n is false, so else runs; 7 * 7 == 49 is true.
Explanation: The nested condition runs only because the values are equal.
Common Mistake: Misreading != as equal to.

Q107. What will be the output of the following code?
a = 2
b = 5
c = 12

if a + b > c:
    print("Greater Sum")
else:
    if c - b * a == 2:
        print("Precedence Result")
    else:
        print("Different Result")

A) Greater Sum
B) Different Result
C) Sum Equal
D) Precedence Result
Correct Answer: D
Verified: Yes — 2 + 5 > 12 is false; 12 - 5 * 2 = 2.
Explanation: Multiplication is done before subtraction.
Common Mistake: Calculating (c - b) * a.

Q108. What will be the output of the following code?
bill = 999
discount = 99

if bill - discount >= 900:
    if bill // 100 == 9 and discount % 10 == 9:
        print("Offer Applied")
    else:
        print("Offer Partial")
else:
    print("Offer Failed")

A) Offer Applied
B) Offer Partial
C) Offer Failed
D) Discount Error
Correct Answer: A
Verified: Yes — 999 - 99 = 900, 999 // 100 == 9, and 99 % 10 == 9.
Explanation: Both nested checks are true after the outer discount condition passes.
Common Mistake: Thinking 999 // 100 is 10.

Q109. What will be the output of the following code?
x = 11

if x > 10:
    if x % 2 == 1 and not x > 15:
        print("Small Odd Above Ten")
    else:
        print("Other Above Ten")
else:
    print("Ten or Below")

A) Other Above Ten
B) Small Odd Above Ten
C) Ten or Below
D) Odd Only
Correct Answer: B
Verified: Yes — 11 % 2 == 1 is true, and not x > 15 is also true.
Explanation: not x > 15 means not (x > 15).
Common Mistake: Applying not incorrectly in the condition.

Q110. What will be the output of the following code?
a = 30
b = 6
c = 5

if a // b == c:
    if a / b == c:
        print("Both Division True")
    else:
        print("Integer Division Only")
else:
    print("Division False")

A) Integer Division Only
B) Division False
C) Both Division True
D) Quotient Error
Correct Answer: C
Verified: Yes — 30 // 6 is 5, and 30 / 6 is 5.0, which equals 5.
Explanation: / gives float division, while // gives integer division.
Common Mistake: Thinking 5.0 == 5 is false.

Q111. What will be the output of the following code?
n = 81

if n % 9 == 0:
    if n // 9 == 9 and n % 2 == 1:
        print("Nine Square Odd")
    else:
        print("Multiple of Nine")
else:
    print("Not Nine")

A) Multiple of Nine
B) Not Nine
C) Nine Only
D) Nine Square Odd
Correct Answer: D
Verified: Yes — 81 % 9 == 0, 81 // 9 == 9, and 81 is odd.
Explanation: Both nested conditions joined by and are true.
Common Mistake: Forgetting that 81 is odd.

Q112. What will be the output of the following code?
x = 14
y = 7
z = 2

if x == y * z:
    if x // z == y and x % z == 0:
        print("Clean Relation")
    else:
        print("Rough Relation")
else:
    print("No Relation")

A) Clean Relation
B) Rough Relation
C) No Relation
D) Multiplication Error
Correct Answer: A
Verified: Yes — 14 == 7 * 2, 14 // 2 == 7, and 14 % 2 == 0.
Explanation: Multiplication, quotient, and remainder relations all match.
Common Mistake: Checking only x == y * z.

Q113. What will be the output of the following code?
age = 20
marks = 74

if age // 10 == 2:
    if marks + age > 95:
        print("Strong Candidate")
    else:
        print("Age Group OK")
else:
    print("Different Age Group")

A) Strong Candidate
B) Age Group OK
C) Different Age Group
D) Marks OK
Correct Answer: B
Verified: Yes — 20 // 10 == 2, but 74 + 20 > 95 is false.
Explanation: The age group condition is true, but the nested total condition fails.
Common Mistake: Treating 94 > 95 as true.

Q114. What will be the output of the following code?
a = 5
b = 5
c = 9

if a + b > c:
    if (a + b) % c == 1:
        print("Close Sum")
    else:
        print("Large Sum")
else:
    print("Small Sum")

A) Large Sum
B) Small Sum
C) Close Sum
D) Equal Sum
Correct Answer: C
Verified: Yes — 5 + 5 > 9, and 10 % 9 == 1.
Explanation: The sum is greater than c, and its remainder with c is 1.
Common Mistake: Thinking 10 % 9 is 9.

Q115. What will be the output of the following code?
x = 24

if x % 6 == 0:
    if x % 4 == 0 and x % 8 == 0:
        print("Multiple of 6, 4 and 8")
    else:
        print("Multiple of 6 Only")
else:
    print("Not Multiple of 6")

A) Multiple of 6 Only
B) Not Multiple of 6
C) Multiple of 4 Only
D) Multiple of 6, 4 and 8
Correct Answer: D
Verified: Yes — 24 is divisible by 6, 4, and 8.
Explanation: All nested divisibility checks are true.
Common Mistake: Checking only divisibility by 6.

Q116. What will be the output of the following code?
num = 17

if num > 10:
    if num % 3 == 2 and num % 5 == 2:
        print("Same Remainders")
    else:
        print("Different Remainders")
else:
    print("Small Number")

A) Same Remainders
B) Different Remainders
C) Small Number
D) Remainder Zero
Correct Answer: A
Verified: Yes — 17 % 3 == 2 and 17 % 5 == 2.
Explanation: The number gives the same remainder for both divisors.
Common Mistake: Assuming modulo must always give zero.

Q117. What will be the output of the following code?
p = 4
q = 9

if p * p > q + 5:
    if q - p == 5:
        print("Math Match")
    else:
        print("Square Only")
else:
    print("Small Square")

A) Square Only
B) Math Match
C) Small Square
D) Difference Error
Correct Answer: B
Verified: Yes — 4 * 4 = 16, 9 + 5 = 14, and 9 - 4 == 5.
Explanation: Both the square comparison and difference check are true.
Common Mistake: Calculating p * p after comparing q + 5.

Q118. What will be the output of the following code?
total = 250
tax = 25

if total + tax * 2 >= 300:
    if (total + tax) * 2 >= 550:
        print("Both Totals")
    else:
        print("First Total")
else:
    print("Below Total")

A) First Total
B) Below Total
C) Both Totals
D) Tax Missing
Correct Answer: C
Verified: Yes — 250 + 25 * 2 = 300, and (250 + 25) * 2 = 550.
Explanation: Parentheses change the second expression.
Common Mistake: Treating total + tax * 2 and (total + tax) * 2 as the same.

Q119. What will be the output of the following code?
x = 50
y = 15

if x - y * 3 >= 5:
    if (x - y) * 3 >= 100:
        print("Parentheses Bigger")
    else:
        print("First Bigger")
else:
    print("Too Small")

A) First Bigger
B) Too Small
C) Equal Result
D) Parentheses Bigger
Correct Answer: D
Verified: Yes — 50 - 15 * 3 = 5, and (50 - 15) * 3 = 105.
Explanation: The expression with parentheses gives a much larger result.
Common Mistake: Ignoring parentheses.

Q120. What will be the output of the following code?
n = 64

if n // 8 == 8:
    if n % 8 == 0 and n / 8 == 8:
        print("Perfect Eight")
    else:
        print("Integer Eight")
else:
    print("Not Eight")

A) Perfect Eight
B) Integer Eight
C) Not Eight
D) Division Error
Correct Answer: A
Verified: Yes — 64 // 8 == 8, 64 % 8 == 0, and 64 / 8 == 8.0.
Explanation: Both integer division and normal division match the expected value.
Common Mistake: Thinking 8.0 == 8 is false.

Q121. What will be the output of the following code?
a = 12
b = 2
c = 5

if a > b + c:
    if a - b * c == 2:
        print("Precedence Check")
    else:
        print("Greater Only")
else:
    print("Not Greater")

A) Greater Only
B) Precedence Check
C) Not Greater
D) Addition Error
Correct Answer: B
Verified: Yes — 12 > 2 + 5, and 12 - 2 * 5 = 2.
Explanation: Multiplication happens before subtraction.
Common Mistake: Calculating (a - b) * c.

Q122. What will be the output of the following code?
income = 500000
tax_rate = 10

if income // 100000 >= 5:
    if income * tax_rate // 100 == 50000:
        print("Tax Computed")
    else:
        print("Tax Different")
else:
    print("Income Low")

A) Tax Different
B) Income Low
C) Tax Computed
D) Rate Error
Correct Answer: C
Verified: Yes — 500000 // 100000 == 5, and 500000 * 10 // 100 == 50000.
Explanation: Multiplication is performed before integer division.
Common Mistake: Dividing by 100 before multiplying mentally and losing track of result.

Q123. What will be the output of the following code?
x = 9
y = 2

if x // y == 4:
    if x / y == 4:
        print("Both Four")
    else:
        print("Integer Only")
else:
    print("Not Four")

A) Both Four
B) Not Four
C) Division Same
D) Integer Only
Correct Answer: D
Verified: Yes — 9 // 2 == 4, but 9 / 2 == 4.5, not 4.
Explanation: // removes the decimal part, while / keeps it.
Common Mistake: Thinking / and // always give the same result.

Q124. What will be the output of the following code?
a = 7
b = 3
c = 21

if a * b == c:
    if c // a == b or c // b == a:
        print("Product Verified")
    else:
        print("Product Only")
else:
    print("Product Failed")

A) Product Verified
B) Product Only
C) Product Failed
D) Division Failed
Correct Answer: A
Verified: Yes — 7 * 3 == 21, and both division checks actually satisfy the or.
Explanation: The product and quotient relationships are correct.
Common Mistake: Forgetting that or needs only one true condition.

Q125. What will be the output of the following code?
m = 40
n = 8
p = 5

if m / n == p:
    if m // n == p and m % n == 0:
        print("Exact Divide")
    else:
        print("Normal Divide")
else:
    print("Not Divide")

A) Normal Divide
B) Exact Divide
C) Not Divide
D) Remainder Found
Correct Answer: B
Verified: Yes — 40 / 8 == 5.0, 40 // 8 == 5, and 40 % 8 == 0.
Explanation: Both normal division and integer division show exact divisibility.
Common Mistake: Thinking / and // always differ even when division is exact.


Q126. What will be the output of the following code?
a = 24
b = 6
c = 3
d = 2

if a % b == 0:
    if a // b > c:
        if (a + b) // c == 10:
            if d * d == 4:
                print("Deep Match")
            else:
                print("Power Mismatch")
        else:
            print("Sum Division Failed")
    else:
        print("Quotient Low")
else:
    print("Not Divisible")

A) Deep Match
B) Power Mismatch
C) Sum Division Failed
D) Quotient Low
Correct Answer: A
Verified: Yes — 24 % 6 = 0, 24 // 6 = 4, (24+6)//3 = 10, and 2*2 = 4.
Explanation: All four nested conditions are true, so the deepest print() executes.
Common Mistake: Forgetting that // gives integer quotient.

Q127. What will be the output of the following code?
x = 18
y = 5
z = 2

if x - y * z > 7:
    if (x + y) % z == 1:
        if x // z == 9:
            if y + z * z == 9:
                print("All Clear")
            else:
                print("Last Check Failed")
        else:
            print("Division Failed")
    else:
        print("Remainder Failed")
else:
    print("Outer Failed")

A) Outer Failed
B) All Clear
C) Division Failed
D) Last Check Failed
Correct Answer: B
Verified: Yes — 18 - 5*2 = 8, 23 % 2 = 1, 18 // 2 = 9, and 5 + 2*2 = 9.
Explanation: Multiplication happens before subtraction and addition. All conditions are true.
Common Mistake: Calculating x - y * z as (x - y) * z.

Q128. What will be the output of the following code?
m = 30
n = 4
p = 6

if m // n == 7:
    if m % n == 2:
        if n * p > 25:
            if m - p == 24:
                print("Full Match")
            else:
                print("Difference Failed")
        else:
            print("Product Low")
    else:
        print("Remainder Failed")
else:
    print("Quotient Failed")

A) Full Match
B) Difference Failed
C) Product Low
D) Remainder Failed
Correct Answer: C
Verified: Yes — 30 // 4 = 7, 30 % 4 = 2, but 4 * 6 = 24, not greater than 25.
Explanation: The first two conditions pass, but the third nested condition fails.
Common Mistake: Thinking 24 > 25 is true because the values are close.

Q129. What will be the output of the following code?
score = 48
bonus = 4
penalty = 1

if score + bonus >= 50:
    if score - penalty >= 45:
        if bonus * 2 + penalty == 9:
            if score + bonus - penalty == 51:
                print("Final Pass")
            else:
                print("Final Total Failed")
        else:
            print("Bonus Rule Failed")
    else:
        print("Penalty Too High")
else:
    print("Fail")

A) Bonus Rule Failed
B) Penalty Too High
C) Fail
D) Final Pass
Correct Answer: D
Verified: Yes — 52 >= 50, 47 >= 45, 8 + 1 = 9, and 48 + 4 - 1 = 51.
Explanation: All nested maths conditions are true.
Common Mistake: Forgetting to subtract the penalty in the final condition.

Q130. What will be the output of the following code?
a = 9
b = 3
c = 2

if a % b == 0:
    if a // b == c:
        if a - b == 6:
            if c * b == a:
                print("All True")
            else:
                print("Last Failed")
        else:
            print("Subtraction Failed")
    else:
        print("Quotient Different")
else:
    print("Not Divisible")

A) All True
B) Quotient Different
C) Subtraction Failed
D) Not Divisible
Correct Answer: B
Verified: Yes — 9 % 3 = 0, but 9 // 3 = 3, which is not equal to 2.
Explanation: The outer condition is true, but the second-level condition fails.
Common Mistake: Assuming divisibility means the quotient will match any given value.

Q131. What will be the output of the following code?
n = 125

if n > 100:
    if n % 5 == 0:
        if n // 5 > 20:
            if n % 10 == 5:
                print("Ends with 5")
            else:
                print("Does Not End with 5")
        else:
            print("Quotient Small")
    else:
        print("Not Multiple of 5")
else:
    print("Too Small")

A) Not Multiple of 5
B) Quotient Small
C) Ends with 5
D) Too Small
Correct Answer: C
Verified: Yes — 125 > 100, 125 % 5 = 0, 125 // 5 = 25, and 125 % 10 = 5.
Explanation: The number satisfies all four nested checks.
Common Mistake: Confusing % 5 with % 10.

Q132. What will be the output of the following code?
p = 40
q = 8
r = 5

if p / q == r:
    if p // q == r:
        if p % q == 0:
            if q + r * 2 == 18:
                print("Exact Math")
            else:
                print("Expression Failed")
        else:
            print("Remainder Found")
    else:
        print("Integer Division Failed")
else:
    print("Normal Division Failed")

A) Exact Math
B) Expression Failed
C) Integer Division Failed
D) Remainder Found
Correct Answer: A
Verified: Yes — 40 / 8 = 5.0, 40 // 8 = 5, 40 % 8 = 0, and 8 + 5*2 = 18.
Explanation: Normal division and integer division both match because division is exact.
Common Mistake: Thinking 5.0 == 5 is false in Python.

Q133. What will be the output of the following code?
a = 14
b = 2
c = 3
d = 4

if a > b * c + d:
    if a - b * c == 8:
        if (a + d) // b == 9:
            if c + d == 7:
                print("Chain True")
            else:
                print("Addition Failed")
        else:
            print("Division Failed")
    else:
        print("Subtraction Failed")
else:
    print("Outer Failed")

A) Outer Failed
B) Chain True
C) Subtraction Failed
D) Division Failed
Correct Answer: B
Verified: Yes — 14 > 10, 14 - 6 = 8, 18 // 2 = 9, and 3 + 4 = 7.
Explanation: Operator precedence makes b * c + d equal to 10.
Common Mistake: Evaluating b * c + d incorrectly.

Q134. What will be the output of the following code?
x = 7
y = 4
z = 3

if x + y * z == 19:
    if (x + y) * z == 33:
        if x * z - y == 17:
            if z * z + y == 13:
                print("Precedence Perfect")
            else:
                print("Square Check Failed")
        else:
            print("Product Check Failed")
    else:
        print("Parentheses Check Failed")
else:
    print("First Check Failed")

A) Precedence Perfect
B) Square Check Failed
C) Product Check Failed
D) First Check Failed
Correct Answer: A
Verified: Yes — 7 + 4*3 = 19, (7+4)*3 = 33, 7*3 - 4 = 17, and 3*3 + 4 = 13.
Explanation: This question checks both precedence and parentheses.
Common Mistake: Treating x + y * z and (x + y) * z as same.

Q135. What will be the output of the following code?
a = 50
b = 15
c = 5

if a - b * c < 0:
    if (a - b) * c > 150:
        if a // c == 10:
            if b % c == 0:
                print("Parentheses Win")
            else:
                print("Remainder Failed")
        else:
            print("Quotient Failed")
    else:
        print("Parentheses Failed")
else:
    print("First Condition Failed")

A) Parentheses Failed
B) Parentheses Win
C) Quotient Failed
D) First Condition Failed
Correct Answer: B
Verified: Yes — 50 - 15*5 = -25, (50-15)*5 = 175, 50//5 = 10, and 15%5 = 0.
Explanation: Parentheses produce a very different value from normal precedence.
Common Mistake: Calculating (a - b) * c in the first condition also.

Q136. What will be the output of the following code?
num = 36

if num % 2 == 0:
    if num % 3 == 0:
        if num % 4 == 0:
            if num % 9 == 0:
                print("Divisible by 2, 3, 4 and 9")
            else:
                print("Not Divisible by 9")
        else:
            print("Not Divisible by 4")
    else:
        print("Not Divisible by 3")
else:
    print("Odd Number")

A) Not Divisible by 4
B) Not Divisible by 9
C) Divisible by 2, 3, 4 and 9
D) Odd Number
Correct Answer: C
Verified: Yes — 36 is divisible by 2, 3, 4, and 9.
Explanation: Every nested divisibility condition is true.
Common Mistake: Checking only divisibility by 2 and 3.

Q137. What will be the output of the following code?
n = 45

if n % 2 == 1:
    if n % 3 == 0:
        if n % 5 == 0:
            if n // 5 == 8:
                print("Exact Pattern")
            else:
                print("Multiple but Quotient Different")
        else:
            print("Not Multiple of 5")
    else:
        print("Not Multiple of 3")
else:
    print("Even Number")

A) Exact Pattern
B) Multiple but Quotient Different
C) Not Multiple of 5
D) Even Number
Correct Answer: B
Verified: Yes — 45 is odd and divisible by 3 and 5, but 45 // 5 = 9, not 8.
Explanation: The fourth-level condition fails.
Common Mistake: Assuming the quotient is 8 without calculating.

Q138. What will be the output of the following code?
wallet = 500
item = 350
tax = 35
fee = 15

if wallet >= item + tax + fee:
    if wallet - item >= tax + fee:
        if (tax + fee) * 2 == 100:
            if wallet // 100 == 5:
                print("Purchase Safe")
            else:
                print("Wallet Division Failed")
        else:
            print("Extra Cost Failed")
    else:
        print("Remaining Amount Low")
else:
    print("Not Enough")

A) Purchase Safe
B) Wallet Division Failed
C) Remaining Amount Low
D) Not Enough
Correct Answer: A
Verified: Yes — 350+35+15 = 400, remaining is 150, (35+15)*2 = 100, and 500//100 = 5.
Explanation: The wallet satisfies all nested cost checks.
Common Mistake: Ignoring tax and fee in the total cost.

Q139. What will be the output of the following code?
age = 19
marks = 78
income = 250000

if age < 25:
    if marks >= 75:
        if income // 100000 <= 2:
            if marks + age > 100:
                print("Eligible Premium")
            else:
                print("Eligible Basic")
        else:
            print("Income High")
    else:
        print("Marks Low")
else:
    print("Age Not Eligible")

A) Eligible Premium
B) Income High
C) Marks Low
D) Eligible Basic
Correct Answer: D
Verified: Yes — age and marks pass; 250000 // 100000 = 2, but 78 + 19 = 97, not greater than 100.
Explanation: The final nested condition fails, so Eligible Basic prints.
Common Mistake: Thinking 250000 // 100000 gives 2.5; // gives integer quotient.

Q140. What will be the output of the following code?
a = 11
b = 2
c = 5

if a // b == 5:
    if a % b == 1:
        if b * c == a - 1:
            if (a + b + c) % 3 == 0:
                print("Pattern Found")
            else:
                print("Final Remainder Failed")
        else:
            print("Product Failed")
    else:
        print("Remainder Failed")
else:
    print("Quotient Failed")

A) Pattern Found
B) Final Remainder Failed
C) Product Failed
D) Quotient Failed
Correct Answer: A
Verified: Yes — 11//2 = 5, 11%2 = 1, 2*5 = 10, and 18%3 = 0.
Explanation: The quotient, remainder, product, and final modulo all match.
Common Mistake: Confusing 11 / 2 with 11 // 2.

Q141. What will be the output of the following code?
x = 20
y = 6
z = 2

if x - y * z > 8:
    if x // y == 3:
        if x % y == 2:
            if z * y == 12:
                print("Deep True")
            else:
                print("Last Failed")
        else:
            print("Remainder Failed")
    else:
        print("Quotient Failed")
else:
    print("Outer Failed")

A) Deep True
B) Quotient Failed
C) Remainder Failed
D) Outer Failed
Correct Answer: D
Verified: Yes — 20 - 6*2 = 8, and 8 > 8 is false.
Explanation: Because the outer condition fails, none of the inner conditions are checked.
Common Mistake: Treating > as if it includes equality.

Q142. What will be the output of the following code?
m = 16
n = 3
p = 1

if m % n == 1:
    if m // n == 5:
        if (m + n) * p == 19:
            if not p > 1:
                print("Not Makes True")
            else:
                print("Not Failed")
        else:
            print("Expression Failed")
    else:
        print("Quotient Failed")
else:
    print("Remainder Failed")

A) Not Failed
B) Expression Failed
C) Not Makes True
D) Remainder Failed
Correct Answer: C
Verified: Yes — 16%3 = 1, 16//3 = 5, (16+3)*1 = 19, and not p > 1 is true.
Explanation: not p > 1 means not (p > 1). Since 1 > 1 is false, not False becomes true.
Common Mistake: Applying not only to p instead of the comparison.

Q143. What will be the output of the following code?
a = 8
b = 4
c = 2

if a == b * c:
    if a / b == c:
        if a // b == c:
            if a % b == 0:
                print("All Equal")
            else:
                print("Remainder Failed")
        else:
            print("Integer Division Failed")
    else:
        print("Normal Division Failed")
else:
    print("Multiplication Failed")

A) Multiplication Failed
B) Normal Division Failed
C) All Equal
D) Integer Division Failed
Correct Answer: C
Verified: Yes — 8 == 4*2, 8/4 = 2.0, 8//4 = 2, and 8%4 = 0.
Explanation: The number 8 divides exactly by 4.
Common Mistake: Thinking / and // always give different comparable results.

Q144. What will be the output of the following code?
price = 999
discount = 99
gst = 18

if price - discount == 900:
    if price // 100 == 9:
        if discount % 10 == 9:
            if gst * 5 == 90:
                print("Offer Valid")
            else:
                print("GST Failed")
        else:
            print("Discount Failed")
    else:
        print("Price Division Failed")
else:
    print("Final Price Failed")

A) Offer Valid
B) GST Failed
C) Discount Failed
D) Final Price Failed
Correct Answer: A
Verified: Yes — 999-99 = 900, 999//100 = 9, 99%10 = 9, and 18*5 = 90.
Explanation: All nested offer checks are true.
Common Mistake: Thinking 999 // 100 is 10.

Q145. What will be the output of the following code?
n = 28

if n % 7 == 0:
    if n % 4 == 0:
        if n // 7 + n // 4 == 11:
            if n // (7 - 3) == 7:
                print("Mixed Divisors")
            else:
                print("Parentheses Division Failed")
        else:
            print("Quotient Sum Failed")
    else:
        print("Not Multiple of 4")
else:
    print("Not Multiple of 7")

A) Not Multiple of 4
B) Quotient Sum Failed
C) Mixed Divisors
D) Parentheses Division Failed
Correct Answer: C
Verified: Yes — 28%7 = 0, 28%4 = 0, 4+7 = 11, and 28//4 = 7.
Explanation: Parentheses make 7 - 3 evaluate first.
Common Mistake: Ignoring parentheses in n // (7 - 3).

Q146. What will be the output of the following code?
a = 3
b = 5
c = 7

if a + b * c > 35:
    if (a + b) * c > 55:
        if c - b + a == 5:
            if a * b + c == 22:
                print("Four Level True")
            else:
                print("Final Expression Failed")
        else:
            print("Middle Expression Failed")
    else:
        print("Parentheses Failed")
else:
    print("Outer Failed")

A) Four Level True
B) Final Expression Failed
C) Parentheses Failed
D) Outer Failed
Correct Answer: A
Verified: Yes — 3+5*7 = 38, (3+5)*7 = 56, 7-5+3 = 5, and 3*5+7 = 22.
Explanation: This checks precedence and left-to-right evaluation for addition/subtraction.
Common Mistake: Calculating a + b * c as (a+b)*c.

Q147. What will be the output of the following code?
x = 64
y = 8

if x // y == 8:
    if x / y == 8:
        if x % y == 0:
            if y * y == x:
                print("Perfect Square Division")
            else:
                print("Square Failed")
        else:
            print("Remainder Failed")
    else:
        print("Normal Division Failed")
else:
    print("Integer Division Failed")

A) Perfect Square Division
B) Square Failed
C) Remainder Failed
D) Integer Division Failed
Correct Answer: A
Verified: Yes — 64//8 = 8, 64/8 = 8.0, 64%8 = 0, and 8*8 = 64.
Explanation: 64 is exactly divisible by 8, and 8 squared is 64.
Common Mistake: Thinking 8.0 == 8 is false.

Q148. What will be the output of the following code?
num = 30

if num > 10:
    if num < 50:
        if num % 6 == 0:
            if num % 4 == 0:
                print("Multiple of 6 and 4")
            else:
                print("Not Multiple of 4")
        else:
            print("Not Multiple of 6")
    else:
        print("Too Large")
else:
    print("Too Small")

A) Multiple of 6 and 4
B) Not Multiple of 6
C) Not Multiple of 4
D) Too Large
Correct Answer: C
Verified: Yes — 30 > 10, 30 < 50, 30%6 = 0, but 30%4 = 2.
Explanation: The first three nested conditions pass, but the fourth condition fails.
Common Mistake: Assuming a multiple of 6 is also a multiple of 4.

Q149. What will be the output of the following code?
a = 100
b = 20
c = 5

if a / b == c:
    if a // b == c:
        if a % b == 0:
            if a - b * c == 0:
                print("Exact Relationship")
            else:
                print("Expression Failed")
        else:
            print("Remainder Failed")
    else:
        print("Integer Division Failed")
else:
    print("Normal Division Failed")

A) Normal Division Failed
B) Expression Failed
C) Exact Relationship
D) Remainder Failed
Correct Answer: C
Verified: Yes — 100/20 = 5.0, 100//20 = 5, 100%20 = 0, and 100 - 20*5 = 0.
Explanation: All division and expression checks confirm the relationship.
Common Mistake: Calculating a - b * c as (a-b)*c.

Q150. What will be the output of the following code?
n = 57

if n > 50:
    if n % 2 != 0:
        if n % 3 == 0:
            if n // 3 == 19:
                print("Odd Triple Pattern")
            else:
                print("Quotient Failed")
        else:
            print("Not Multiple of 3")
    else:
        print("Even Above 50")
else:
    print("Small Number")

A) Odd Triple Pattern
B) Quotient Failed
C) Not Multiple of 3
D) Even Above 50
Correct Answer: A
Verified: Yes — 57 > 50, 57 is odd, 57%3 = 0, and 57//3 = 19.
Explanation: All four nested checks are true.
Common Mistake: Forgetting that != 0 means “not equal to zero.”

Q151. What will be the output of the following code?
n = 7

if (n & 1) == 1:
    print("Odd")
else:
    print("Even")

A) Even
B) Odd
C) One
D) Seven
Correct Answer: B
Verified: Yes — 7 & 1 gives 1.
Explanation:
Step 1: 7 is odd, so its last binary bit is 1.
Step 2: (n & 1) == 1 is true.
Final: Odd is printed.
Common Mistake: Thinking & works the same as logical and.
Quick Check: What is 6 & 1?

Q152. What will be the output of the following code?
n = 12

if (n & 1) == 0:
    print("Even")
else:
    print("Odd")

A) Odd
B) Even
C) Zero
D) Twelve
Correct Answer: B
Verified: Yes — 12 & 1 gives 0.
Explanation:
Step 1: Even numbers have last binary bit 0.
Step 2: 12 & 1 gives 0.
Final: Even is printed.
Common Mistake: Thinking & 1 checks divisibility by 1.
Quick Check: What does (n & 1) == 0 usually check?

Q153. What will be the output of the following code?
x = 10

if (x >> 1) == 5:
    print("Half")
else:
    print("Different")

A) Half
B) Different
C) Double
D) Shift Error
Correct Answer: A
Verified: Yes — 10 >> 1 gives 5.
Explanation:
Step 1: Right shift by 1 divides by 2 using integer behavior.
Step 2: 10 >> 1 becomes 5.
Final: Half is printed.
Common Mistake: Thinking >> increases the number.
Quick Check: What is 8 >> 1?

Q154. What will be the output of the following code?
x = 6

if (x << 1) == 12:
    print("Double")
else:
    print("Same")

A) Same
B) Six
C) Double
D) Half
Correct Answer: C
Verified: Yes — 6 << 1 gives 12.
Explanation:
Step 1: Left shift by 1 multiplies by 2.
Step 2: 6 << 1 becomes 12.
Final: Double is printed.
Common Mistake: Confusing left shift with right shift.
Quick Check: What is 5 << 1?

Q155. What will be the output of the following code?
a = 6
b = 3

if (a & b) != 0:
    print("Common Bit")
else:
    print("No Common Bit")

A) No Common Bit
B) Common Bit
C) Equal Values
D) Different Values
Correct Answer: B
Verified: Yes — 6 & 3 gives 2, which is non-zero.
Explanation:
Step 1: 6 is 110 in binary and 3 is 011.
Step 2: 110 & 011 gives 010, which is 2.
Final: Common Bit is printed.
Common Mistake: Thinking a & b must equal 1 to be true.
Quick Check: Is non-zero treated as true in a condition?

Q156. What will be the output of the following code?
a = 8
b = 4

if (a & b) == 0:
    print("No Common Bit")
else:
    print("Common Bit")

A) Common Bit
B) No Common Bit
C) Both Even
D) Both Positive
Correct Answer: B
Verified: Yes — 8 & 4 gives 0.
Explanation:
Step 1: 8 is 1000, and 4 is 0100.
Step 2: There is no common 1 bit.
Final: No Common Bit is printed.
Common Mistake: Thinking both even numbers always share a common bit.
Quick Check: What is 8 & 4?

Q157. What will be the output of the following code?
x = 5
y = 2

if (x | y) == 7:
    print("Bitwise OR Match")
else:
    print("Different")

A) Bitwise OR Match
B) Different
C) Bitwise AND Match
D) Equal
Correct Answer: A
Verified: Yes — 5 | 2 gives 7.
Explanation:
Step 1: 5 is 101, and 2 is 010.
Step 2: 101 | 010 gives 111, which is 7.
Final: Bitwise OR Match is printed.
Common Mistake: Confusing | with or.
Quick Check: What is 4 | 1?

Q158. What will be the output of the following code?
x = 5
y = 1

if (x ^ y) == 4:
    print("XOR Match")
else:
    print("XOR Different")

A) XOR Different
B) Same Bits
C) XOR Match
D) OR Match
Correct Answer: C
Verified: Yes — 5 ^ 1 gives 4.
Explanation:
Step 1: 5 is 101, and 1 is 001.
Step 2: XOR gives 1 only where bits are different.
Final: 101 ^ 001 = 100, which is 4.
Common Mistake: Thinking XOR works like OR.
Quick Check: What is 3 ^ 1?

Q159. What will be the output of the following code?
n = 9

if (n & 1) == 1:
    if n > 5:
        print("Odd and Big")
    else:
        print("Odd and Small")
else:
    print("Even")

A) Odd and Small
B) Even
C) Odd and Big
D) Big Only
Correct Answer: C
Verified: Yes — 9 & 1 is 1, and 9 > 5 is true.
Explanation:
Step 1: (n & 1) == 1 confirms that 9 is odd.
Step 2: The nested condition n > 5 is true.
Final: Odd and Big is printed.
Common Mistake: Checking only odd/even and ignoring the nested condition.
Quick Check: What will happen for n = 3?

Q160. What will be the output of the following code?
n = 14

if (n & 1) == 0:
    if (n >> 1) == 7:
        print("Even Half Seven")
    else:
        print("Even Other")
else:
    print("Odd")

A) Even Other
B) Odd
C) Half Only
D) Even Half Seven
Correct Answer: D
Verified: Yes — 14 & 1 is 0, and 14 >> 1 is 7.
Explanation:
Step 1: 14 is even.
Step 2: Right shift by 1 gives half of 14.
Final: Even Half Seven is printed.
Common Mistake: Thinking 14 >> 1 gives 28.
Quick Check: What is 14 << 1?

Q161. What will be the output of the following code?
x = 3

if (x << 2) == 12:
    if (x & 1) == 1:
        print("Shifted Odd")
    else:
        print("Shifted Even")
else:
    print("Shift Failed")

A) Shifted Even
B) Shifted Odd
C) Shift Failed
D) Odd Only
Correct Answer: B
Verified: Yes — 3 << 2 gives 12, and 3 & 1 gives 1.
Explanation:
Step 1: Left shift by 2 multiplies by 4.
Step 2: 3 << 2 = 12.
Step 3: 3 is odd, so 3 & 1 = 1.
Final: Shifted Odd is printed.
Common Mistake: Thinking left shift by 2 means multiply by 2 only.
Quick Check: What is 4 << 2?

Q162. What will be the output of the following code?
a = 10
b = 6

if (a & b) == 2:
    if (a | b) == 14:
        print("Both Match")
    else:
        print("Only AND Match")
else:
    print("AND Failed")

A) Both Match
B) Only AND Match
C) AND Failed
D) OR Failed
Correct Answer: A
Verified: Yes — 10 & 6 = 2, and 10 | 6 = 14.
Explanation:
Step 1: 10 is 1010, and 6 is 0110.
Step 2: AND gives 0010, which is 2.
Step 3: OR gives 1110, which is 14.
Final: Both Match is printed.
Common Mistake: Mixing the results of & and |.
Quick Check: Which operator keeps only common 1 bits?

Q163. What will be the output of the following code?
a = 12
b = 5

if (a ^ b) == 9:
    if (a & b) == 4:
        print("XOR and AND")
    else:
        print("Only XOR")
else:
    print("XOR Failed")

A) XOR and AND
B) Only XOR
C) XOR Failed
D) AND Only
Correct Answer: A
Verified: Yes — 12 ^ 5 = 9, and 12 & 5 = 4.
Explanation:
Step 1: 12 is 1100, and 5 is 0101.
Step 2: XOR gives 1001, which is 9.
Step 3: AND gives 0100, which is 4.
Final: XOR and AND is printed.
Common Mistake: Thinking XOR and AND give the same result.
Quick Check: What is 12 | 5?

Q164. What will be the output of the following code?
n = 16

if (n >> 2) == 4:
    if (n & 1) == 0:
        print("Quarter Even")
    else:
        print("Quarter Odd")
else:
    print("Shift Failed")

A) Quarter Odd
B) Shift Failed
C) Quarter Even
D) Even Only
Correct Answer: C
Verified: Yes — 16 >> 2 gives 4, and 16 & 1 gives 0.
Explanation:
Step 1: Right shift by 2 divides by 4 using integer behavior.
Step 2: 16 >> 2 = 4.
Step 3: 16 is even.
Final: Quarter Even is printed.
Common Mistake: Thinking right shift by 2 divides by 2 only.
Quick Check: What is 20 >> 2?

Q165. Which condition correctly checks whether n is odd using bitwise AND?
n = 11

if ______:
    print("Odd")
else:
    print("Even")

A) (n & 1) == 1
B) (n | 1) == 1
C) (n ^ 1) == 1
D) (n << 1) == 1
Correct Answer: A
Verified: Yes — odd numbers have last bit 1, so n & 1 gives 1.
Explanation:
Step 1: Bitwise AND with 1 checks the last bit.
Step 2: If the last bit is 1, the number is odd.
Final: Use (n & 1) == 1.
Common Mistake: Using | instead of &.
Quick Check: What does (10 & 1) give?

Q166. Which condition correctly checks whether n is even using bitwise AND?
n = 20

if ______:
    print("Even")
else:
    print("Odd")

A) (n & 1) == 1
B) (n & 1) == 0
C) (n | 1) == 0
D) (n ^ 1) == 0
Correct Answer: B
Verified: Yes — even numbers have last bit 0.
Explanation:
Step 1: n & 1 checks the last bit.
Step 2: For even numbers, the result is 0.
Final: The condition should be (n & 1) == 0.
Common Mistake: Reversing odd and even checks.
Quick Check: Is (15 & 1) equal to 0 or 1?

Q167. What will be the output of the following code?
x = 4
y = 1

if (x | y) == 5:
    if (x ^ y) == 5:
        print("OR and XOR Same")
    else:
        print("Only OR")
else:
    print("OR Failed")

A) Only OR
B) OR Failed
C) OR and XOR Same
D) XOR Failed
Correct Answer: C
Verified: Yes — 4 | 1 is 5, and 4 ^ 1 is also 5.
Explanation:
Step 1: 4 is 100, and 1 is 001.
Step 2: Since there are no common 1 bits, OR and XOR both give 101.
Final: OR and XOR Same is printed.
Common Mistake: Thinking OR and XOR can never give the same answer.
Quick Check: When can OR and XOR give the same result?

Q168. What will be the output of the following code?
x = 7
y = 3

if (x & y) == 3:
    if (x ^ y) == 4:
        print("Common and Different")
    else:
        print("Common Only")
else:
    print("No Common")

A) Common and Different
B) Common Only
C) No Common
D) Different Only
Correct Answer: A
Verified: Yes — 7 & 3 = 3, and 7 ^ 3 = 4.
Explanation:
Step 1: 7 is 111, and 3 is 011.
Step 2: AND gives 011, which is 3.
Step 3: XOR gives 100, which is 4.
Final: Common and Different is printed.
Common Mistake: Thinking XOR keeps common bits.
Quick Check: Which operator keeps different bits?

Q169. What will be the output of the following code?
n = 5

if (n << 1) > 8:
    if (n & 1) == 1:
        print("Odd Double Large")
    else:
        print("Even Double Large")
else:
    print("Double Small")

A) Odd Double Large
B) Even Double Large
C) Double Small
D) Odd Small
Correct Answer: A
Verified: Yes — 5 << 1 gives 10, and 5 & 1 gives 1.
Explanation:
Step 1: 5 << 1 = 10, which is greater than 8.
Step 2: 5 is odd.
Final: Odd Double Large is printed.
Common Mistake: Forgetting that << 1 doubles the number.
Quick Check: What is 6 << 1?

Q170. What will be the output of the following code?
n = 11

if (n >> 1) == 5:
    if (n & 1) == 1:
        print("Odd Half Five")
    else:
        print("Even Half Five")
else:
    print("Half Different")

A) Even Half Five
B) Odd Half Five
C) Half Different
D) Odd Only
Correct Answer: B
Verified: Yes — 11 >> 1 gives 5, and 11 & 1 gives 1.
Explanation:
Step 1: Right shift by 1 gives integer half.
Step 2: 11 >> 1 = 5.
Step 3: 11 is odd.
Final: Odd Half Five is printed.
Common Mistake: Thinking 11 >> 1 gives 5.5.
Quick Check: What is 9 >> 1?
Q171. What will be the output of the following code?
a = 9
b = 5

if (a | b) == 13:
    if (a & b) == 1:
        if (a ^ b) == 12:
            print("All Bitwise Match")
        else:
            print("XOR Failed")
    else:
        print("AND Failed")
else:
    print("OR Failed")

A) OR Failed
B) AND Failed
C) XOR Failed
D) All Bitwise Match
Correct Answer: D
Verified: Yes — 9 | 5 = 13, 9 & 5 = 1, and 9 ^ 5 = 12.
Explanation:
Step 1: 9 is 1001, and 5 is 0101.
Step 2: OR, AND, and XOR checks are all correct.
Final: All Bitwise Match is printed.
Common Mistake: Mixing up |, &, and ^.
Quick Check: Which operator gives 1 only when both bits are 1?

Q172. What will be the output of the following code?
x = 10

if (x & 1) == 0:
    if (x >> 1) == 5:
        if (x << 1) == 20:
            print("Even Shift Match")
        else:
            print("Left Shift Failed")
    else:
        print("Right Shift Failed")
else:
    print("Odd Number")

A) Even Shift Match
B) Left Shift Failed
C) Right Shift Failed
D) Odd Number
Correct Answer: A
Verified: Yes — 10 & 1 = 0, 10 >> 1 = 5, and 10 << 1 = 20.
Explanation:
Step 1: The number is even.
Step 2: Right shift halves it.
Step 3: Left shift doubles it.
Final: All checks pass.
Common Mistake: Reversing << and >>.
Quick Check: Which shift operator doubles the number?

Q173. What will be the output of the following code?
n = 13

if (n & 1) == 1:
    if (n >> 2) == 3:
        if (n % 4) == 1:
            print("Odd Shift Pattern")
        else:
            print("Modulo Failed")
    else:
        print("Shift Failed")
else:
    print("Even Number")

A) Odd Shift Pattern
B) Modulo Failed
C) Shift Failed
D) Even Number
Correct Answer: A
Verified: Yes — 13 & 1 = 1, 13 >> 2 = 3, and 13 % 4 = 1.
Explanation:
Step 1: 13 is odd.
Step 2: Right shift by 2 gives 3.
Step 3: 13 % 4 gives 1.
Final: Odd Shift Pattern is printed.
Common Mistake: Thinking 13 >> 2 gives 6.
Quick Check: What is 12 >> 2?

Q174. What will be the output of the following code?
a = 6
b = 2

if (a & b) == b:
    if (a | b) == a:
        print("b Bits Inside a")
    else:
        print("OR Changed")
else:
    print("AND Failed")

A) b Bits Inside a
B) OR Changed
C) AND Failed
D) Bits Different
Correct Answer: A
Verified: Yes — 6 & 2 = 2, and 6 | 2 = 6.
Explanation:
Step 1: 6 is 110, and 2 is 010.
Step 2: All 1 bits of 2 are already present in 6.
Final: b Bits Inside a is printed.
Common Mistake: Thinking OR always changes the number.
Quick Check: What happens when you OR a number with a bit it already has?

Q175. What will be the output of the following code?
a = 4
b = 2

if (a & b) == b:
    print("Inside")
else:
    if (a | b) == 6:
        print("OR Added")
    else:
        print("No Match")

A) Inside
B) OR Added
C) No Match
D) AND Added
Correct Answer: B
Verified: Yes — 4 & 2 = 0, so outer if fails; 4 | 2 = 6.
Explanation:
Step 1: 4 is 100, and 2 is 010.
Step 2: AND gives 0, so the outer condition fails.
Step 3: OR gives 110, which is 6.
Final: OR Added is printed.
Common Mistake: Thinking 4 & 2 gives 6.
Quick Check: Which operator combines bits: & or |?

Q176. What will be the output of the following code?
x = 15

if (x & 1) == 1:
    if (x >> 1) == 7:
        if (x & 7) == 7:
            print("Odd Seven Pattern")
        else:
            print("Last Three Bits Failed")
    else:
        print("Shift Failed")
else:
    print("Even")

A) Odd Seven Pattern
B) Last Three Bits Failed
C) Shift Failed
D) Even
Correct Answer: A
Verified: Yes — 15 & 1 = 1, 15 >> 1 = 7, and 15 & 7 = 7.
Explanation:
Step 1: 15 is odd.
Step 2: 15 >> 1 gives 7.
Step 3: 15 & 7 keeps the last three bits, giving 7.
Final: Odd Seven Pattern is printed.
Common Mistake: Thinking x & 7 checks divisibility by 7.
Quick Check: What is 14 & 1?

Q177. What will be the output of the following code?
x = 8

if (x >> 2) == 2:
    if (x << 1) == 16:
        if (x & 1) == 0:
            print("Shift Even")
        else:
            print("Shift Odd")
    else:
        print("Left Shift Failed")
else:
    print("Right Shift Failed")

A) Shift Odd
B) Right Shift Failed
C) Shift Even
D) Left Shift Failed
Correct Answer: C
Verified: Yes — 8 >> 2 = 2, 8 << 1 = 16, and 8 & 1 = 0.
Explanation:
Step 1: Right shift by 2 divides 8 by 4.
Step 2: Left shift by 1 doubles 8.
Step 3: 8 is even.
Final: Shift Even is printed.
Common Mistake: Thinking shifting changes the original variable permanently.
Quick Check: Does x << 1 change x itself?

Q178. What will be the output of the following code?
a = 7
b = 4

if (a & b) == 4:
    if (a ^ b) == 3:
        print("Split Bits")
    else:
        print("XOR Failed")
else:
    print("AND Failed")

A) Split Bits
B) XOR Failed
C) AND Failed
D) OR Failed
Correct Answer: A
Verified: Yes — 7 & 4 = 4, and 7 ^ 4 = 3.
Explanation:
Step 1: 7 is 111, and 4 is 100.
Step 2: AND gives 100, which is 4.
Step 3: XOR gives 011, which is 3.
Final: Split Bits is printed.
Common Mistake: Thinking XOR keeps common bits.
Quick Check: What is 7 | 4?

Q179. What will be the output of the following code?
n = 20

if (n >> 2) == 5:
    if (n & 3) == 0:
        print("Multiple of Four Pattern")
    else:
        print("Remainder Bits Found")
else:
    print("Shift Not Five")

A) Shift Not Five
B) Remainder Bits Found
C) Multiple of Four Pattern
D) Five Only
Correct Answer: C
Verified: Yes — 20 >> 2 = 5, and 20 & 3 = 0.
Explanation:
Step 1: 20 >> 2 gives 5.
Step 2: n & 3 checks the last two bits.
Step 3: Last two bits are 00, so result is 0.
Final: Multiple of Four Pattern is printed.
Common Mistake: Thinking n & 3 means n % 3.
Quick Check: What is 18 & 3?

Q180. What will be the output of the following code?
a = 5
b = 6

if (a & b) == 4:
    if (a | b) == 7:
        if (a ^ b) == 3:
            print("All Operators")
        else:
            print("XOR Failed")
    else:
        print("OR Failed")
else:
    print("AND Failed")

A) AND Failed
B) OR Failed
C) XOR Failed
D) All Operators
Correct Answer: D
Verified: Yes — 5 & 6 = 4, 5 | 6 = 7, and 5 ^ 6 = 3.
Explanation:
Step 1: 5 is 101, and 6 is 110.
Step 2: AND, OR, and XOR all match their expected values.
Final: All Operators is printed.
Common Mistake: Confusing OR and XOR results.
Quick Check: Which operator gives 1 when bits are different?

Q181. What will be the output of the following code?
n = 32

if (n >> 3) == 4:
    if (n << 1) == 64:
        print("Shift Pair")
    else:
        print("Left Shift Failed")
else:
    print("Right Shift Failed")

A) Shift Pair
B) Left Shift Failed
C) Right Shift Failed
D) Pair Failed
Correct Answer: A
Verified: Yes — 32 >> 3 = 4, and 32 << 1 = 64.
Explanation:
Step 1: Right shift by 3 divides by 8.
Step 2: Left shift by 1 multiplies by 2.
Final: Shift Pair is printed.
Common Mistake: Thinking >> 3 means subtract 3.
Quick Check: What is 16 >> 3?

Q182. What will be the output of the following code?
x = 2

if (x << 3) == 16:
    if (x | 1) == 3:
        print("Shift OR Match")
    else:
        print("OR Failed")
else:
    print("Shift Failed")

A) Shift Failed
B) OR Failed
C) Shift OR Match
D) Shift Only
Correct Answer: C
Verified: Yes — 2 << 3 = 16, and 2 | 1 = 3.
Explanation:
Step 1: Left shift by 3 multiplies by 8.
Step 2: 2 | 1 turns on the last bit.
Final: Shift OR Match is printed.
Common Mistake: Thinking left shift by 3 multiplies only by 3.
Quick Check: What is 3 << 2?

Q183. What will be the output of the following code?
x = 9

if (x & 1) == 1:
    if (x | 2) == 11:
        print("Odd OR Match")
    else:
        print("OR Failed")
else:
    print("Even")

A) Even
B) Odd OR Match
C) OR Failed
D) Odd Only
Correct Answer: B
Verified: Yes — 9 & 1 = 1, and 9 | 2 = 11.
Explanation:
Step 1: 9 is odd.
Step 2: 9 | 2 gives 11.
Final: Odd OR Match is printed.
Common Mistake: Thinking OR only works with Boolean values.
Quick Check: What is 8 | 2?

Q184. What will be the output of the following code?
a = 14
b = 7

if (a >> 1) == b:
    if (a & b) == 6:
        print("Shift and AND")
    else:
        print("Only Shift")
else:
    print("Shift Failed")

A) Shift and AND
B) Only Shift
C) Shift Failed
D) AND Only
Correct Answer: A
Verified: Yes — 14 >> 1 = 7, and 14 & 7 = 6.
Explanation:
Step 1: 14 >> 1 gives 7.
Step 2: 14 & 7 gives 6.
Final: Shift and AND is printed.
Common Mistake: Assuming a & b must equal either a or b.
Quick Check: What is 14 | 7?

Q185. What will be the output of the following code?
n = 6

if (n ^ 1) == 7:
    if (n & 1) == 0:
        print("Even Toggled")
    else:
        print("Odd Toggled")
else:
    print("Toggle Failed")

A) Even Toggled
B) Odd Toggled
C) Toggle Failed
D) Even Only
Correct Answer: A
Verified: Yes — 6 ^ 1 = 7, and 6 & 1 = 0.
Explanation:
Step 1: XOR with 1 toggles the last bit.
Step 2: 6 is even.
Final: Even Toggled is printed.
Common Mistake: Thinking ^ means power in Python.
Quick Check: Is ^ exponentiation in Python?

Q186. What will be the output of the following code?
n = 7

if (n ^ 1) == 6:
    if (n & 1) == 1:
        print("Odd Toggled")
    else:
        print("Even Toggled")
else:
    print("Toggle Failed")

A) Toggle Failed
B) Even Toggled
C) Odd Toggled
D) Odd Only
Correct Answer: C
Verified: Yes — 7 ^ 1 = 6, and 7 & 1 = 1.
Explanation:
Step 1: XOR with 1 toggles the last bit.
Step 2: 7 is odd.
Final: Odd Toggled is printed.
Common Mistake: Thinking 7 ^ 1 means 7 raised to power 1.
Quick Check: Which Python operator is used for power?

Q187. What will be the output of the following code?
x = 4

if (x << 1) == 8:
    if (x >> 1) == 2:
        if (x | 1) == 5:
            print("Three Checks")
        else:
            print("OR Failed")
    else:
        print("Right Shift Failed")
else:
    print("Left Shift Failed")

A) Three Checks
B) OR Failed
C) Right Shift Failed
D) Left Shift Failed
Correct Answer: A
Verified: Yes — 4 << 1 = 8, 4 >> 1 = 2, and 4 | 1 = 5.
Explanation:
Step 1: Left shift doubles the number.
Step 2: Right shift halves the number.
Step 3: OR with 1 sets the last bit.
Final: Three Checks is printed.
Common Mistake: Thinking shifting changes the original x.
Quick Check: After checking x << 1, is x still 4?

Q188. What will be the output of the following code?
a = 10
b = 3

if (a & b) == 2:
    if (a | b) == 11:
        if (a ^ b) == 9:
            print("Bitwise Trio")
        else:
            print("XOR Failed")
    else:
        print("OR Failed")
else:
    print("AND Failed")

A) Bitwise Trio
B) XOR Failed
C) OR Failed
D) AND Failed
Correct Answer: A
Verified: Yes — 10 & 3 = 2, 10 | 3 = 11, and 10 ^ 3 = 9.
Explanation:
Step 1: 10 is 1010, and 3 is 0011.
Step 2: AND, OR, and XOR results all match.
Final: Bitwise Trio is printed.
Common Mistake: Mixing OR result with XOR result.
Quick Check: What is 10 | 3?

Q189. What will be the output of the following code?
n = 12

if (n & 3) == 0:
    if (n >> 2) == 3:
        print("Divisible by Four Pattern")
    else:
        print("Shift Failed")
else:
    print("Last Bits Not Zero")

A) Shift Failed
B) Last Bits Not Zero
C) Divisible by Four Pattern
D) Four Only
Correct Answer: C
Verified: Yes — 12 & 3 = 0, and 12 >> 2 = 3.
Explanation:
Step 1: (n & 3) == 0 checks whether the last two bits are zero.
Step 2: For 12, this is true.
Step 3: 12 >> 2 gives 3.
Final: Divisible by Four Pattern is printed.
Common Mistake: Thinking n & 3 is the same as n % 3.
Quick Check: What is 16 & 3?

Q190. What will be the output of the following code?
x = 5

if (~x) == -6:
    if (x & 1) == 1:
        print("Complement Odd")
    else:
        print("Complement Even")
else:
    print("Complement Failed")

A) Complement Odd
B) Complement Even
C) Complement Failed
D) Odd Only
Correct Answer: A
Verified: Yes — in Python, ~5 is -6, and 5 & 1 is 1.
Explanation:
Step 1: Bitwise NOT follows the rule ~x = -(x + 1).
Step 2: So ~5 = -6.
Step 3: 5 is odd.
Final: Complement Odd is printed.
Common Mistake: Thinking ~5 gives positive 5 or 0.
Quick Check: What is ~3 in Python?

Q191. What will be the output of the following code?
n = 18

if (n & 1) == 0:
    if (n >> 1) == 9:
        if n + 6 == (n << 1):
            print("Full Match")
        else:
            print("Half Match")
    else:
        print("Shift Failed")
else:
    print("Odd Number")

A) Full Match
B) Half Match
C) Shift Failed
D) Odd Number
Correct Answer: B
Verified: Yes — 18 & 1 = 0, 18 >> 1 = 9, but 18 + 6 != 18 << 1.
Explanation:
Step 1: 18 is even, so the first condition is true.
Step 2: 18 >> 1 gives 9.
Step 3: 18 + 6 = 24, but 18 << 1 = 36.
Final: Half Match is printed.
Common Mistake: Thinking << 1 adds 1 instead of doubling.
Quick Check: What is 10 << 1?

Q192. What will be the output of the following code?
a = 10
b = 6

if (a & b) == 2:
    if (a | b) + 2 == 16:
        if (a ^ b) * 2 == 24:
            print("Full Pattern")
        else:
            print("XOR Failed")
    else:
        print("OR Failed")
else:
    print("AND Failed")

A) AND Failed
B) OR Failed
C) XOR Failed
D) Full Pattern
Correct Answer: D
Verified: Yes — 10 & 6 = 2, 10 | 6 = 14, and 10 ^ 6 = 12.
Explanation:
Step 1: 10 & 6 gives 2.
Step 2: (10 | 6) + 2 becomes 14 + 2 = 16.
Step 3: (10 ^ 6) * 2 becomes 12 * 2 = 24.
Final: Full Pattern is printed.
Common Mistake: Confusing | and ^.
Quick Check: Which operator gives 1 when bits are different?

Q193. What will be the output of the following code?
n = 21

if (n & 1) == 1:
    if (n & 3) == 1:
        if n // 3 == 7:
            print("Odd Remainder Pattern")
        else:
            print("Division Failed")
    else:
        print("Bit Pattern Failed")
else:
    print("Even Number")

A) Odd Remainder Pattern
B) Division Failed
C) Bit Pattern Failed
D) Even Number
Correct Answer: A
Verified: Yes — 21 & 1 = 1, 21 & 3 = 1, and 21 // 3 = 7.
Explanation:
Step 1: 21 is odd.
Step 2: 21 & 3 checks the last two bits and gives 1.
Step 3: 21 // 3 gives 7.
Final: Odd Remainder Pattern is printed.
Common Mistake: Thinking n & 3 is the same as n % 3.
Quick Check: What is 20 & 3?

Q194. What will be the output of the following code?
x = 12
y = 5

if (x | y) == 13:
    if (x & y) == 4:
        if x - y * 2 > 0:
            print("Bitwise Maths OK")
        else:
            print("Math Failed")
    else:
        print("AND Failed")
else:
    print("OR Failed")

A) OR Failed
B) AND Failed
C) Bitwise Maths OK
D) Math Failed
Correct Answer: C
Verified: Yes — 12 | 5 = 13, 12 & 5 = 4, and 12 - 5 * 2 = 2.
Explanation:
Step 1: OR condition is true.
Step 2: AND condition is also true.
Step 3: Multiplication happens before subtraction, so 12 - 10 = 2.
Final: Bitwise Maths OK is printed.
Common Mistake: Calculating x - y * 2 as (x - y) * 2.
Quick Check: What is 12 - 5 * 2?

Q195. What will be the output of the following code?
n = 24

if (n >> 3) == 3:
    if (n & 7) == 0:
        if n + 8 == (n << 1):
            print("Full Shift Pattern")
        else:
            print("Shift Pattern Partial")
    else:
        print("Last Bits Failed")
else:
    print("Right Shift Failed")

A) Full Shift Pattern
B) Shift Pattern Partial
C) Last Bits Failed
D) Right Shift Failed
Correct Answer: B
Verified: Yes — 24 >> 3 = 3, 24 & 7 = 0, but 24 + 8 != 24 << 1.
Explanation:
Step 1: 24 >> 3 gives 3.
Step 2: 24 & 7 gives 0.
Step 3: 24 + 8 = 32, but 24 << 1 = 48.
Final: Shift Pattern Partial is printed.
Common Mistake: Thinking left shift by 1 adds 8.
Quick Check: What is 24 << 1?

Q196. What will be the output of the following code?
a = 7
b = 2

if (a ^ b) == 5:
    if a + b * 2 == 11:
        if (a & b) == 2:
            print("XOR Math Common")
        else:
            print("AND Failed")
    else:
        print("Math Failed")
else:
    print("XOR Failed")

A) XOR Failed
B) Math Failed
C) AND Failed
D) XOR Math Common
Correct Answer: D
Verified: Yes — 7 ^ 2 = 5, 7 + 2 * 2 = 11, and 7 & 2 = 2.
Explanation:
Step 1: XOR condition is true.
Step 2: Multiplication happens before addition.
Step 3: AND condition is true.
Final: XOR Math Common is printed.
Common Mistake: Thinking ^ means power.
Quick Check: Which operator is used for power in Python?

Q197. What will be the output of the following code?
n = 30

if (n & 1) == 0:
    if (n >> 1) == 15:
        if (n & 3) == 2:
            print("Even Half Remainder")
        else:
            print("Last Bits Different")
    else:
        print("Half Failed")
else:
    print("Odd Number")

A) Even Half Remainder
B) Last Bits Different
C) Half Failed
D) Odd Number
Correct Answer: A
Verified: Yes — 30 & 1 = 0, 30 >> 1 = 15, and 30 & 3 = 2.
Explanation:
Step 1: 30 is even.
Step 2: Right shift gives 15.
Step 3: 30 & 3 gives 2.
Final: Even Half Remainder is printed.
Common Mistake: Thinking n & 3 means divide by 3.
Quick Check: What is 30 % 4?

Q198. What will be the output of the following code?
x = 9

if (x << 1) == 18:
    if (x | 4) == 13:
        if x % 4 == 1:
            print("Shift OR Mod")
        else:
            print("Modulo Failed")
    else:
        print("OR Failed")
else:
    print("Shift Failed")

A) Shift Failed
B) OR Failed
C) Shift OR Mod
D) Modulo Failed
Correct Answer: C
Verified: Yes — 9 << 1 = 18, 9 | 4 = 13, and 9 % 4 = 1.
Explanation:
Step 1: Left shift doubles 9.
Step 2: Bitwise OR with 4 gives 13.
Step 3: 9 % 4 gives 1.
Final: Shift OR Mod is printed.
Common Mistake: Confusing | with logical or.
Quick Check: What is 8 | 4?

Q199. What will be the output of the following code?
a = 14
b = 3

if (a & b) == 2:
    if a // b == 4:
        if (a ^ b) == 13:
            print("All Checks")
        else:
            print("XOR Failed")
    else:
        print("Division Failed")
else:
    print("AND Failed")

A) Division Failed
B) All Checks
C) XOR Failed
D) AND Failed
Correct Answer: B
Verified: Yes — 14 & 3 = 2, 14 // 3 = 4, and 14 ^ 3 = 13.
Explanation:
Step 1: AND condition is true.
Step 2: Integer division gives 4.
Step 3: XOR gives 13.
Final: All Checks is printed.
Common Mistake: Using normal division / instead of integer division //.
Quick Check: What is 14 / 3 approximately?

Q200. What will be the output of the following code?
n = 11

if (n & 1) == 1:
    if (n << 1) - n == 11:
        if (n >> 1) + (n & 1) == 6:
            print("Odd Shift Balance")
        else:
            print("Balance Failed")
    else:
        print("Shift Difference Failed")
else:
    print("Even Number")

A) Balance Failed
B) Shift Difference Failed
C) Even Number
D) Odd Shift Balance
Correct Answer: D
Verified: Yes — 11 is odd, 22 - 11 = 11, and 5 + 1 = 6.
Explanation:
Step 1: 11 & 1 = 1, so the number is odd.
Step 2: 11 << 1 gives 22.
Step 3: 11 >> 1 gives 5, and 11 & 1 gives 1.
Final: Odd Shift Balance is printed.
Common Mistake: Thinking 11 >> 1 gives 5.5.
Quick Check: What is 13 >> 1?

Q201. What will be the output of the following code?
n = 16

if (n & 1) == 0:
    if (n >> 2) == 4:
        if (n | 3) == 19:
            print("Even OR Pattern")
        else:
            print("OR Failed")
    else:
        print("Shift Failed")
else:
    print("Odd Number")

A) Even OR Pattern
B) OR Failed
C) Shift Failed
D) Odd Number
Correct Answer: A
Verified: Yes — 16 & 1 = 0, 16 >> 2 = 4, and 16 | 3 = 19.
Explanation:
Step 1: 16 is even.
Step 2: Right shift by 2 gives 4.
Step 3: OR with 3 gives 19.
Final: Even OR Pattern is printed.
Common Mistake: Thinking 16 | 3 gives 16 + 3 by arithmetic addition.
Quick Check: What is 8 | 1?

Q202. What will be the output of the following code?
a = 5
b = 12

if (a | b) == 13:
    if (a & b) == 4:
        if b - a == (a ^ b) - 6:
            print("Difference Match")
        else:
            print("Difference Failed")
    else:
        print("AND Failed")
else:
    print("OR Failed")

A) Difference Match
B) AND Failed
C) Difference Failed
D) OR Failed
Correct Answer: C
Verified: Yes — 5 | 12 = 13, 5 & 12 = 4, but 12 - 5 != (5 ^ 12) - 6.
Explanation:
Step 1: OR and AND checks are true.
Step 2: 12 - 5 = 7.
Step 3: 5 ^ 12 = 9, and 9 - 6 = 3.
Final: Difference Failed is printed.
Common Mistake: Assuming the third condition is true because the first two are true.
Quick Check: What is 5 ^ 12?

Q203. What will be the output of the following code?
x = 6
y = 9

if (x & y) == 0:
    if x + y == 15:
        if (x | y) == 15:
            print("Disjoint Bits Sum")
        else:
            print("OR Failed")
    else:
        print("Sum Failed")
else:
    print("Common Bits")

A) Common Bits
B) Disjoint Bits Sum
C) Sum Failed
D) OR Failed
Correct Answer: B
Verified: Yes — 6 & 9 = 0, 6 + 9 = 15, and 6 | 9 = 15.
Explanation:
Step 1: 6 and 9 have no common 1 bits.
Step 2: Their sum is 15.
Step 3: Their OR is also 15.
Final: Disjoint Bits Sum is printed.
Common Mistake: Thinking & always gives a positive value for positive numbers.
Quick Check: What is 4 & 2?

Q204. What will be the output of the following code?
n = 27

if (n & 1) == 1:
    if (n >> 1) == 13:
        if n % 5 == (n & 3):
            print("Final Match")
        else:
            print("Last Check Failed")
    else:
        print("Shift Failed")
else:
    print("Even Number")

A) Final Match
B) Shift Failed
C) Even Number
D) Last Check Failed
Correct Answer: D
Verified: Yes — 27 is odd, 27 >> 1 = 13, but 27 % 5 is not equal to 27 & 3.
Explanation:
Step 1: 27 & 1 = 1.
Step 2: 27 >> 1 = 13.
Step 3: 27 % 5 = 2, but 27 & 3 = 3.
Final: Last Check Failed is printed.
Common Mistake: Thinking % and & always give the same result for small values.
Quick Check: What is 27 & 3?

Q205. What will be the output of the following code?
a = 8
b = 2
c = 1

if (a >> b) == 2:
    if (a | c) == 9:
        if (a & c) == 0:
            print("Shift OR No Common")
        else:
            print("Common Bit Found")
    else:
        print("OR Failed")
else:
    print("Shift Failed")

A) Shift OR No Common
B) Common Bit Found
C) OR Failed
D) Shift Failed
Correct Answer: A
Verified: Yes — 8 >> 2 = 2, 8 | 1 = 9, and 8 & 1 = 0.
Explanation:
Step 1: Right shift condition is true.
Step 2: OR with 1 gives 9.
Step 3: AND with 1 gives 0.
Final: Shift OR No Common is printed.
Common Mistake: Thinking 8 & 1 is 1 because both numbers are positive.
Quick Check: Is 8 odd or even?

Q206. What will be the output of the following code?
n = 31

if (n & 15) == 15:
    if (n >> 4) == 1:
        if (n ^ 15) == 16:
            print("Last Four Bits")
        else:
            print("XOR Failed")
    else:
        print("Shift Failed")
else:
    print("Bit Mask Failed")

A) Bit Mask Failed
B) Shift Failed
C) Last Four Bits
D) XOR Failed
Correct Answer: C
Verified: Yes — 31 & 15 = 15, 31 >> 4 = 1, and 31 ^ 15 = 16.
Explanation:
Step 1: n & 15 checks the last four bits.
Step 2: 31 >> 4 gives 1.
Step 3: XOR with 15 gives 16.
Final: Last Four Bits is printed.
Common Mistake: Thinking & 15 checks divisibility by 15.
Quick Check: What is 16 & 15?

Q207. What will be the output of the following code?
x = 18

if (x & 3) == 2:
    if x // 3 == 6:
        if (x >> 1) == x - 9:
            print("Remainder and Half")
        else:
            print("Half Failed")
    else:
        print("Division Failed")
else:
    print("Bit Check Failed")

A) Half Failed
B) Remainder and Half
C) Division Failed
D) Bit Check Failed
Correct Answer: B
Verified: Yes — 18 & 3 = 2, 18 // 3 = 6, and 18 >> 1 = 9.
Explanation:
Step 1: The bit check gives 2.
Step 2: Integer division gives 6.
Step 3: 18 >> 1 = 9, and 18 - 9 = 9.
Final: Remainder and Half is printed.
Common Mistake: Thinking x >> 1 changes the value of x.
Quick Check: After x >> 1, what is the original value of x?

Q208. What will be the output of the following code?
a = 9
b = 6

if (a | b) == 15:
    if (a & b) == 0:
        if a + b == (a | b):
            print("OR Equals Sum")
        else:
            print("Sum Failed")
    else:
        print("Common Bits")
else:
    print("OR Failed")

A) OR Failed
B) Common Bits
C) Sum Failed
D) OR Equals Sum
Correct Answer: D
Verified: Yes — 9 | 6 = 15, 9 & 6 = 0, and 9 + 6 = 15.
Explanation:
Step 1: OR gives 15.
Step 2: AND gives 0, meaning there are no common 1 bits.
Step 3: Since there are no common bits, the OR equals the arithmetic sum here.
Final: OR Equals Sum is printed.
Common Mistake: Thinking OR always equals addition.
Quick Check: Does 5 | 3 equal 5 + 3?

Q209. What will be the output of the following code?
n = 20

if (n & 1) == 0:
    if (n << 1) == 40:
        if (n | 3) == 23:
            print("Even Shift OR")
        else:
            print("OR Failed")
    else:
        print("Shift Failed")
else:
    print("Odd Number")

A) Even Shift OR
B) OR Failed
C) Shift Failed
D) Odd Number
Correct Answer: A
Verified: Yes — 20 & 1 = 0, 20 << 1 = 40, and 20 | 3 = 23.
Explanation:
Step 1: 20 is even.
Step 2: Left shift doubles it.
Step 3: OR with 3 gives 23.
Final: Even Shift OR is printed.
Common Mistake: Thinking 20 | 3 gives 20 only.
Quick Check: What is 20 | 1?

Q210. What will be the output of the following code?
a = 13
b = 5

if (a ^ b) == 8:
    if (a & b) == 5:
        if a + b > (a | b):
            print("XOR With Common")
        else:
            print("Sum Not Greater")
    else:
        print("AND Failed")
else:
    print("XOR Failed")

A) XOR Failed
B) AND Failed
C) XOR With Common
D) Sum Not Greater
Correct Answer: C
Verified: Yes — 13 ^ 5 = 8, 13 & 5 = 5, and 18 > 13.
Explanation:
Step 1: XOR gives 8.
Step 2: AND gives 5.
Step 3: a + b is 18, while a | b is 13.
Final: XOR With Common is printed.
Common Mistake: Thinking a | b is always greater than a + b.
Quick Check: What is 13 | 5?

Q211. What will be the output of the following code?
n = 10

if (n & 1) == 0:
    if (n >> 1) + (n & 3) == 7:
        if (n << 1) - 5 == 15:
            print("Compound Shift")
        else:
            print("Final Maths Failed")
    else:
        print("Middle Check Failed")
else:
    print("Odd Number")

A) Middle Check Failed
B) Compound Shift
C) Final Maths Failed
D) Odd Number
Correct Answer: B
Verified: Yes — 10 is even, 10 >> 1 = 5, 10 & 3 = 2, and 20 - 5 = 15.
Explanation:
Step 1: First condition confirms even number.
Step 2: (n >> 1) + (n & 3) becomes 5 + 2 = 7.
Step 3: (n << 1) - 5 becomes 20 - 5 = 15.
Final: Compound Shift is printed.
Common Mistake: Confusing & 3 with % 3.
Quick Check: What is 10 % 4?

Q212. What will be the output of the following code?
x = 4
y = 7

if (x | y) == 7:
    if (x & y) == 4:
        if y - x == x - 1:
            print("Bits Included")
        else:
            print("Math Failed")
    else:
        print("AND Failed")
else:
    print("OR Failed")

A) OR Failed
B) AND Failed
C) Math Failed
D) Bits Included
Correct Answer: D
Verified: Yes — 4 | 7 = 7, 4 & 7 = 4, and 7 - 4 = 4 - 1.
Explanation:
Step 1: OR condition is true.
Step 2: AND condition is true.
Step 3: Both sides of the maths comparison are 3.
Final: Bits Included is printed.
Common Mistake: Thinking x | y must always be greater than both numbers.
Quick Check: What is 4 | 7?

Q213. What will be the output of the following code?
n = 6

if (n ^ 1) == 7:
    if ((n + 2) << 1) == 16:
        if (n & 1) == 0:
            print("Toggle Even")
        else:
            print("Toggle Odd")
    else:
        print("Shift Maths Failed")
else:
    print("Toggle Failed")

A) Toggle Even
B) Toggle Odd
C) Shift Maths Failed
D) Toggle Failed
Correct Answer: A
Verified: Yes — 6 ^ 1 = 7, (6 + 2) << 1 = 16, and 6 & 1 = 0.
Explanation:
Step 1: XOR with 1 toggles the last bit.
Step 2: (n + 2) becomes 8, and 8 << 1 gives 16.
Step 3: 6 is even.
Final: Toggle Even is printed.
Common Mistake: Thinking ^ means exponentiation.
Quick Check: What is the exponent operator in Python?

Q214. What will be the output of the following code?
a = 15
b = 8

if (a & b) == 8:
    if (a >> 1) == 7:
        if (a ^ b) + 1 == 8:
            print("High Bit Pattern")
        else:
            print("XOR Maths Failed")
    else:
        print("Shift Failed")
else:
    print("AND Failed")

A) AND Failed
B) Shift Failed
C) High Bit Pattern
D) XOR Maths Failed
Correct Answer: C
Verified: Yes — 15 & 8 = 8, 15 >> 1 = 7, and (15 ^ 8) + 1 = 8.
Explanation:
Step 1: AND confirms that the 8 bit is present.
Step 2: Right shift gives 7.
Step 3: 15 ^ 8 = 7, and 7 + 1 = 8.
Final: High Bit Pattern is printed.
Common Mistake: Thinking XOR keeps common bits.
Quick Check: What is 15 ^ 8?

Q215. What will be the output of the following code?
n = 32

if (n >> 5) == 1:
    if (n & 31) == 0:
        if (n | 7) == 39:
            print("Power Bit Pattern")
        else:
            print("OR Failed")
    else:
        print("Lower Bits Found")
else:
    print("Shift Failed")

A) Shift Failed
B) Power Bit Pattern
C) Lower Bits Found
D) OR Failed
Correct Answer: B
Verified: Yes — 32 >> 5 = 1, 32 & 31 = 0, and 32 | 7 = 39.
Explanation:
Step 1: Right shift by 5 reduces 32 to 1.
Step 2: 32 & 31 gives 0, meaning lower five bits are zero.
Step 3: 32 | 7 gives 39.
Final: Power Bit Pattern is printed.
Common Mistake: Thinking & 31 checks divisibility by 31.
Quick Check: What is 16 & 15?