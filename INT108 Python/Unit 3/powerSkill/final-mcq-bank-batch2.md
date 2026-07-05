# Functions & Recursion — Final MCQ Bank, Batch 2 (Q51–Q100)

*Unit 3 final revision bank. Batch 2 of 4. Covers Topic 03 (User-Defined Functions), Topic 04 (Parameters & Arguments), and conditionals used inside functions.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch2-answers.md`.*

---

## Topic 03 — User-Defined Functions

**Q51. [E]** To create a function you write the keyword `def`, then the name, then:
- A) parentheses `()` and a colon `:`
- B) square brackets `[]`
- C) a semicolon `;`
- D) the word `return`

**Q52. [E]** Running a function's code by using its name is called:
- A) defining the function
- B) calling the function
- C) importing the function
- D) printing the function

**Q53. [H]** What does this print?
```python
def g():
    print('a')

g
```
- A) `a`
- B) `g`
- C) Nothing
- D) An error

**Q54. [E]** How do you call a function named `g`?
- A) `g`
- B) `call g`
- C) `def g()`
- D) `g()`

**Q55. [H]** What happens here?
```python
hello()

def hello():
    print('hi')
```
- A) An error — called before it is defined
- B) `hi`
- C) Nothing
- D) `hi` twice

**Q56. [M]** What does this print?
```python
def f():
    print('one')

def f():
    print('two')

f()
```
- A) `one`
- B) `two`
- C) `one` then `two`
- D) An error

**Q57. [M]** How many stars does this print?
```python
def s():
    print('*')

s()
s()
s()
```
- A) One
- B) Two
- C) Three, on three lines
- D) Nine

**Q58. [M]** What does this print?
```python
def f():
    print('in')

print('out')
```
- A) `in` then `out`
- B) `in`
- C) `out` then `in`
- D) `out`

**Q59. [H]** What does this print?
```python
print('A')

def f():
    print('B')

print('C')
f()
```
- A) `A C B`
- B) `A B C`
- C) `B A C`
- D) `A C`

**Q60. [M]** What does this print?
```python
def a():
    print(1)

def b():
    print(2)

b()
a()
```
- A) `1` then `2`
- B) `2` then `1`
- C) `1`
- D) `2`

**Q61. [M]** What does this print?
```python
def m():
    for i in range(1, 4):
        print(i, end=' ')

m()
```
- A) `0 1 2`
- B) `1 2 3 4`
- C) `1 2 3`
- D) Nothing

**Q62. [H]** What is wrong here?
```python
def f():
print('x')
```
- A) Nothing
- B) The colon is missing
- C) `print` is misspelled
- D) The body is not indented — an error

**Q63. [M]** What does this print?
```python
def f():
    pass

f()
print('ok')
```
- A) `ok`
- B) An error
- C) Nothing
- D) `pass` then `ok`

**Q64. [H]** What does this print?
```python
def f():
    print('in')
print('out')
f()
```
- A) `in` then `out`
- B) `out` then `in`
- C) `in`
- D) `out`

**Q65. [M]** What does this print?
```python
def f():
    print('a')
    print('b')
print('c')
f()
```
- A) `a b c`
- B) `a b`
- C) `c` then `a` then `b`
- D) `c`

**Q66. [M]** Why is `def 2fun():` invalid?
- A) `fun` is reserved
- B) The number is too small
- C) It is valid
- D) A name cannot start with a digit

**Q67. [M]** Why is `def my-func():` invalid?
- A) Python reads `-` as minus, so hyphens aren't allowed
- B) Names can't be that long
- C) Hyphens are fine; nothing is wrong
- D) It needs a capital letter

**Q68. [E]** Which is a **valid** function name?
- A) `2fun`
- B) `my_func`
- C) `my func`
- D) `my-func`

**Q69. [M]** Why is `def while():` invalid?
- A) `while` is too short
- B) Names must be capitalised
- C) `while` is a reserved keyword
- D) It is valid

**Q70. [M]** Why is `def my func():` invalid?
- A) `func` is reserved
- B) It needs a number
- C) It is valid
- D) A name cannot contain a space

**Q71. [M]** Which is a **valid** function name?
- A) `calc2`
- B) `2calc`
- C) `calc 2`
- D) `calc-2`

**Q72. [H]** Is `_temp` a valid function name?
- A) No — can't start with underscore
- B) Yes — a name may start with an underscore
- C) No — underscores never allowed
- D) Only with a digit

**Q73. [H]** What does this print?
```python
def Go():
    print('cap')

def go():
    print('low')

go()
Go()
```
- A) `cap cap`
- B) `low low`
- C) `low` then `cap`
- D) An error

**Q74. [H]** What happens here?
```python
def go():
    print('hi')

Go()
```
- A) `hi`
- B) Nothing
- C) `Go`
- D) An error — `Go` differs from `go`

**Q75. [H]** Naming a function `print` with `def print():` is:
- A) allowed, but a bad idea — it hides the built-in
- B) impossible — forbidden
- C) the recommended way
- D) an automatic error

**Q76. [M]** How many lines does this print?
```python
def b():
    print('x')
    print('y')

b()
print('z')
```
- A) `2`
- B) `3`
- C) `1`
- D) `4`

---

## Topic 04 — Parameters & Arguments

**Q77. [M]** What does this print?
```python
def sub(a, b):
    print(a - b)

sub(4, 10)
```
- A) `6`
- B) `14`
- C) `-6`
- D) `4`

**Q78. [H]** What does this print?
```python
def f(x, y):
    print(x, y)

f(y=1, x=2)
```
- A) `1 2`
- B) `2 2`
- C) An error
- D) `2 1`

**Q79. [M]** What does this print?
```python
def g(a, b=5):
    print(a + b)

g(10)
```
- A) `15`
- B) `10`
- C) `5`
- D) An error

**Q80. [M]** What does this print?
```python
def g(a, b=5):
    print(a + b)

g(10, 20)
```
- A) `15`
- B) `30`
- C) `35`
- D) `25`

**Q81. [H]** Why does `def f(a=1, b):` cause an error?
- A) Only one default is allowed
- B) `a` and `b` clash
- C) A default parameter can't come before a non-default one
- D) Defaults must be strings

**Q82. [E]** What does this print?
```python
def area(l, w):
    print(l * w)

area(6, 3)
```
- A) `9`
- B) `63`
- C) `2`
- D) `18`

**Q83. [H]** What happens here?
```python
def f(a, b):
    print(a + b)

f(5)
```
- A) An error — a required argument is missing
- B) `5`
- C) `10`
- D) `0`

**Q84. [H]** What happens here?
```python
def f(a):
    print(a)

f(1, 2)
```
- A) `1`
- B) An error — too many arguments
- C) `1 2`
- D) `3`

**Q85. [M]** What does this print?
```python
def f(n):
    print(n * n)

f(3 + 2)
```
- A) `13`
- B) `11`
- C) `25`
- D) `10`

**Q86. [M]** What does this print?
```python
x = 7
def f(n):
    print(n)

f(x)
```
- A) `x`
- B) `0`
- C) An error
- D) `7`

**Q87. [H]** What does this print?
```python
def f(a, b, c):
    print(a, b, c)

f(1, c=3, b=2)
```
- A) `1 2 3`
- B) `1 3 2`
- C) `1 2 3` in a different order
- D) An error

**Q88. [M]** What does this print?
```python
def greet(name, g='Hi'):
    print(g, name)

greet('Al')
```
- A) `Al Hi`
- B) `Hi Al`
- C) `Hi`
- D) An error

**Q89. [M]** What does this print?
```python
def f(a, b, c):
    print(a * b + c)

f(2, 3, 4)
```
- A) `14`
- B) `20`
- C) `10`
- D) `24`

**Q90. [M]** What does this print?
```python
n = 100
def f(n):
    print(n)

f(7)
print(n)
```
- A) `7` then `7`
- B) `100` then `7`
- C) `100` then `100`
- D) `7` then `100`

**Q91. [M]** What does this print?
```python
def f(a, b):
    print(a // b)

f(20, 3)
```
- A) `6`
- B) `6.66`
- C) `7`
- D) `2`

**Q92. [H]** What does this print?
```python
def f(x, step=2):
    print(x + step)

f(10)
f(10, 5)
```
- A) `12` then `12`
- B) `12` then `15`
- C) `15` then `15`
- D) `10` then `10`

**Q93. [M]** What does this print?
```python
def f(a, b):
    print(a - b)

f(b=3, a=10)
```
- A) `-7`
- B) `13`
- C) `7`
- D) An error

**Q94. [H]** What does this print?
```python
def dbl(n):
    return n * 2

def f(n):
    print(n + 1)

f(dbl(3))
```
- A) `6`
- B) `4`
- C) `8`
- D) `7`

**Q95. [M]** What does this print?
```python
def f(a, b):
    print(a % b == 0)

f(12, 4)
```
- A) `True`
- B) `False`
- C) `0`
- D) `3`

**Q96. [M]** What does this print?
```python
def f(a, b=0):
    print(a + b)

f(9)
```
- A) `0`
- B) `9`
- C) An error
- D) `90`

---

## Conditionals Inside Functions

**Q97. [M]** What does this print?
```python
def sign(n):
    if n > 0:
        return 'pos'
    elif n < 0:
        return 'neg'
    return 'zero'

print(sign(-4))
```
- A) `pos`
- B) `zero`
- C) `neg`
- D) `-4`

**Q98. [H]** What does this print?
```python
def f(n):
    if n % 2 == 0:
        if n > 10:
            return 'big even'
        return 'small even'
    return 'odd'

print(f(4))
```
- A) `big even`
- B) `odd`
- C) `4`
- D) `small even`

**Q99. [M]** What does this print?
```python
def cat(a):
    if a < 13:
        return 'child'
    elif a < 20:
        return 'teen'
    else:
        return 'adult'

print(cat(16))
```
- A) `teen`
- B) `child`
- C) `adult`
- D) `16`

**Q100. [M]** What does this print?
```python
def f(m):
    if m >= 90:
        return 'A'
    if m >= 75:
        return 'B'
    return 'C'

print(f(80))
```
- A) `A`
- B) `B`
- C) `C`
- D) `80`

---

*End of Batch 2 — Q51–Q100. Difficulty: 5 [E] · 28 [M] · 17 [H]. Every answer verified by executing the code.*