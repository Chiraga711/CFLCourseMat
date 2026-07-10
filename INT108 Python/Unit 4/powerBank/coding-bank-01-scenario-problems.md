# Strings Coding Bank — Batch 1: Scenario & Word Problems (1–20)

*Real systems doing text work: signups, receipts, logs, filenames, messages.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-01-scenario-solutions.md`.*

---

## 1 — Username Generator  [M]

A signup system builds a username from a full name: first name and last name, joined by a dot, all lowercase.

**Input Format:** Two words on one line — the full name.
**Output Format:** The username.

**Sample Input:**
```
Ravi Kumar
```
**Sample Output:**
```
ravi.kumar
```
---

## 2 — Password Categories  [M]

A password checker reports how many of these categories appear: uppercase letter, lowercase letter, digit. Print the count (0–3).

**Input Format:** One line — the password.
**Output Format:** An integer 0–3.

**Sample Input:**
```
Pass123
```
**Sample Output:**
```
3
```
---

## 3 — Mask a Word  [E]

A chat filter shows a banned word as asterisks of the same length.

**Input Format:** One line — the word.
**Output Format:** A string of `*` of equal length.

**Sample Input:**
```
secret
```
**Sample Output:**
```
******
```
---

## 4 — Bill Line Total  [E]

A till computes one bill line: quantity × unit price (given in paise), displayed in rupees with exactly two decimals.

**Input Format:** Two lines — the quantity, then the unit price in paise (both integers).
**Output Format:** The line total in rupees, to 2 decimals.

**Sample Input:**
```
3
1525
```
**Sample Output:**
```
45.75
```
---

## 5 — Initials  [M]

A form shows a person's initials: first letter of each word, uppercased, joined.

**Input Format:** One line — a full name.
**Output Format:** The initials.

**Sample Input:**
```
mohandas karamchand gandhi
```
**Sample Output:**
```
MKG
```
---

## 6 — File Parts  [M]

An uploader splits a filename into name and extension around the **last** dot, printing them on one line separated by a space.

**Input Format:** One line — a filename containing at least one dot.
**Output Format:** `name extension`.

**Sample Input:**
```
photo.png
```
**Sample Output:**
```
photo png
```
---

## 7 — Log Field  [M]

A log line has fields separated by `|`. Print the field at a given position (counting from 0).

**Input Format:** Two lines — the log line, then an integer position.
**Output Format:** The field at that position.

**Sample Input:**
```
2024|INFO|start
1
```
**Sample Output:**
```
INFO
```
---

## 8 — SMS Preview  [M]

A phone shows only the first 10 characters of a message, adding `...` if it was longer. Print the preview.

**Input Format:** One line — the message.
**Output Format:** The first 10 characters, plus `...` if the message exceeded 10.

**Sample Input:**
```
Hello, are you coming today?
```
**Sample Output:**
```
Hello, are...
```
---

## 9 — Email Domain Count  [H]

Given two email addresses on separate lines, print `1` if they share the same domain (the part after `@`), otherwise print the length of the first domain. (An information-rich check.)

**Input Format:** Two lines — two email addresses.
**Output Format:** `1` if same domain, else the first domain's length.

**Sample Input:**
```
a@mail.com
b@mail.com
```
**Sample Output:**
```
1
```
---

## 10 — Roll Number Check Digit  [M]

A roll number's check value is the sum of its digit characters. Print it.

**Input Format:** One line — a roll number mixing letters and digits.
**Output Format:** The sum of the digits.

**Sample Input:**
```
CS2024
```
**Sample Output:**
```
8
```
---

## 11 — Line Wrap Count  [H]

A display fits `w` characters per line. Print how many lines a text needs (a partly-filled last line counts).

**Input Format:** Two lines — the text, then the width `w`.
**Output Format:** The number of lines.

**Sample Input:**
```
hello world
4
```
**Sample Output:**
```
3
```
---

## 12 — Name Tag  [M]

A badge printer shows `SURNAME, First` from `First Surname`.

**Input Format:** One line — first name and surname.
**Output Format:** `SURNAME, First`.

**Sample Input:**
```
Ravi Kumar
```
**Sample Output:**
```
KUMAR, Ravi
```
---

## 13 — Hashtag Builder  [M]

A social app turns a phrase into a hashtag: remove the spaces, capitalise each word, prefix `#`.

**Input Format:** One line — a phrase.
**Output Format:** The hashtag.

**Sample Input:**
```
good morning all
```
**Sample Output:**
```
#GoodMorningAll
```
---

## 14 — Duplicate Username  [H]

If a requested username already exists, systems append a number. Given the requested name and the count of existing copies, print the name if the count is 0, else the name followed by the count.

**Input Format:** Two lines — the name, then an integer count.
**Output Format:** The resolved username.

**Sample Input:**
```
ravi
0
```
**Sample Output:**
```
ravi
```
---

## 15 — CSV Column  [M]

Print column `k` (0-based) of a comma-separated record.

**Input Format:** Two lines — the record, then `k`.
**Output Format:** The field at column `k`.

**Sample Input:**
```
Ravi,25,Delhi
2
```
**Sample Output:**
```
Delhi
```
---

## 16 — Characters Remaining  [M]

A title box allows 30 characters. Print how many remain after the given title (0 if exactly full; assume it fits).

**Input Format:** One line — the title (length ≤ 30).
**Output Format:** The characters remaining out of 30.

**Sample Input:**
```
My Trip
```
**Sample Output:**
```
23
```
---

## 17 — Phone Normaliser  [M]

Strip spaces and dashes from a phone number; print the cleaned digits and their count, separated by a space.

**Input Format:** One line — the raw phone number.
**Output Format:** `digits count`.

**Sample Input:**
```
98-76 54
```
**Sample Output:**
```
987654 6
```
---

## 18 — Search Hits  [M]

Print how many times a search term occurs in a line of text (case-insensitive).

**Input Format:** Two lines — the text, then the term.
**Output Format:** The number of occurrences.

**Sample Input:**
```
The theme of the day
the
```
**Sample Output:**
```
3
```
---

## 19 — Invoice Code  [E]

Build an invoice code by joining a year, a department, and a serial with `/`.

**Input Format:** Three lines — year, department, serial.
**Output Format:** `YEAR/DEPT/SERIAL`.

**Sample Input:**
```
2024
HR
007
```
**Sample Output:**
```
2024/HR/007
```
---

## 20 — Time Band  [H]

A support system reads a 24-hour time like `14:30` and prints the shift number: hours 0–7 → `0`, 8–15 → `1`, 16–23 → `2`.

**Input Format:** One line — a time `HH:MM`.
**Output Format:** The shift number 0, 1 or 2.

**Sample Input:**
```
14:30
```
**Sample Output:**
```
1
```
---

*End of Batch 1 — 20 problems. Difficulty: 3 [E] · 13 [M] · 4 [H]. All reference solutions verified by execution.*