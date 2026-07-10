# Topic 01 — Introduction to Strings

*Unit 4 · Strings. This is the foundation lesson: what a string is, how to make one, and the single most important idea about strings — that they cannot be changed in place. Later topics build indexing, slicing, traversal, comparison, and methods on top of everything here.*

---

## 1. What is a string?

A **string** is a piece of text — a sequence of characters written between quotes. Characters can be letters, digits, spaces, punctuation, or symbols.

```python
name = "Ravi"
greeting = 'Hello, world!'
digits = "12345"
```

Even though `"12345"` looks like a number, it is text. A string of digits is not the same as the integer `12345` — you cannot do arithmetic with it directly.

```python
print("5" + "5")
```
This prints `55`, not `10`. For strings, `+` **joins** text; it does not add numbers.

---

## 2. Creating strings

You can write a string with single quotes or double quotes — they behave identically:

```python
a = 'hi'
b = "hi"
print(a == b)      # True
```

Use whichever is convenient. Double quotes are handy when the text itself contains an apostrophe (`"it's fine"`), and single quotes when it contains double quotes (`'she said "hi"'`).

For text spanning several lines, use **triple quotes**:

```python
message = '''Dear friend,
Welcome aboard.'''
print(message)
```

An **empty string** has no characters at all, written `''` or `""`. Its length is 0:

```python
print(len(""))     # 0
```

### Turning other values into strings

The `str()` function converts a number or other value into its text form:

```python
print(str(42))     # 42  (now text, not a number)
print(str(3.5))    # 3.5
print(str(True))   # True
```

This is useful when you want to join a number onto a message:

```python
age = 20
print("Age: " + str(age))   # Age: 20
```

Without `str()`, `"Age: " + age` would be an error, because you cannot join text directly to a number.

---

## 3. A string is a sequence of characters

This is the key mental model for the whole unit: a string is an ordered sequence of characters, each sitting at a numbered position.

The word `"hello"` is five characters in a row:

```
 h   e   l   l   o
 0   1   2   3   4
```

Because a string is a sequence, several things work naturally:

**Length** — how many characters:
```python
print(len("hello"))    # 5
```

**Access one character by its position** (positions start at 0):
```python
print("hello"[0])      # h
print("hello"[4])      # o
```

**Loop over every character**:
```python
for ch in "cat":
    print(ch)
```
prints `c`, then `a`, then `t`, each on its own line.

**Ask whether a character (or piece of text) is inside**:
```python
print("e" in "hello")    # True
print("z" in "hello")    # False
```

Indexing, slicing, and traversal — the next three topics — all rest on this one idea: a string is characters in order, at positions you can count.

---

## 4. Joining and repeating

Two simple operations build bigger strings from smaller ones.

**Concatenation** with `+` joins two strings end to end:
```python
print("foo" + "bar")    # foobar
first = "Good "
second = "morning"
print(first + second)   # Good morning
```

**Repetition** with `*` repeats a string a whole number of times:
```python
print("ab" * 3)         # ababab
print("-" * 10)         # ----------
```

Both `+` and `*` produce a **new** string; they never alter the originals. That leads directly to the most important idea in this unit.

---

## 5. Strings are immutable

**Immutable** means "cannot be changed." Once a string exists, you cannot change one of its characters in place. Trying to do so is an error:

```python
s = "hello"
s[0] = "H"      # TypeError: 'str' object does not support item assignment
```

Python refuses this. A string's characters are fixed the moment the string is created.

So how do you "change" a string? You don't — you **build a new one** and keep it instead:

```python
s = "hello"
s = "H" + s[1:]     # take "ello", put "H" in front
print(s)            # Hello
```

Here `s[1:]` is the slice `"ello"` (slicing comes in Topic 03). We made a brand-new string `"Hello"` and pointed `s` at it. The old `"hello"` was not edited — it was replaced.

### Why this matters

Because strings are immutable, assigning one string variable to another, then changing one, never disturbs the other:

```python
a = "hi"
b = a          # b now refers to the same text
a = a + "!"    # a becomes a NEW string "hi!"
print(a, b)    # hi! hi
```

`b` is still `"hi"`. The `a = a + "!"` line did not modify the original text; it created `"hi!"` and reassigned `a`. This predictability is a feature: a string you hand to a function can never be secretly altered.

Every string method you will meet (like `upper()` or `replace()`) follows this rule — they **return a new string** and leave the original untouched.

---

## 6. Printing strings

`print()` displays a string. It can take several values, which it shows separated by spaces:

```python
print("x", "y", "z")     # x y z
```

You can change the separator with `sep`:

```python
print("x", "y", sep="-")   # x-y
```

To confirm something is a string, `type()` reports its kind:

```python
print(type("hi"))    # <class 'str'>
```

---

## Summary

- A **string** is text: a sequence of characters in quotes. Single, double, or triple quotes all create strings.
- A digit-string like `"5"` is text, not a number; `"5" + "5"` is `"55"`. Use `str()` to convert numbers to text.
- A string is a **sequence of characters** at numbered positions (starting at 0). This supports `len()`, indexing `s[i]`, looping `for ch in s`, and membership `in`.
- `+` **joins** strings, `*` **repeats** them — both make new strings.
- Strings are **immutable**: you cannot change a character in place (`s[0] = "H"` is a `TypeError`). To "change" a string, build a new one and reassign.
- Because of immutability, copying a string variable and changing one copy never affects the other. Every string method returns a *new* string and leaves the original unchanged.

**Next:** Topic 02 — Indexing & Slicing, where we use those numbered positions to pull out single characters and whole ranges.
