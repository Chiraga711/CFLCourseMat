# User-Defined Functions — MCQ Set (Q1–Q50)

*Unit 3 · Topic 03. Covers: defining with `def`, calling, the function body, and naming rules.*
*Scope note: parameters (Topic 04) and `return` (Topic 05) are not used here — every function takes no input in its parentheses and returns nothing. Bodies use loops, conditionals, and `input()` as needed.*
*Tags: [E] easy · [M] medium · [H] hard. Answers are in the separate file `03-user-defined-functions-mcq-answers.md`.*

---

## Section A — `def` and Call Syntax

**Q1. [E]** Which keyword begins the definition of a function?
- A) `func`
- B) `def`
- C) `define`
- D) `function`

**Q2. [E]** What punctuation mark must end the first line of a function definition?
- A) A semicolon `;`
- B) A full stop `.`
- C) A colon `:`
- D) Nothing

**Q3. [M]** What is wrong with this code?
```python
def greet()
    print("hi")
```
- A) Nothing is wrong
- B) `print` should be capitalised
- C) A function cannot be named `greet`
- D) The colon `:` after `greet()` is missing

**Q4. [M]** How do you **call** a function named `greet`?
- A) `greet`
- B) `call greet`
- C) `greet()`
- D) `def greet()`

**Q5. [H]** What does this code print?
```python
def greet():
    print("hi")

greet
```
- A) `hi`
- B) Nothing is printed
- C) An error
- D) `greet`

**Q6. [M]** What does this code do?
```python
def greet():
    print("hi")
```
- A) Prints `hi`
- B) Causes an error
- C) Prints `greet`
- D) Prints nothing — the function is defined but never called

**Q7. [M]** How many times is `hi` printed?
```python
def greet():
    print("hi")

greet()
greet()
greet()
```
- A) `3`
- B) `1`
- C) `0`
- D) `2`

**Q8. [H]** What happens when this runs?
```python
greet()

def greet():
    print("hi")
```
- A) It prints `hi`
- B) It prints nothing
- C) An error — `greet` is called before it is defined
- D) It prints `hi` twice

**Q9. [M]** What does this print?
```python
def f():
    print("one")

def f():
    print("two")

f()
```
- A) `one`
- B) `two`
- C) `one` then `two`
- D) An error

**Q10. [M]** A pair of empty parentheses `()` in `def greet():` tells Python that:
- A) The function is empty
- B) The function will cause an error
- C) The function returns nothing
- D) The function takes no values inside its parentheses

**Q11. [E]** Defining a function means:
- A) Writing its code and giving it a name, to run later
- B) Running its code immediately
- C) Printing its name
- D) Deleting it from memory

**Q12. [H]** What does this code print?
```python
def start():
    print("go")

start()
start
start()
```
- A) `go` three times
- B) `go` twice
- C) `go` once
- D) An error

---

## Section B — Execution Order & Tracing

**Q13. [M]** What does this print?
```python
def f():
    print("inside")

print("outside")
```
- A) `inside` then `outside`
- B) `inside`
- C) `outside`
- D) `outside` then `inside`

**Q14. [H]** What does this print?
```python
print("A")

def f():
    print("B")

print("C")
f()
print("D")
```
- A) `A B C D`
- B) `B A C D`
- C) `A C D B`
- D) `A C B D`

**Q15. [M]** What does this print?
```python
def one():
    print(1)

def two():
    print(2)

two()
one()
two()
```
- A) `2 1 2`
- B) `1 2 1`
- C) `1 1 2`
- D) `2 2 1`

**Q16. [H]** What happens when this runs?
```python
def a():
    print("a")

b()

def b():
    print("b")
```
- A) It prints `a` then `b`
- B) It prints `b`
- C) An error — `b` is called before it is defined
- D) It prints `a`

**Q17. [M]** What does this print?
```python
def evens():
    for i in range(2, 9, 2):
        print(i, end=" ")

evens()
```
- A) `2 4 6 8 10`
- B) `2 4 6 8`
- C) `1 2 3 4`
- D) Nothing

**Q18. [M]** What does this print?
```python
def stars():
    for i in range(3):
        print("*", end="")
    print()

stars()
stars()
```
- A) `***`
- B) `******`
- C) 
```
*
*
```
- D) Two lines, each `***`:
```
***
***
```

**Q19. [H]** With inputs `5` then `8` (one per line), what does this print?
```python
def rd():
    n = int(input())
    print(n * 2)

rd()
rd()
```
- A) `10`
- B) `10` then `16`
- C) `16` then `10`
- D) `26`

**Q20. [E]** Defining a function (but not calling it) causes its body to run:
- A) Once
- B) Twice
- C) Never
- D) Every line of the program

**Q21. [M]** In what order do the labelled lines run?
```python
def show():
    print("Y")     # line 2

print("X")         # line 1
show()             # calls line 2
print("Z")         # line 3
```
- A) `X Y Z`
- B) `Y X Z`
- C) `X Z Y`
- D) `Y Z X`

**Q22. [M]** How many lines of output does this produce?
```python
def hello():
    print("hi")

hello()
hello()
```
- A) `1`
- B) `0`
- C) `4`
- D) `2`

**Q23. [H]** What does this print?
```python
def count():
    for i in range(1, 4):
        print(i, end=" ")

count()
count()
```
- A) `1 2 3`
- B) `1 2 3 1 2 3`
- C) `2 4 6`
- D) `1 2 3 4 5 6`

**Q24. [M]** What does this print?
```python
def greet():
    print("hi")

def bye():
    print("bye")

greet()
bye()
greet()
```
- A) `hi bye`
- B) `hi hi bye`
- C) `hi bye hi`
- D) `bye hi bye`

**Q25. [H]** What does this print?
```python
def check():
    n = 12
    if n % 2 == 0:
        print("even")
    else:
        print("odd")

check()
```
- A) `even`
- B) `odd`
- C) `12`
- D) Nothing

**Q26. [M]** A function's body can contain:
- A) Only `print()` statements
- B) Only one line
- C) No loops
- D) Loops, `if` statements, and any code you've learned

---

## Section C — Function Body & Indentation

**Q27. [M]** In Python, what marks which lines belong to a function's body?
- A) Curly braces `{ }`
- B) Indentation (spaces at the start of the line)
- C) A `begin` and `end` keyword
- D) Square brackets `[ ]`

**Q28. [H]** What does this print?
```python
def f():
    print("in")
print("out")
f()
```
- A) `in out`
- B) `in`
- C) `out in`
- D) `out`

**Q29. [M]** Which lines are part of the function's body?
```python
def f():
    print("a")
    print("b")
print("c")
```
- A) `print("a")` and `print("b")`
- B) All three `print` lines
- C) Only `print("a")`
- D) Only `print("c")`

**Q30. [H]** What is wrong with this code?
```python
def f():
print("hello")
```
- A) Nothing is wrong
- B) The colon is missing
- C) `print` is misspelled
- D) The body is not indented, causing an error

**Q31. [M]** A function whose body is completely empty:
- A) Runs fine and does nothing
- B) Causes an error unless it contains at least `pass`
- C) Prints an empty line
- D) Is not allowed in Python

**Q32. [M]** What does this print?
```python
def nothing():
    pass

nothing()
print("done")
```
- A) An error
- B) Nothing
- C) `done`
- D) `pass` then `done`

**Q33. [H]** What does this print?
```python
def f():
    print("a")
    print("b")

print("c")
f()
```
- A) `c a b`
- B) `a b c`
- C) `a b`
- D) `c`

**Q34. [M]** Why might a programmer write a function body of just `pass`?
- A) To make the function print `pass`
- B) To stop the program
- C) To call the function
- D) To leave a placeholder for code to be written later, without an error

**Q35. [M]** In `def f():`, the code that runs when `f()` is called is:
- A) Every line after `def f():` until the end of the file
- B) Only the very next line
- C) The line `def f():` itself
- D) The indented block beneath `def f():`

**Q36. [H]** How many lines of output does this produce?
```python
def block():
    print("x")
    print("y")

block()
print("z")
```
- A) `2`
- B) `1`
- C) `3`
- D) `4`

---

## Section D — Naming Rules

**Q37. [E]** Which of these is a **valid** function name?
- A) `my_func`
- B) `2fun`
- C) `my func`
- D) `my-func`

**Q38. [M]** Why is `def 2fun():` invalid?
- A) `fun` is a reserved word
- B) The number is too small
- C) It is actually valid
- D) A function name cannot start with a digit

**Q39. [M]** Why is `def my-func():` invalid?
- A) The name is too long
- B) Hyphens are not allowed in names — Python reads `-` as minus
- C) Hyphens are allowed; nothing is wrong
- D) It needs a capital letter

**Q40. [H]** Why is `def for():` invalid?
- A) `for` is too short
- B) Function names must be capitalised
- C) `for` is a reserved keyword and cannot be used as a name
- D) It is actually valid

**Q41. [M]** Which of these is a **valid** function name?
- A) `fun2`
- B) `def`
- C) `2fun`
- D) `my func`

**Q42. [M]** Why is `def my func():` invalid?
- A) `func` is reserved
- B) It needs a number
- C) It is actually valid
- D) Names cannot contain a space

**Q43. [H]** Is `_hidden` a valid function name?
- A) No — names cannot start with an underscore
- B) Yes — a name may start with an underscore
- C) No — underscores are never allowed
- D) Only if it contains a digit

**Q44. [H]** What does this print?
```python
def Show():
    print("cap")

def show():
    print("low")

show()
Show()
```
- A) `low` then `cap`
- B) `cap cap`
- C) `low low`
- D) An error — two functions can't have such similar names

**Q45. [H]** What happens when this runs?
```python
def show():
    print("hi")

Show()
```
- A) An error — `Show` is not the same name as `show`
- B) It prints `hi`
- C) It prints nothing
- D) It prints `Show`

**Q46. [M]** By common Python convention, function names should be written:
- A) In `UPPERCASE`
- B) Starting with a number
- C) With hyphens between words
- D) In `lowercase_with_underscores`

**Q47. [M]** Which of these function names breaks Python's rules?
- A) `total_marks`
- B) `find max`
- C) `calc3`
- D) `_temp`

**Q48. [M]** Which character is allowed inside a function name?
- A) A space
- B) A hyphen `-`
- C) An underscore `_`
- D) A full stop `.`

**Q49. [H]** Naming a function `print` (as in `def print():`) is:
- A) Allowed by the rules, but a bad idea — it hides the built-in `print`
- B) Impossible — Python forbids it
- C) The recommended way to make a print function
- D) An automatic error

**Q50. [E]** Function names in Python are case-sensitive. This means `Total` and `total` are:
- A) The same name
- B) Two different names
- C) Both invalid
- D) Not allowed together

---

*End of set — 50 questions. Difficulty: 6 [E] · 27 [M] · 17 [H]. Every answer verified by executing the code.*