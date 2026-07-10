# Strings — Final MCQ Bank, Batch 3 (Q101–Q150)

*Batch 3 of the series. Covers `split`/`join` (including edge behaviour) and character/word iteration with accumulation.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch3-answers.md`.*

---

## Splitting & Joining

**Q101. [E]** What does this print?
```python
print('x y z'.split())
```
- A) `['x', 'y', 'z']`
- B) `'x y z'`
- C) `['x y z']`
- D) `xyz`

**Q102. [E]** What does this print?
```python
print('1-2-3'.split('-'))
```
- A) `[1, 2, 3]`
- B) `['1', '2', '3']`
- C) `['1-2-3']`
- D) `123`

**Q103. [M]** What does this print?
```python
print(len('a,b,,c'.split(',')))
```
- A) `3`
- B) `5`
- C) `4`
- D) `2`

**Q104. [M]** What does this print?
```python
print('up-down-left'.split('-')[2])
```
- A) `down`
- B) `up`
- C) `['left']`
- D) `left`

**Q105. [E]** What does this print?
```python
print('*'.join(['a', 'b']))
```
- A) `a*b`
- B) `ab`
- C) `a * b`
- D) `*ab*`

**Q106. [M]** What does this print?
```python
print(''.join(['1', '2', '3']))
```
- A) `1 2 3`
- B) `123`
- C) `['123']`
- D) `6`

**Q107. [M]** What does this print?
```python
print('.'.join('ab'))
```
- A) `ab.`
- B) `.ab`
- C) `a.b`
- D) An error

**Q108. [H]** What does this print?
```python
print('w x  y'.split(' '))
```
- A) `['w', 'x', 'y']`
- B) `['w x  y']`
- C) `['w', 'x', ' ', 'y']`
- D) `['w', 'x', '', 'y']`

**Q109. [M]** What does this print?
```python
print('w x  y'.split())
```
- A) `['w', 'x', 'y']`
- B) `['w', 'x', '', 'y']`
- C) `['w x  y']`
- D) An error

**Q110. [H]** What does this print?
```python
print('a:b:c:d'.split(':', 1))
```
- A) `['a', 'b', 'c', 'd']`
- B) `['a', 'b:c:d']`
- C) `['a:b', 'c:d']`
- D) `['a']`

**Q111. [M]** What does this print?
```python
words = 'go stop go'.split()
print(words.count('go'))
```
- A) `1`
- B) `3`
- C) `2`
- D) `go go`

**Q112. [M]** What does this print?
```python
print(' '.join('a-b'.split('-')))
```
- A) `a-b`
- B) `ab`
- C) `['a', 'b']`
- D) `a b`

**Q113. [M]** What does this print?
```python
print('-'.join('cat'))
```
- A) `c-a-t`
- B) `cat-`
- C) `-cat-`
- D) An error

**Q114. [H]** What happens here?
```python
print(','.join([5, 6]))
```
- A) `5,6`
- B) An error — `join` needs strings, not numbers
- C) `56`
- D) `[5, 6]`

**Q115. [M]** What does this print?
```python
parts = 'one two three'.split()
print(parts[0], parts[-1])
```
- A) `one two`
- B) `two three`
- C) `one three`
- D) `three one`

**Q116. [E]** What does this print?
```python
print(len('spring'.split('r')))
```
- A) `1`
- B) `3`
- C) `6`
- D) `2`

**Q117. [M]** What does this print?
```python
print('aXbXc'.split('X'))
```
- A) `['a', 'b', 'c']`
- B) `['aXbXc']`
- C) `['a', 'X', 'b', 'X', 'c']`
- D) `abc`

**Q118. [H]** What does this print?
```python
print('::'.join(['p', 'q', 'r']))
```
- A) `p:q:r`
- B) `p::q::r`
- C) `::pqr::`
- D) `pq::r`

**Q119. [M]** What does this print?
```python
s = 'red green blue'
print(len(s.split()[1]))
```
- A) `3`
- B) `4`
- C) `5`
- D) `15`

**Q120. [M]** What does this print?
```python
print(' '.join('hi there you'.split()[::-1]))
```
- A) `hi there you`
- B) `uoy ereht ih`
- C) `you hi there`
- D) `you there hi`

**Q121. [E]** What does this print?
```python
print('a b c'.split()[1])
```
- A) `b`
- B) `a`
- C) `c`
- D) `['b']`

**Q122. [H]** What does this print?
```python
line = 'k=v'
key = line.split('=')[0]
val = line.split('=')[1]
print(val + '=' + key)
```
- A) `k=v`
- B) `v=k`
- C) `kv=`
- D) `=vk`

---

## Iteration & Building

**Q123. [E]** What does this print?
```python
c = 0
for ch in 'abcd':
    c += 1
print(c)
```
- A) `3`
- B) `abcd`
- C) `4`
- D) `0`

**Q124. [M]** What does this print?
```python
r = ''
for ch in 'xy':
    r = r + ch + ch
print(r)
```
- A) `xyxy`
- B) `xy`
- C) `yyxx`
- D) `xxyy`

**Q125. [M]** What does this print?
```python
r = ''
for ch in 'dog':
    r = ch + r
print(r)
```
- A) `god`
- B) `dog`
- C) `ddoogg`
- D) `ogd`

**Q126. [E]** What does this print?
```python
print('end' in 'weekend')
```
- A) `False`
- B) `True`
- C) `end`
- D) `4`

**Q127. [M]** What does this print?
```python
c = 0
for ch in 'level up':
    if ch in 'aeiou':
        c += 1
print(c)
```
- A) `2`
- B) `4`
- C) `3`
- D) `8`

**Q128. [M]** What does this print?
```python
r = ''
for ch in 'a1b2':
    if ch.isalpha():
        r = r + ch
print(r)
```
- A) `12`
- B) `a1b2`
- C) `ba`
- D) `ab`

**Q129. [H]** What does this print?
```python
s = 'abc'
for i in range(len(s) - 1, -1, -1):
    print(s[i], end='')
```
- A) `cba`
- B) `abc`
- C) `cb`
- D) `bca`

**Q130. [M]** What does this print?
```python
total = 0
for ch in '246':
    total += int(ch)
print(total)
```
- A) `246`
- B) `12`
- C) `6`
- D) `3`

**Q131. [M]** What does this print?
```python
c = 0
for ch in 'good food':
    if ch == 'o':
        c += 1
print(c)
```
- A) `3`
- B) `2`
- C) `4`
- D) `5`

**Q132. [E]** What does this print?
```python
print('z' not in 'puzzle')
```
- A) `True`
- B) `z`
- C) An error
- D) `False`

**Q133. [M]** What does this print?
```python
r = ''
for ch in 'note':
    if ch not in 'aeiou':
        r = r + ch
print(r)
```
- A) `nt`
- B) `oe`
- C) `note`
- D) `n`

**Q134. [H]** What does this print?
```python
s = 'ping'
r = ''
for i in range(len(s)):
    if i % 2 == 0:
        r = r + s[i]
print(r)
```
- A) `ig`
- B) `pn`
- C) `ping`
- D) `pi`

**Q135. [M]** What does this print?
```python
big = ''
for w in 'cat mouse ox'.split():
    if len(w) > len(big):
        big = w
print(big)
```
- A) `cat`
- B) `ox`
- C) `mouse`
- D) `catmouseox`

**Q136. [M]** What does this print?
```python
c = 0
for w in 'a bb ccc dddd'.split():
    if len(w) >= 3:
        c += 1
print(c)
```
- A) `3`
- B) `4`
- C) `1`
- D) `2`

**Q137. [E]** What does this print?
```python
for ch in 'no':
    print(ch)
```
- A) `n` and `o` on separate lines
- B) `no`
- C) `n o`
- D) `nn oo`

**Q138. [H]** What does this print?
```python
s = 'swap'
r = ''
for ch in s:
    if ch == 'a':
        r = r + 'o'
    else:
        r = r + ch
print(r)
```
- A) `swap`
- B) `swop`
- C) `swoop`
- D) `swp`

**Q139. [M]** What does this print?
```python
count = 0
for ch in 'Hi There':
    if ch.isupper():
        count += 1
print(count)
```
- A) `1`
- B) `3`
- C) `2`
- D) `7`

**Q140. [M]** What does this print?
```python
first = ''
for w in 'sky blue bird'.split():
    first = first + w[0]
print(first)
```
- A) `sky`
- B) `sb`
- C) `bbs`
- D) `sbb`

**Q141. [M]** What does this print?
```python
r = ''
for ch in 'seed':
    if ch != 'e':
        r = r + ch
print(r)
```
- A) `sd`
- B) `ee`
- C) `seed`
- D) `s`

**Q142. [H]** What does this print?
```python
s = 'mirror'
c = 0
for i in range(len(s)):
    if s[i] == s[len(s) - 1 - i]:
        c += 1
print(c)
```
- A) `6`
- B) `2`
- C) `0`
- D) `3`

**Q143. [M]** What does this print?
```python
total = 0
for w in 'to be or'.split():
    total += len(w)
print(total)
```
- A) `8`
- B) `3`
- C) `6`
- D) `7`

**Q144. [E]** What does this print?
```python
print(len('a b c'.split()))
```
- A) `5`
- B) `2`
- C) `1`
- D) `3`

**Q145. [M]** What does this print?
```python
r = ''
for ch in 'abc':
    r = r + ch.upper() + ch
print(r)
```
- A) `AaBbCc`
- B) `ABCabc`
- C) `aAbBcC`
- D) `AaBb`

**Q146. [H]** What does this print?
```python
vow = 0
con = 0
for ch in 'stream':
    if ch in 'aeiou':
        vow += 1
    else:
        con += 1
print(vow, con)
```
- A) `4 2`
- B) `2 4`
- C) `2 5`
- D) `3 3`

**Q147. [M]** What does this print?
```python
c = 0
for ch in 'a1b2c3d4':
    if ch.isdigit():
        c += 1
print(c)
```
- A) `8`
- B) `3`
- C) `4`
- D) `1234`

**Q148. [M]** What does this print?
```python
found = 0
for w in 'the cat the dog'.split():
    if w == 'the':
        found += 1
print(found)
```
- A) `1`
- B) `4`
- C) `0`
- D) `2`

**Q149. [H]** What does this print?
```python
s = 'abcdef'
r = ''
for i in range(0, len(s), 2):
    r = r + s[i + 1]
print(r)
```
- A) `bdf`
- B) `ace`
- C) `abcdef`
- D) `fdb`

**Q150. [M]** What does this print?
```python
longest = 0
for w in 'hi hello hey'.split():
    if len(w) > longest:
        longest = len(w)
print(longest)
```
- A) `3`
- B) `5`
- C) `2`
- D) `hello`

---

*End of Batch 3 — Q101–Q150. Difficulty: 10 [E] · 29 [M] · 11 [H]. Every answer verified by executing the code.*