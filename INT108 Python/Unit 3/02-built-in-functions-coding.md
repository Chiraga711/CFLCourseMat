# Built-in Functions — Coding Problems (1–15)

*Unit 3 · Topic 02. Every problem uses only built-in functions plus your loops and conditionals knowledge — no `def` needed (that starts in Topic 03). Every solution was verified by execution.*

---

**Problem 1.** Read three integers, one per line. Print the largest using `max()`.

Sample input:
```
14
9
23
```
Sample output:
```
23
```

<details>
<summary>Solution</summary>

```python
a = int(input())
b = int(input())
c = int(input())
print(max(a, b, c))
```
</details>

---

**Problem 2.** Read a float. Print it rounded to 1 decimal place using `round()`.

Sample input:
```
7.46
```
Sample output:
```
7.5
```

<details>
<summary>Solution</summary>

```python
x = float(input())
print(round(x, 1))
```
</details>

---

**Problem 3.** Read an integer. Print how many digits it has — **without a loop**, using `len()` and `str()`.

Sample input:
```
45072
```
Sample output:
```
5
```

<details>
<summary>Solution</summary>

```python
n = int(input())
print(len(str(n)))
```

Compare with your digit-count loop from the loops unit — five lines became one. That's what built-ins are for.
</details>

---

**Problem 4.** Read two floats, one per line. Print the smaller one using `min()`.

Sample input:
```
3.7
3.25
```
Sample output:
```
3.25
```

<details>
<summary>Solution</summary>

```python
a = float(input())
b = float(input())
print(min(a, b))
```
</details>

---

**Problem 5.** Read an integer. Print it as a float (so `7` prints as `7.0`).

Sample input:
```
7
```
Sample output:
```
7.0
```

<details>
<summary>Solution</summary>

```python
n = int(input())
print(float(n))
```
</details>

---

**Problem 6.** A price arrives as a float, like `45.75`. Print the rupees and the paise as two integers separated by a space.

Sample input:
```
45.75
```
Sample output:
```
45 75
```

<details>
<summary>Solution</summary>

```python
x = float(input())
r = int(x)
p = round(x * 100) % 100
print(r, p)
```

`int(x)` cuts off the paise; `round(x * 100)` turns the whole price into paise safely (avoiding float noise), and `% 100` keeps just the paise part.
</details>

---

**Problem 7.** Read four integers, one per line. Print their total using `sum()`.

Sample input:
```
5
12
8
20
```
Sample output:
```
45
```

<details>
<summary>Solution</summary>

```python
a = int(input())
b = int(input())
c = int(input())
d = int(input())
print(sum([a, b, c, d]))
```

Note the square brackets — `sum()` needs its numbers inside a list.
</details>

---

**Problem 8.** Read a float. Print `int()` of it and `round()` of it, separated by a space — see the difference on the same number.

Sample input:
```
8.6
```
Sample output:
```
8 9
```

<details>
<summary>Solution</summary>

```python
x = float(input())
print(int(x), round(x))
```

`int()` cuts (8), `round()` rounds (9). Two different questions, two different answers.
</details>

---

**Problem 9.** Read three floats, one per line. Print the largest, rounded to 2 decimal places.

Sample input:
```
4.518
4.526
4.52
```
Sample output:
```
4.53
```

<details>
<summary>Solution</summary>

```python
a = float(input())
b = float(input())
c = float(input())
print(round(max(a, b, c), 2))
```

Functions nest: `max` picks 4.526, then `round` trims it to 4.53.
</details>

---

**Problem 10.** Read one line with `input()` but do **not** convert it. Print how many characters the user typed.

Sample input:
```
4507
```
Sample output:
```
4
```

<details>
<summary>Solution</summary>

```python
t = input()
print(len(t))
```

No `int()` anywhere — `input()` already gives a string, and strings have a length. This works even if the user types letters.
</details>

---

**Problem 11.** Read a float. Print it two ways, on two lines: first with `round(x, 2)`, then with `f"{x:.2f}"`. Try it with `5.5` and study the difference.

Sample input:
```
5.5
```
Sample output:
```
5.5
5.50
```

<details>
<summary>Solution</summary>

```python
x = float(input())
print(round(x, 2))
print(f"{x:.2f}")
```

The lesson in one run: `round()` gives a *number*, and numbers don't keep trailing zeros — `f"{x:.2f}"` gives *text* padded to exactly two places. For money displays, the f-string is the right tool.
</details>

---

**Problem 12.** Read two integers. Print their difference as a positive number — using only `max()` and `min()`.

Sample input:
```
9
23
```
Sample output:
```
14
```

<details>
<summary>Solution</summary>

```python
a = int(input())
b = int(input())
print(max(a, b) - min(a, b))
```

Bigger minus smaller is never negative — no `if` needed.
</details>

---

**Problem 13.** Read an integer. Print `1` if it is a 3-digit number, otherwise print `0`. Use `len()` and `str()` instead of comparing against 100 and 999.

Sample input:
```
457
```
Sample output:
```
1
```

Second sample — input `45` → output `0`.

<details>
<summary>Solution</summary>

```python
n = int(input())
if len(str(n)) == 3:
    print(1)
else:
    print(0)
```
</details>

---

**Problem 14.** Read three integers (marks out of 10). Print their average rounded to 2 decimal places.

Sample input:
```
7
8
8
```
Sample output:
```
7.67
```

<details>
<summary>Solution</summary>

```python
a = int(input())
b = int(input())
c = int(input())
print(round(sum([a, b, c]) / 3, 2))
```

Three built-ins in one line: `sum` totals, `/` averages, `round` trims.
</details>

---

**Problem 15.** Read an integer `n`. Print the type of `n`, the type of `float(n)`, and the type of `str(n)` — three lines.

Sample input:
```
9
```
Sample output:
```
<class 'int'>
<class 'float'>
<class 'str'>
```

<details>
<summary>Solution</summary>

```python
n = int(input())
print(type(n))
print(type(float(n)))
print(type(str(n)))
```

One value, three costumes — the whole conversion story in three lines.
</details>

---

*End — 15 problems. All solutions verified by execution.*
