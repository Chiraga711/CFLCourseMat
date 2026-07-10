# Strings — Final MCQ Bank, Batch 1 (Q1–Q50)

*Unit 4 final revision bank. Batch 1 of the series. Covers introduction & immutability, indexing (positive and negative), and slicing (ranges, steps, and edge behaviour).*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch1-answers.md`.*

---

## Introduction & Immutability

**Q1. [E]** What does this print?
```python
print('5' + '5')
```
- A) `55`
- B) `10`
- C) `5 5`
- D) An error

**Q2. [E]** What does this print?
```python
print(len('hello world'))
```
- A) `10`
- B) `11`
- C) `12`
- D) `2`

**Q3. [M]** What does this print?
```python
print(str(7) + str(3))
```
- A) `10`
- B) `7 3`
- C) `73`
- D) An error

**Q4. [E]** What does this print?
```python
print(type('123'))
```
- A) `<class 'int'>`
- B) `123`
- C) `<class 'number'>`
- D) `<class 'str'>`

**Q5. [E]** What does this print?
```python
print('ha' * 3)
```
- A) `hahaha`
- B) `ha3`
- C) `hahahaha`
- D) `ha ha ha`

**Q6. [M]** What happens here?
```python
s = 'dog'
s[0] = 'D'
print(s)
```
- A) `Dog`
- B) An error — strings are immutable
- C) `dog`
- D) `Ddog`

**Q7. [H]** What does this print?
```python
s = 'cat'
t = s
s = s + 's'
print(t)
```
- A) `cats`
- B) `catss`
- C) `cat`
- D) An error

**Q8. [E]** What does this print?
```python
print(len(''))
```
- A) `1`
- B) An error
- C) `None`
- D) `0`

**Q9. [H]** What does this print?
```python
print('a' + 'b' * 2)
```
- A) `abb`
- B) `abab`
- C) `ab2`
- D) `aabb`

**Q10. [M]** What does this print?
```python
print(('a' + 'b') * 2)
```
- A) `abb`
- B) `abab`
- C) `ab2`
- D) `aabb`

**Q11. [M]** What does this print?
```python
s = 'hi'
s.upper()
print(s)
```
- A) `HI`
- B) `Hi`
- C) `hi`
- D) An error

**Q12. [M]** What happens here?
```python
print('Age: ' + 21)
```
- A) `Age: 21`
- B) `Age: `
- C) `21`
- D) An error — text cannot be joined to a number without `str()`

---

## Indexing

**Q13. [E]** What does this print?
```python
print('python'[2])
```
- A) `t`
- B) `y`
- C) `h`
- D) `p`

**Q14. [E]** What does this print?
```python
print('python'[-1])
```
- A) `p`
- B) `n`
- C) `o`
- D) An error

**Q15. [M]** What does this print?
```python
print('python'[-6])
```
- A) `n`
- B) An error
- C) `p`
- D) `y`

**Q16. [M]** What does this print?
```python
print('apple'[len('apple') - 1])
```
- A) `l`
- B) An error
- C) `a`
- D) `e`

**Q17. [M]** What happens here?
```python
print('code'[4])
```
- A) An error — index 4 is past the end
- B) `e`
- C) `c`
- D) Nothing prints

**Q18. [H]** What happens here?
```python
print('code'[-5])
```
- A) `c`
- B) An error — negative indexing also has limits
- C) `e`
- D) `code`

**Q19. [E]** What does this print?
```python
s = 'book'
print(s[1] + s[2])
```
- A) `bo`
- B) `ok`
- C) `oo`
- D) `bk`

**Q20. [M]** What does this print?
```python
s = 'grape'
print(s[0].upper() + s[-1])
```
- A) `GE`
- B) `ge`
- C) `Gr`
- D) `Ge`

**Q21. [E]** What does this print?
```python
s = 'ab'
print(s[0] * 3)
```
- A) `aaa`
- B) `ababab`
- C) `a3`
- D) `bbb`

**Q22. [H]** What does this print?
```python
w = 'mango'
print(w[2], w[-3])
```
- A) `n g`
- B) `n n`
- C) `a n`
- D) `g o`

**Q23. [M]** What does this print?
```python
print('xyz'[0] == 'x')
```
- A) `False`
- B) `x`
- C) `True`
- D) An error

**Q24. [E]** What does this print?
```python
s = 'hello'
print(s[1] + s[3])
```
- A) `he`
- B) `ll`
- C) `eo`
- D) `el`

**Q25. [M]** What does this print?
```python
s = 'tiger'
i = 2
print(s[i + 1])
```
- A) `e`
- B) `g`
- C) `i`
- D) `r`

**Q26. [H]** What does this print?
```python
print('12345'[2] + '12345'[2])
```
- A) `6`
- B) `33`
- C) `3`
- D) An error

**Q27. [M]** What does this print?
```python
print(int('12345'[2]) * 2)
```
- A) `33`
- B) `24`
- C) `6`
- D) An error

**Q28. [M]** What does this print?
```python
s = 'abcdef'
print(s[len(s) // 2])
```
- A) `c`
- B) `cd`
- C) `e`
- D) `d`

**Q29. [E]** What does this print?
```python
s = 'race'
print(s[-2] + s[-1])
```
- A) `ce`
- B) `ra`
- C) `ec`
- D) `ac`

**Q30. [M]** What does this print?
```python
s = 'sun'
print(s[0] + s[1] + s[2] == s)
```
- A) `False`
- B) `True`
- C) `sun`
- D) An error

---

## Slicing

**Q31. [E]** What does this print?
```python
print('elephant'[1:4])
```
- A) `leph`
- B) `ele`
- C) `lep`
- D) `eleph`

**Q32. [E]** What does this print?
```python
print('elephant'[:4])
```
- A) `eleph`
- B) `hant`
- C) `elepha`
- D) `elep`

**Q33. [E]** What does this print?
```python
print('elephant'[4:])
```
- A) `hant`
- B) `phant`
- C) `elep`
- D) `ant`

**Q34. [M]** What does this print?
```python
print('elephant'[:])
```
- A) `''` (empty)
- B) `elephant`
- C) An error
- D) `e`

**Q35. [M]** What does this print?
```python
print('window'[-3:])
```
- A) `win`
- B) `ndo`
- C) `dow`
- D) `w`

**Q36. [M]** What does this print?
```python
print('window'[:-3])
```
- A) `dow`
- B) `window`
- C) `wind`
- D) `win`

**Q37. [H]** What does this print?
```python
print('abcdefgh'[1:7:2])
```
- A) `bdf`
- B) `bdfh`
- C) `aceg`
- D) `bcd`

**Q38. [M]** What does this print?
```python
print('abcdefgh'[::3])
```
- A) `abc`
- B) `adg`
- C) `adgh`
- D) `cfh`

**Q39. [M]** What does this print?
```python
print('racecar'[::-1])
```
- A) `rac`
- B) `racecarr`
- C) `racecar`
- D) An error

**Q40. [E]** What does this print?
```python
print('python'[::-1])
```
- A) `python`
- B) `p`
- C) `nohty`
- D) `nohtyp`

**Q41. [M]** What does this print?
```python
print('sunday'[2:99])
```
- A) `nday`
- B) An error
- C) `''` (empty)
- D) `sunday`

**Q42. [H]** What does this print?
```python
print('sunday'[99:])
```
- A) An error
- B) `''` — an empty string, with no error
- C) `sunday`
- D) `y`

**Q43. [M]** What does this print?
```python
print(len('sunday'[1:4]))
```
- A) `4`
- B) `2`
- C) `3`
- D) `6`

**Q44. [H]** What does this print?
```python
s = 'keyboard'
print(s[2:5] + s[:2])
```
- A) `keybo`
- B) `ybike`
- C) `board`
- D) `yboke`

**Q45. [H]** What does this print?
```python
print('abcdef'[4:1:-1])
```
- A) `edc`
- B) `bcd`
- C) `edcb`
- D) `fed`

**Q46. [M]** What does this print?
```python
s = 'monitor'
print(s[1:-1])
```
- A) `monitor`
- B) `onito`
- C) `onitor`
- D) `monit`

**Q47. [H]** What does this print?
```python
print('ab'[1:1])
```
- A) `b`
- B) `a`
- C) `''` — an empty string
- D) An error

**Q48. [M]** What does this print?
```python
s = 'planet'
print(s[:3] * 2)
```
- A) `planetplanet`
- B) `pla2`
- C) `plapl`
- D) `plapla`

**Q49. [H]** What does this print?
```python
s = 'stream'
print(s[::2] + s[1::2])
```
- A) `sratem`
- B) `stream`
- C) `srtaem`
- D) `maerts`

**Q50. [M]** What does this print?
```python
s = 'coding'
print(s[-4:-1])
```
- A) `ding`
- B) `din`
- C) `cod`
- D) `ing`

---

*End of Batch 1 — Q1–Q50. Difficulty: 15 [E] · 24 [M] · 11 [H]. Every answer verified by executing the code.*