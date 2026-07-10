# Topic Covers: Introduction to Strings in Python

## Course Topic
**Strings in Python**

## Target Learners
First-year B.Tech students / beginners in Python programming

## Learning Objectives

After completing this lesson, students will be able to:

1. Define what a string is in Python.
2. Create strings using single, double, and triple quotes.
3. Access characters using indexing and slicing.
4. Apply common string methods for case conversion, searching, testing, splitting, and joining.
5. Use loops and conditionals with strings.
6. Build simple real-life string-processing programs.
7. Format strings using f-strings, `.format()`, and `%` formatting.
8. Understand immutability of strings.

---

# 01. Introduction to Strings

## 1.1 What is a String?

A **string** is a sequence of characters.

Characters may include:

- Letters: `A`, `B`, `c`, `d`
- Digits: `1`, `2`, `3`
- Symbols: `@`, `#`, `$`
- Spaces
- Special characters

In Python, strings are written inside quotes.

### Example

```python
name = "Rahul"
city = "Delhi"
message = "Welcome to Python"
```

Here:

- `"Rahul"` is a string.
- `"Delhi"` is a string.
- `"Welcome to Python"` is also a string.

A string can contain one character, many characters, or even no character.

```python
a = "A"
b = "Python"
c = ""
```

Here, `c` is an empty string.

---

## 1.2 Creating Strings Using Quotes

Python allows strings to be written using different types of quotes.

### Single Quotes

```python
name = 'Amit'
print(name)
```

### Double Quotes

```python
name = "Amit"
print(name)
```

Both single quotes and double quotes work in the same way.

### Triple Quotes

Triple quotes are used for multi-line strings.

```python
message = '''Hello students,
Welcome to Python programming.
Today we will learn strings.'''

print(message)
```

Triple quotes can be written using:

```python
'''text'''
```

or

```python
"""text"""
```

---

## 1.3 When to Use Single and Double Quotes?

If the string contains an apostrophe, double quotes are useful.

```python
sentence = "It's a good day"
print(sentence)
```

If the string contains double quotes inside it, single quotes are useful.

```python
sentence = 'He said "Good morning"'
print(sentence)
```

---

## 1.4 Using `str()` Function

The `str()` function converts a value into a string.

### Example

```python
age = 20
text = str(age)

print(text)
print(type(text))
```

### Output

```text
20
<class 'str'>
```

Here, integer `20` is converted into string `"20"`.

---

## 1.5 Why Do We Need `str()`?

Sometimes we need to combine numbers with strings.

### Incorrect Example

```python
age = 20
print("My age is " + age)
```

This gives an error because Python cannot directly join a string and an integer using `+`.

### Correct Example

```python
age = 20
print("My age is " + str(age))
```

### Output

```text
My age is 20
```

---

## 1.6 Printing Strings

The `print()` function is used to display strings.

```python
name = "Simran"
print(name)
```

### Output

```text
Simran
```

We can also print a direct string.

```python
print("Python is easy")
```

### Output

```text
Python is easy
```

---

## 1.7 String Immutability

Strings in Python are **immutable**.

This means once a string is created, its characters cannot be changed directly.

### Example

```python
s = "Python"
s[0] = "J"
```

This gives an error because strings do not allow direct modification of characters.

### Correct Way

```python
s = "Python"
s = "J" + s[1:]

print(s)
```

### Output

```text
Jython
```

Here, we did not change the original string directly. We created a new string.

---

## 1.8 Important Points

- A string is a sequence of characters.
- Strings are written inside quotes.
- Single quotes, double quotes, and triple quotes can be used.
- `str()` converts values into strings.
- Strings are immutable.
- `print()` displays strings on the screen.

---

# 02. Indexing and Slicing

## 2.1 What is Indexing?

Indexing means accessing a character from a string using its position.

In Python, indexing starts from `0`.

### Example

```python
s = "Python"
```

Index positions:

```text
P   y   t   h   o   n
0   1   2   3   4   5
```

### Code

```python
s = "Python"

print(s[0])
print(s[1])
print(s[5])
```

### Output

```text
P
y
n
```

---

## 2.2 Negative Indexing

Python also supports negative indexing.

Negative indexing starts from the end of the string.

```text
P    y    t    h    o    n
-6  -5   -4   -3   -2   -1
```

### Example

```python
s = "Python"

print(s[-1])
print(s[-2])
print(s[-6])
```

### Output

```text
n
o
P
```

---

## 2.3 What is Slicing?

Slicing means extracting a part of a string.

Syntax:

```python
s[start:end]
```

The character at `start` is included, but the character at `end` is not included.

### Example

```python
s = "Python"

print(s[0:2])
print(s[2:5])
```

### Output

```text
Py
tho
```

---

## 2.4 Omitting Start or End

If start is omitted, slicing starts from the beginning.

```python
s = "Python"
print(s[:3])
```

### Output

```text
Pyt
```

If end is omitted, slicing goes till the end.

```python
s = "Python"
print(s[3:])
```

### Output

```text
hon
```

---

## 2.5 Slicing with Step

Syntax:

```python
s[start:end:step]
```

The `step` decides how many positions to jump.

### Example

```python
s = "Python"

print(s[0:6:2])
```

### Output

```text
Pto
```

Explanation:

- Start at index `0`
- Go up to index `6`, but not including `6`
- Jump by `2`

Characters selected: `P`, `t`, `o`

---

## 2.6 Reverse a String Using `[::-1]`

A very common slicing trick is:

```python
s[::-1]
```

It reverses the string.

### Example

```python
s = "Python"
print(s[::-1])
```

### Output

```text
nohtyP
```

---

## 2.7 Common Slicing Examples

```python
s = "Programming"

print(s[0:4])
print(s[4:])
print(s[:6])
print(s[::2])
print(s[::-1])
```

### Output

```text
Prog
ramming
Progra
Pormig
gnimmargorP
```

---

## 2.8 Common Mistakes

### Mistake 1: Using Index Out of Range

```python
s = "Python"
print(s[10])
```

This gives an error because index `10` does not exist.

### Mistake 2: Confusing End Index

```python
s = "Python"
print(s[0:3])
```

Output:

```text
Pyt
```

Index `3` is not included.

---

# 03. String Methods I: Case and Whitespace

String methods are built-in functions that work with strings.

Strings are immutable, so most string methods return a new string instead of changing the original string.

---

## 3.1 `upper()`

Converts all letters to uppercase.

```python
s = "python"
print(s.upper())
```

### Output

```text
PYTHON
```

---

## 3.2 `lower()`

Converts all letters to lowercase.

```python
s = "PYTHON"
print(s.lower())
```

### Output

```text
python
```

---

## 3.3 `title()`

Converts the first letter of each word to uppercase.

```python
s = "python programming language"
print(s.title())
```

### Output

```text
Python Programming Language
```

---

## 3.4 `capitalize()`

Converts only the first character of the string to uppercase and the remaining characters to lowercase.

```python
s = "python PROGRAMMING"
print(s.capitalize())
```

### Output

```text
Python programming
```

---

## 3.5 `strip()`

Removes spaces from both the beginning and end of a string.

```python
s = "   Python   "
print(s.strip())
```

### Output

```text
Python
```

---

## 3.6 `lstrip()`

Removes spaces from the left side.

```python
s = "   Python   "
print(s.lstrip())
```

### Output

```text
Python   
```

---

## 3.7 `rstrip()`

Removes spaces from the right side.

```python
s = "   Python   "
print(s.rstrip())
```

### Output

```text
   Python
```

---

## 3.8 `swapcase()`

Converts uppercase letters to lowercase and lowercase letters to uppercase.

```python
s = "PyThOn"
print(s.swapcase())
```

### Output

```text
pYtHoN
```

---

## 3.9 Important Example

```python
name = "   aMiT kuMar   "

clean_name = name.strip().title()

print(clean_name)
```

### Output

```text
Amit Kumar
```

Here:

- `strip()` removes extra spaces.
- `title()` converts the name into title case.

---

## 3.10 Summary Table

| Method | Use |
|---|---|
| `upper()` | Converts to uppercase |
| `lower()` | Converts to lowercase |
| `title()` | Capitalizes each word |
| `capitalize()` | Capitalizes first character only |
| `strip()` | Removes spaces from both sides |
| `lstrip()` | Removes spaces from left side |
| `rstrip()` | Removes spaces from right side |
| `swapcase()` | Swaps uppercase and lowercase |

---

# 04. String Methods II: Search and Test

This section covers methods used to search inside strings and test the type of string content.

---

## 4.1 `find()`

The `find()` method returns the index of the first occurrence of a substring.

If the substring is not found, it returns `-1`.

### Example

```python
s = "Python programming"

print(s.find("pro"))
print(s.find("Java"))
```

### Output

```text
7
-1
```

---

## 4.2 `index()`

The `index()` method also returns the index of the first occurrence of a substring.

But if the substring is not found, it gives an error.

### Example

```python
s = "Python programming"

print(s.index("pro"))
```

### Output

```text
7
```

### Error Example

```python
s = "Python programming"
print(s.index("Java"))
```

This gives an error because `"Java"` is not present.

---

## 4.3 Difference Between `find()` and `index()`

| Method | If value is found | If value is not found |
|---|---|---|
| `find()` | Returns index | Returns `-1` |
| `index()` | Returns index | Gives error |

---

## 4.4 `count()`

The `count()` method counts how many times a substring appears.

### Example

```python
s = "banana"

print(s.count("a"))
print(s.count("na"))
```

### Output

```text
3
2
```

---

## 4.5 `startswith()`

Checks whether a string starts with a given value.

It returns `True` or `False`.

```python
s = "Python programming"

print(s.startswith("Python"))
print(s.startswith("Java"))
```

### Output

```text
True
False
```

---

## 4.6 `endswith()`

Checks whether a string ends with a given value.

```python
filename = "report.pdf"

print(filename.endswith(".pdf"))
print(filename.endswith(".jpg"))
```

### Output

```text
True
False
```

---

## 4.7 `replace()`

The `replace()` method replaces one substring with another substring.

```python
s = "I like Java"

new_s = s.replace("Java", "Python")

print(new_s)
```

### Output

```text
I like Python
```

---

## 4.8 Testing Methods

Testing methods check the nature of a string.

They usually return `True` or `False`.

---

## 4.9 `isalpha()`

Returns `True` if all characters are alphabets.

```python
print("Python".isalpha())
print("Python3".isalpha())
```

### Output

```text
True
False
```

---

## 4.10 `isdigit()`

Returns `True` if all characters are digits.

```python
print("12345".isdigit())
print("123a".isdigit())
```

### Output

```text
True
False
```

---

## 4.11 `isalnum()`

Returns `True` if all characters are letters or digits.

```python
print("Python123".isalnum())
print("Python 123".isalnum())
```

### Output

```text
True
False
```

The second output is `False` because it contains a space.

---

## 4.12 `isspace()`

Returns `True` if all characters are spaces.

```python
print("   ".isspace())
print(" a ".isspace())
```

### Output

```text
True
False
```

---

## 4.13 `islower()`

Returns `True` if all alphabetic characters are lowercase.

```python
print("python".islower())
print("Python".islower())
```

### Output

```text
True
False
```

---

## 4.14 `isupper()`

Returns `True` if all alphabetic characters are uppercase.

```python
print("PYTHON".isupper())
print("Python".isupper())
```

### Output

```text
True
False
```

---

## 4.15 Real-Life Example: Username Validation

```python
username = "student123"

if username.isalnum():
    print("Valid username")
else:
    print("Invalid username")
```

### Output

```text
Valid username
```

---

# 05. Splitting and Joining

Splitting means breaking a string into parts.

Joining means combining multiple strings into one string.

---

## 5.1 `split()`

The `split()` method breaks a string into a list of words.

By default, it splits using spaces.

### Example

```python
s = "Python is easy"

words = s.split()

print(words)
```

### Output

```text
['Python', 'is', 'easy']
```

---

## 5.2 Splitting Using a Separator

```python
date = "07-07-2026"

parts = date.split("-")

print(parts)
```

### Output

```text
['07', '07', '2026']
```

---

## 5.3 `rsplit()`

The `rsplit()` method splits from the right side.

It is useful when we want to limit the number of splits from the right.

### Example

```python
s = "name,course,section,roll"

print(s.rsplit(",", 1))
```

### Output

```text
['name,course,section', 'roll']
```

Only one split is made from the right side.

---

## 5.4 `splitlines()`

The `splitlines()` method splits a multi-line string into a list of lines.

### Example

```python
text = """Python
Java
C++"""

lines = text.splitlines()

print(lines)
```

### Output

```text
['Python', 'Java', 'C++']
```

---

## 5.5 `join()`

The `join()` method joins strings from a list using a separator.

### Example

```python
words = ["Python", "is", "easy"]

sentence = " ".join(words)

print(sentence)
```

### Output

```text
Python is easy
```

---

## 5.6 Joining with Different Separators

```python
items = ["apple", "banana", "mango"]

print(",".join(items))
print("-".join(items))
print(" | ".join(items))
```

### Output

```text
apple,banana,mango
apple-banana-mango
apple | banana | mango
```

---

## 5.7 Important Rule for `join()`

`join()` works with strings only.

### Incorrect Example

```python
numbers = [1, 2, 3]
print("-".join(numbers))
```

This gives an error because list elements are integers.

### Correct Example

```python
numbers = ["1", "2", "3"]
print("-".join(numbers))
```

### Output

```text
1-2-3
```

---

## 5.8 Real-Life Example: Creating a Clean Sentence

```python
words = ["welcome", "to", "python"]

sentence = " ".join(words).capitalize()

print(sentence)
```

### Output

```text
Welcome to python
```

---

# 06. Iteration and Building Strings

## 6.1 Iterating Through a String

A string can be processed character by character using a loop.

### Example

```python
s = "Python"

for ch in s:
    print(ch)
```

### Output

```text
P
y
t
h
o
n
```

Here, `ch` stores one character at a time.

---

## 6.2 Using `len()`

The `len()` function returns the number of characters in a string.

```python
s = "Python"
print(len(s))
```

### Output

```text
6
```

Spaces are also counted.

```python
s = "Hello World"
print(len(s))
```

### Output

```text
11
```

---

## 6.3 Membership Operators: `in` and `not in`

The `in` operator checks whether a character or substring exists in a string.

```python
s = "Python programming"

print("Python" in s)
print("Java" in s)
```

### Output

```text
True
False
```

The `not in` operator checks whether a value is absent.

```python
s = "Python programming"

print("Java" not in s)
```

### Output

```text
True
```

---

## 6.4 Accumulating a Result String

Because strings are immutable, we cannot modify a character directly.

But we can build a new string step by step.

### Example: Remove Spaces

```python
s = "P y t h o n"
result = ""

for ch in s:
    if ch != " ":
        result = result + ch

print(result)
```

### Output

```text
Python
```

---

## 6.5 Example: Convert Lowercase Letters to Uppercase Manually

```python
s = "hello"
result = ""

for ch in s:
    result = result + ch.upper()

print(result)
```

### Output

```text
HELLO
```

---

## 6.6 Example: Count Vowels

```python
s = "education"
count = 0

for ch in s:
    if ch in "aeiou":
        count = count + 1

print(count)
```

### Output

```text
5
```

---

## 6.7 Important Point About Building Strings

This is acceptable for beginner programs:

```python
result = result + ch
```

For very large data, programmers often use list and `join()` for better performance.

```python
chars = []

for ch in "Python":
    chars.append(ch)

result = "".join(chars)
print(result)
```

---

# 07. Formatting

String formatting means inserting values into a string in a clean and readable way.

---

## 7.1 f-Strings

f-strings are the most common and modern way of formatting strings.

Syntax:

```python
f"text {variable}"
```

### Example

```python
name = "Ananya"
marks = 85

print(f"{name} scored {marks} marks")
```

### Output

```text
Ananya scored 85 marks
```

---

## 7.2 Formatting Decimal Values Using `:.2f`

`:.2f` displays a number up to 2 decimal places.

### Example

```python
price = 45.6789

print(f"Price = {price:.2f}")
```

### Output

```text
Price = 45.68
```

---

## 7.3 Width and Alignment

Formatting can also control spacing.

### Left Alignment

```python
name = "Amit"
print(f"{name:<10}End")
```

### Output

```text
Amit      End
```

### Right Alignment

```python
name = "Amit"
print(f"{name:>10}End")
```

### Output

```text
      AmitEnd
```

### Center Alignment

```python
name = "Amit"
print(f"{name:^10}End")
```

### Output

```text
   Amit   End
```

---

## 7.4 Formatting Table-Like Output

```python
name = "Riya"
marks = 92.456

print(f"{'Name':<10}{'Marks':>10}")
print(f"{name:<10}{marks:>10.2f}")
```

### Output

```text
Name           Marks
Riya           92.46
```

---

## 7.5 `.format()` Method

The `.format()` method is another way to insert values into a string.

### Example

```python
name = "Karan"
age = 19

print("{} is {} years old".format(name, age))
```

### Output

```text
Karan is 19 years old
```

We can also use positions.

```python
print("{0} scored {1} marks".format("Neha", 88))
```

### Output

```text
Neha scored 88 marks
```

---

## 7.6 `%` Formatting

This is an older formatting style.

```python
name = "Rohit"
marks = 76

print("%s scored %d marks" % (name, marks))
```

### Output

```text
Rohit scored 76 marks
```

Common symbols:

| Symbol | Meaning |
|---|---|
| `%s` | String |
| `%d` | Integer |
| `%f` | Float |

For beginners, f-strings are recommended because they are easier to read.

---

## 7.7 `ord()` Function

The `ord()` function returns the Unicode value of a character.

### Example

```python
print(ord("A"))
print(ord("a"))
```

### Output

```text
65
97
```

---

## 7.8 `chr()` Function

The `chr()` function returns the character for a Unicode value.

### Example

```python
print(chr(65))
print(chr(97))
```

### Output

```text
A
a
```

---

## 7.9 Simple Use of `ord()` and `chr()`

```python
ch = "A"

next_ch = chr(ord(ch) + 1)

print(next_ch)
```

### Output

```text
B
```

---

# 08. Strings + Loops and Conditionals: Applications

This section combines strings, loops, and conditionals to solve practical problems.

---

## 8.1 Application 1: Count Digits in a String

### Problem

Given a string, count how many characters are digits.

### Code

```python
s = "abc123xyz45"
count = 0

for ch in s:
    if ch.isdigit():
        count = count + 1

print(count)
```

### Output

```text
5
```

---

## 8.2 Application 2: Count Alphabets, Digits, and Special Characters

### Problem

Given a string, count alphabets, digits, and special characters.

### Code

```python
s = "Amit@123"
alphabets = 0
digits = 0
special = 0

for ch in s:
    if ch.isalpha():
        alphabets = alphabets + 1
    elif ch.isdigit():
        digits = digits + 1
    else:
        special = special + 1

print("Alphabets:", alphabets)
print("Digits:", digits)
print("Special:", special)
```

### Output

```text
Alphabets: 4
Digits: 3
Special: 1
```

---

## 8.3 Application 3: Remove Vowels from a String

### Problem

Given a string, create a new string after removing vowels.

### Code

```python
s = "education"
result = ""

for ch in s:
    if ch not in "aeiouAEIOU":
        result = result + ch

print(result)
```

### Output

```text
dctn
```

---

## 8.4 Application 4: Convert Spaces to Hyphens

### Problem

Given a string, replace spaces with hyphens without using `replace()`.

### Code

```python
s = "python is easy"
result = ""

for ch in s:
    if ch == " ":
        result = result + "-"
    else:
        result = result + ch

print(result)
```

### Output

```text
python-is-easy
```

---

## 8.5 Application 5: Validate a Simple Password

### Problem

A password is valid if:

- It has at least 8 characters.
- It contains at least one digit.
- It contains at least one uppercase letter.

### Code

```python
password = "Python123"

has_digit = False
has_upper = False

for ch in password:
    if ch.isdigit():
        has_digit = True
    if ch.isupper():
        has_upper = True

if len(password) >= 8 and has_digit and has_upper:
    print("Valid password")
else:
    print("Invalid password")
```

### Output

```text
Valid password
```

---

## 8.6 Application 6: Count Words in a Sentence

### Problem

Given a sentence, count the number of words.

### Code

```python
sentence = "Python programming is interesting"

words = sentence.split()

print(len(words))
```

### Output

```text
4
```

---

## 8.7 Application 7: Create Initials from a Name

### Problem

Given a full name, print initials.

### Code

```python
name = "Ravi Kumar Sharma"
words = name.split()
initials = ""

for word in words:
    initials = initials + word[0].upper() + "."

print(initials)
```

### Output

```text
R.K.S.
```

---

## 8.8 Application 8: Check Whether a String is Palindrome

A palindrome reads the same forward and backward.

### Example

`madam` is a palindrome.

### Code

```python
s = "madam"

if s == s[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")
```

### Output

```text
Palindrome
```

---

# Practice Questions

## A. Concept-Based Questions

1. What is a string in Python?
2. Why are strings called immutable?
3. What is the difference between `find()` and `index()`?
4. What is the use of `strip()`?
5. What is the difference between `split()` and `join()`?
6. What does `s[::-1]` do?
7. What is the use of `isdigit()`?
8. Why do we use `str()` while joining numbers with strings?

---

## B. Output-Based Questions

### Question 1

```python
s = "Python"
print(s[1])
print(s[-1])
```

### Question 2

```python
s = "Programming"
print(s[0:4])
print(s[::-1])
```

### Question 3

```python
s = " hello "
print(s.strip().upper())
```

### Question 4

```python
s = "banana"
print(s.count("a"))
print(s.find("na"))
```

### Question 5

```python
text = "one,two,three"
print(text.split(","))
```

---

## C. Coding Practice Problems

### Problem 1: Count Vowels

Write a program to count vowels in a given string.

### Problem 2: Remove Spaces

Write a program to remove all spaces from a given string.

### Problem 3: Count Uppercase Letters

Write a program to count uppercase letters in a given string.

### Problem 4: Reverse Each Word

Input a sentence and reverse each word separately.

Example:

```text
Input: python is easy
Output: nohtyp si ysae
```

### Problem 5: Clean Student Name

Input a student name with extra spaces and irregular case. Print it in proper title case.

Example:

```text
Input:    aMiT kuMAR
Output: Amit Kumar
```

### Problem 6: Extract Digits

Input a string and print only the digits from it.

Example:

```text
Input: ab12cd45
Output: 1245
```

### Problem 7: Validate Roll Number

A roll number is valid if it contains only digits and has exactly 8 characters.

### Problem 8: Replace Vowels with `*`

Input a string and replace every vowel with `*`.

Example:

```text
Input: education
Output: *d*c*t**n
```

---

# Quick Revision Sheet

## String Creation

```python
s1 = 'Python'
s2 = "Python"
s3 = '''Python'''
```

## Indexing

```python
s[0]
s[-1]
```

## Slicing

```python
s[0:3]
s[:3]
s[3:]
s[::-1]
```

## Case Methods

```python
upper()
lower()
title()
capitalize()
swapcase()
```

## Space Methods

```python
strip()
lstrip()
rstrip()
```

## Search Methods

```python
find()
index()
count()
startswith()
endswith()
replace()
```

## Test Methods

```python
isalpha()
isdigit()
isalnum()
isspace()
islower()
isupper()
```

## Split and Join

```python
split()
rsplit()
splitlines()
join()
```

## Formatting

```python
f"{name} scored {marks}"
f"{price:.2f}"
"{} scored {}".format(name, marks)
"%s scored %d" % (name, marks)
```

---

# Final Teaching Note

Strings are one of the most important topics in Python because almost every real application uses text data.

Examples include:

- Student name validation
- Password checking
- Email processing
- File name checking
- Report formatting
- Searching words in text
- Cleaning user input
- Data preprocessing

A good understanding of strings helps students solve many practical programming problems.
