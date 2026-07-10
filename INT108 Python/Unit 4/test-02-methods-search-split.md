# Test 02 — Methods, Search & Split

*Unit 4 · Strings. Covers Topics 04–05: search & test methods (`find`, `count`, `replace`, `startswith`/`endswith`, `is…`) and splitting & joining (`split`, `join`). Every question is a real text-processing scenario.*
*Marks: Section A — 10 MCQ × 1 = 10. Section B — 10 coding × 3 = 30. **Total 40.** Answers and marking scheme in `test-02-methods-search-split-answers.md`.*

---

## Section A — Multiple Choice (1 mark each)

**Q1. [E]** A program checks whether an uploaded file is a spreadsheet:
```python
filename = 'report.csv'
print(filename.endswith('.csv'))
```
What does it print?
- A) `True`
- B) `False`
- C) `.csv`
- D) `report`

**Q2. [M]** A line from a data file holds one record. How many fields does this row have?
```python
row = 'Ravi,25,Delhi,Engineer'
print(len(row.split(',')))
```
- A) `3`
- B) `4`
- C) `23`
- D) `1`

**Q3. [M]** An email validator locates the `@` symbol:
```python
email = 'ravi@site.com'
print(email.find('@'))
```
What is printed?
- A) `5`
- B) `-1`
- C) `4`
- D) `1`

**Q4. [M]** A program extracts the domain part of an email:
```python
email = 'ravi@site.com'
print(email.split('@')[1])
```
- A) `ravi`
- B) `site`
- C) `@site.com`
- D) `site.com`

**Q5. [M]** A phone number is stored with dashes that need removing:
```python
phone = '98-76-54'
print(phone.replace('-', ''))
```
- A) `987654`
- B) `98-76-54`
- C) `98 76 54`
- D) `987654-`

**Q6. [M]** A URL path is split to find the page being requested:
```python
url = 'shop/items/book'
print(url.split('/')[-1])
```
- A) `shop`
- B) `book`
- C) `items`
- D) `shop/items`

**Q7. [E]** A form checks that a 4-digit PIN contains only numbers:
```python
pin = '1234'
print(pin.isdigit())
```
- A) `False`
- B) `1234`
- C) `True`
- D) `4`

**Q8. [M]** A poll counts how many people answered 'yes':
```python
answers = 'yes no yes yes'
print(answers.count('yes'))
```
- A) `2`
- B) `4`
- C) `1`
- D) `3`

**Q9. [M]** A messaging app checks whether a number has the Indian country code:
```python
number = '+91-9876'
print(number.startswith('+91'))
```
- A) `True`
- B) `False`
- C) `+91`
- D) `91`

**Q10. [M]** A blog joins a list of tags into one display string:
```python
tags = ['python', 'code', 'fun']
print(', '.join(tags))
```
- A) `['python', 'code', 'fun']`
- B) `python, code, fun`
- C) `python code fun`
- D) `pythoncodefun`

---

## Section B — Coding (3 marks each)

*Judge-format: read input with `input()`, print exact output. Where two inputs are shown, they arrive on separate lines.*

**Q11. [E] File Extension** — A file-upload system needs the extension. Print the part of the filename after the last dot.
- **Input:** `document.pdf`  →  **Output:** `pdf`

**Q12. [E] Review Word Count** — A shopping site shows how many words a customer review has. Print the number of words.
- **Input:** `great product loved it`  →  **Output:** `4`

**Q13. [M] Email Username** — When someone signs up, the system shows the part of their email before the `@`. Print it.
- **Input:** `john.doe@mail.com`  →  **Output:** `john.doe`

**Q14. [M] Keyword Frequency** — A search tool counts how often a keyword appears in an article, ignoring case. Print the count.
- **Input:** `The cat sat on the mat / the`  →  **Output:** `2`

**Q15. [M] Clean an ID** — An ID is typed with stray spaces. Print how many characters it has once all spaces are removed.
- **Input:** `AB 12 CD 34`  →  **Output:** `8`

**Q16. [H] Numeric Fields** — A CSV record mixes text and numbers. Print how many of its comma-separated fields are purely numeric.
- **Input:** `Ravi,25,Delhi,50000`  →  **Output:** `2`

**Q17. [M] Format an Address** — An address is stored comma-separated. Print it with each comma replaced by a space.
- **Input:** `Delhi,India,110001`  →  **Output:** `Delhi India 110001`

**Q18. [E] First Name** — A greeting uses only the first name. Given a full name, print the first name.
- **Input:** `Ravi Kumar Sharma`  →  **Output:** `Ravi`

**Q19. [H] Capitalised Words** — A style checker counts how many words in a title begin with a capital letter. Print the count.
- **Input:** `The Quick brown Fox`  →  **Output:** `3`

**Q20. [H] Generate a Username** — A system builds a username from a person's first and last name: both lowercased, joined by a dot. Print it.
- **Input:** `Ravi Kumar`  →  **Output:** `ravi.kumar`

---
*End of Test 02 paper.*