# Strings — Final MCQ Bank, Batch 2 (Q51–Q100)

*Batch 2 of the series. Covers case & whitespace methods (`upper`/`lower`/`title`/`capitalize`/`swapcase`/`strip` family) and search & test methods (`find`/`index`/`count`/`replace`/`startswith`/`endswith`/`is…`).*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch2-answers.md`.*

---

## String Methods I — Case & Whitespace

**Q51. [E]** What does this print?
```python
print('good'.upper())
```
- A) `GOOD`
- B) `good`
- C) `Good`
- D) An error

**Q52. [E]** What does this print?
```python
print('LOUD'.lower())
```
- A) `LOUD`
- B) `loud`
- C) `Loud`
- D) `lOUD`

**Q53. [E]** What does this print?
```python
print('nice day'.title())
```
- A) `Nice day`
- B) `NICE DAY`
- C) `Nice Day`
- D) `nice Day`

**Q54. [H]** What does this print?
```python
print('PYTHON is FUN'.capitalize())
```
- A) `Python Is Fun`
- B) `PYTHON is FUN`
- C) `Python is FUN`
- D) `Python is fun`

**Q55. [M]** What does this print?
```python
print('MiXeD'.swapcase())
```
- A) `mIxEd`
- B) `MIXED`
- C) `mixed`
- D) `MiXeD`

**Q56. [E]** What does this print?
```python
print('  gap  '.strip())
```
- A) `  gap  `
- B) `gap`
- C) `gap  `
- D) `  gap`

**Q57. [M]** What does this print? (brackets show the edges)
```python
print('[' + '  gap  '.lstrip() + ']')
```
- A) `[  gap]`
- B) `[gap]`
- C) `[gap  ]`
- D) `[  gap  ]`

**Q58. [M]** What does this print? (brackets show the edges)
```python
print('[' + '  gap  '.rstrip() + ']')
```
- A) `[gap  ]`
- B) `[gap]`
- C) `[  gap  ]`
- D) `[  gap]`

**Q59. [H]** What does this print?
```python
print('xxcorexx'.strip('x'))
```
- A) `core`
- B) `xxcorexx`
- C) `corexx`
- D) `xxcore`

**Q60. [M]** What does this print?
```python
print('aaa'.upper().lower())
```
- A) `AAA`
- B) `aaa`
- C) `Aaa`
- D) An error

**Q61. [E]** What does this print?
```python
print('abc'.upper() == 'ABC')
```
- A) `False`
- B) `ABC`
- C) `True`
- D) `abc`

**Q62. [M]** What does this print?
```python
print(len('  hi  '.strip()))
```
- A) `6`
- B) `4`
- C) `0`
- D) `2`

**Q63. [M]** What does this print?
```python
s = 'Go'
print(s.lower() + s.upper())
```
- A) `goGO`
- B) `GOgo`
- C) `gogo`
- D) `GOGO`

**Q64. [H]** What does this print?
```python
print('one two'.title().swapcase())
```
- A) `ONE TWO`
- B) `oNE tWO`
- C) `One Two`
- D) `one two`

**Q65. [E]** What does this print?
```python
print('HELLO'.capitalize())
```
- A) `HELLO`
- B) `hello`
- C) `Hello`
- D) `HEllo`

**Q66. [E]** What does this print?
```python
print('hello'.title())
```
- A) `hello`
- B) `HELLO`
- C) `hELLO`
- D) `Hello`

**Q67. [E]** What does this print?
```python
print('a b'.upper())
```
- A) `A B`
- B) `AB`
- C) `a b`
- D) `A_B`

**Q68. [H]** What does this print?
```python
s = '  x  '
print(len(s), len(s.strip()))
```
- A) `1 1`
- B) `5 1`
- C) `5 5`
- D) `3 1`

**Q69. [M]** What does this print?
```python
print('Tea'.lower().capitalize())
```
- A) `tea`
- B) `TEA`
- C) `Tea`
- D) `tEA`

**Q70. [M]** What does this print?
```python
print('ab'.upper() * 2)
```
- A) `AB2`
- B) `abab`
- C) `AABB`
- D) `ABAB`

**Q71. [M]** What does this print?
```python
s = 'Word'
t = s.upper()
print(s, t)
```
- A) `Word WORD`
- B) `WORD WORD`
- C) `Word Word`
- D) `WORD Word`

**Q72. [M]** What does this print?
```python
print('  a b  '.strip().upper())
```
- A) `  A B  `
- B) `A B`
- C) `AB`
- D) `a b`

**Q73. [M]** What does this print?
```python
print('yes'.upper().isupper())
```
- A) `False`
- B) `YES`
- C) `True`
- D) An error

**Q74. [H]** What does this print?
```python
print('HI there'.swapcase().swapcase() == 'HI there')
```
- A) `False`
- B) `hi THERE`
- C) An error
- D) `True`

---

## String Methods II — Search & Test

**Q75. [M]** What does this print?
```python
print('mississippi'.count('ss'))
```
- A) `2`
- B) `4`
- C) `1`
- D) `3`

**Q76. [M]** What does this print?
```python
print('mississippi'.find('ss'))
```
- A) `3`
- B) `2`
- C) `-1`
- D) `5`

**Q77. [E]** What does this print?
```python
print('mississippi'.find('x'))
```
- A) `0`
- B) An error
- C) `-1`
- D) `None`

**Q78. [M]** What does this print?
```python
print('coconut'.count('co'))
```
- A) `1`
- B) `3`
- C) `0`
- D) `2`

**Q79. [M]** What does this print?
```python
print('coconut'.replace('co', 'xy'))
```
- A) `xyxynut`
- B) `xyconut`
- C) `coconut`
- D) `xynut`

**Q80. [M]** What does this print?
```python
print('papa'.replace('a', 'o', 1))
```
- A) `popo`
- B) `popa`
- C) `papa`
- D) `pope`

**Q81. [E]** What does this print?
```python
print('report.txt'.endswith('.txt'))
```
- A) `False`
- B) `.txt`
- C) `True`
- D) `report`

**Q82. [E]** What does this print?
```python
print('report.txt'.startswith('rep'))
```
- A) `False`
- B) `rep`
- C) An error
- D) `True`

**Q83. [M]** What does this print?
```python
print('2024ad'.isdigit())
```
- A) `False`
- B) `True`
- C) `2024`
- D) An error

**Q84. [E]** What does this print?
```python
print('2024'.isdigit())
```
- A) `False`
- B) `True`
- C) `2024`
- D) `4`

**Q85. [M]** What does this print?
```python
print('abcXYZ'.isalpha())
```
- A) `False`
- B) `abc`
- C) `True`
- D) An error

**Q86. [M]** What does this print?
```python
print('ab cd'.isalnum())
```
- A) `True`
- B) `abcd`
- C) An error
- D) `False`

**Q87. [M]** What does this print?
```python
print('AB12'.isalnum())
```
- A) `True`
- B) `False`
- C) `AB`
- D) `12`

**Q88. [E]** What does this print?
```python
print('   '.isspace())
```
- A) `False`
- B) `True`
- C) `3`
- D) An error

**Q89. [E]** What does this print?
```python
print('hello'.islower())
```
- A) `False`
- B) `hello`
- C) `True`
- D) `HELLO`

**Q90. [E]** What does this print?
```python
print('Hello'.islower())
```
- A) `True`
- B) `hello`
- C) An error
- D) `False`

**Q91. [E]** What does this print?
```python
print('WORLD'.isupper())
```
- A) `True`
- B) `False`
- C) `WORLD`
- D) `world`

**Q92. [H]** What does this print?
```python
print('banana'.find('a', 2))
```
- A) `1`
- B) `3`
- C) `-1`
- D) `5`

**Q93. [H]** What does this print?
```python
print('banana'.count('a', 0, 3))
```
- A) `3`
- B) `2`
- C) `1`
- D) `0`

**Q94. [M]** What does this print?
```python
print('one,two,one'.replace('one', '1'))
```
- A) `1,two,one`
- B) `one,two,1`
- C) `1,2,1`
- D) `1,two,1`

**Q95. [H]** What does this print?
```python
print(len('aaa'.replace('a', 'bb')))
```
- A) `6`
- B) `3`
- C) `4`
- D) `2`

**Q96. [H]** What does this print?
```python
s = 'test'
print(s.find('t'), s.find('t', 1))
```
- A) `0 0`
- B) `0 3`
- C) `0 1`
- D) `3 3`

**Q97. [M]** What does this print?
```python
print('Data'.startswith('da'))
```
- A) `True`
- B) `Da`
- C) `False`
- D) An error

**Q98. [H]** What does this print?
```python
print('a1'.isalpha() or '12'.isdigit())
```
- A) `False`
- B) `a1`
- C) An error
- D) `True`

**Q99. [E]** What does this print?
```python
print('hello world'.count('o'))
```
- A) `2`
- B) `1`
- C) `3`
- D) `0`

**Q100. [E]** What does this print?
```python
print('abc'.index('b'))
```
- A) `0`
- B) `1`
- C) `2`
- D) `b`

---

*End of Batch 2 — Q51–Q100. Difficulty: 18 [E] · 22 [M] · 10 [H]. Every answer verified by executing the code.*