# Strings — Final MCQ Bank, Batch 4 (Q151–Q200)

*Batch 4 of the series. Covers formatting (f-strings, `:.2f`, `ord`/`chr`, `.format()`) and applied questions that combine slicing, methods, iteration, and conditionals.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch4-answers.md`.*

---

## Formatting

**Q151. [E]** What does this print?
```python
city = 'Pune'
print(f'Welcome to {city}')
```
- A) `Welcome to Pune`
- B) `Welcome to {city}`
- C) `Welcome to city`
- D) `Pune`

**Q152. [M]** What does this print?
```python
print(f'{7 * 6}')
```
- A) `{7 * 6}`
- B) `42`
- C) `7 * 6`
- D) `76`

**Q153. [M]** What does this print?
```python
print(f'{5:.2f}')
```
- A) `5`
- B) `5.0`
- C) `5.00`
- D) `5.20`

**Q154. [M]** What does this print?
```python
print(f'{2 / 8:.2f}')
```
- A) `0.3`
- B) `0.2`
- C) `.25`
- D) `0.25`

**Q155. [H]** What does this print?
```python
print(round(7.10, 2))
```
- A) `7.1`
- B) `7.10`
- C) `7`
- D) `7.100`

**Q156. [M]** What does this print?
```python
print(f'{19.567:.2f}')
```
- A) `19.56`
- B) `19.57`
- C) `19.5`
- D) `20.00`

**Q157. [E]** What does this print?
```python
print(ord('a'))
```
- A) `65`
- B) `a`
- C) `97`
- D) `1`

**Q158. [E]** What does this print?
```python
print(chr(100))
```
- A) `D`
- B) `100`
- C) `c`
- D) `d`

**Q159. [M]** What does this print?
```python
print(ord('b') - ord('a'))
```
- A) `1`
- B) `0`
- C) `2`
- D) `ba`

**Q160. [H]** What does this print?
```python
print(chr(ord('z') - 25))
```
- A) `z`
- B) `a`
- C) `y`
- D) `A`

**Q161. [M]** What does this print?
```python
n = 'Om'
a = 8
print(f'{n}:{a}')
```
- A) `n:a`
- B) `Om 8`
- C) `Om:8`
- D) `{n}:{a}`

**Q162. [M]** What does this print?
```python
print('{}-{}'.format('x', 'y'))
```
- A) `{}-{}`
- B) `xy`
- C) `y-x`
- D) `x-y`

**Q163. [H]** What does this print?
```python
print('{0}{0}'.format('go'))
```
- A) `gogo`
- B) `go`
- C) `{0}{0}`
- D) `go0`

**Q164. [M]** What does this print?
```python
price = 40
print(f'Rs {price}.00')
```
- A) `Rs price.00`
- B) `Rs 40.00`
- C) `Rs 40`
- D) `Rs {price}.00`

**Q165. [M]** What does this print?
```python
print(f'{100 / 3:.2f}')
```
- A) `33.3`
- B) `33`
- C) `33.33`
- D) `33.34`

**Q166. [H]** What does this print?
```python
print(chr(ord('A') + 2))
```
- A) `B`
- B) `c`
- C) `67`
- D) `C`

**Q167. [E]** What does this print?
```python
print(f'{1 + 1}{2 + 2}')
```
- A) `24`
- B) `6`
- C) `1122`
- D) `{2}{4}`

**Q168. [M]** What does this print?
```python
x = 9.5
print(f'{x:.2f} kg')
```
- A) `9.5 kg`
- B) `9.50 kg`
- C) `9 kg`
- D) `9.50kg`

**Q169. [M]** What does this print?
```python
print(ord('A'), ord('a'))
```
- A) `97 65`
- B) `A a`
- C) `65 97`
- D) `65 65`

**Q170. [H]** What does this print?
```python
total = 5
print(f'{total * 2:.2f}')
```
- A) `10`
- B) `10.0`
- C) `5.00`
- D) `10.00`

---

## Application — Combined Skills

**Q171. [M]** What does this print?
```python
s = 'noon'
print(s == s[::-1])
```
- A) `True`
- B) `False`
- C) `noon`
- D) `nnoo`

**Q172. [M]** What does this print?
```python
s = 'stop pots'
words = s.split()
print(words[0] == words[1][::-1])
```
- A) `False`
- B) `True`
- C) `stop`
- D) An error

**Q173. [M]** What does this print?
```python
name = '  ravi kumar  '
print(name.strip().title())
```
- A) `ravi kumar`
- B) `Ravi kumar`
- C) `Ravi Kumar`
- D) `  Ravi Kumar  `

**Q174. [H]** What does this print?
```python
code = 'AB-12-CD'
print(code.replace('-', '').lower())
```
- A) `AB12CD`
- B) `ab-12-cd`
- C) `abcd`
- D) `ab12cd`

**Q175. [M]** What does this print?
```python
c = 0
for w in 'an old owl ate'.split():
    if w[0] in 'aeiou':
        c += 1
print(c)
```
- A) `4`
- B) `3`
- C) `2`
- D) `1`

**Q176. [H]** What does this print?
```python
s = 'a1b2c3'
total = 0
for ch in s:
    if ch.isdigit():
        total += int(ch)
print(total * 2)
```
- A) `6`
- B) `12`
- C) `24`
- D) `123123`

**Q177. [M]** What does this print?
```python
msg = 'send help now'
print(len(msg.split()) * 2)
```
- A) `3`
- B) `13`
- C) `6`
- D) `26`

**Q178. [M]** What does this print?
```python
s = 'banana'
print(s.count('a') + s.count('n'))
```
- A) `3`
- B) `2`
- C) `6`
- D) `5`

**Q179. [H]** What does this print?
```python
u = 'Ravi Kumar'
parts = u.split()
print((parts[0][0] + parts[1][0]).lower())
```
- A) `rk`
- B) `RK`
- C) `Ra`
- D) `rkumar`

**Q180. [M]** What does this print?
```python
s = 'aabbb'
print(s.count('a') < s.count('b'))
```
- A) `False`
- B) `True`
- C) `2 3`
- D) `ab`

**Q181. [M]** What does this print?
```python
file = 'notes.final.txt'
print(file.split('.')[-1])
```
- A) `final`
- B) `notes`
- C) `txt`
- D) `.txt`

**Q182. [H]** What does this print?
```python
s = 'hello'
new = s[0].upper() + s[1:]
print(new)
```
- A) `hello`
- B) `HELLO`
- C) An error
- D) `Hello`

**Q183. [M]** What does this print?
```python
email = 'a@b.com'
print(email.find('@') < email.find('.'))
```
- A) `True`
- B) `False`
- C) `1 3`
- D) An error

**Q184. [M]** What does this print?
```python
s = 'Xy'
print(s.lower() + s.upper() + s)
```
- A) `XyXyXy`
- B) `xyXYXy`
- C) `xyxyxy`
- D) `XYxyXy`

**Q185. [M]** What does this print?
```python
word = 'letter'
print(len(word) - word.count('t'))
```
- A) `6`
- B) `2`
- C) `4`
- D) `5`

**Q186. [H]** What does this print?
```python
s = 'race'
r = ''
for ch in s:
    r = ch + r
print(r == 'ecar')
```
- A) `False`
- B) `ecar`
- C) `race`
- D) `True`

**Q187. [M]** What does this print?
```python
line = 'id:42'
print(int(line.split(':')[1]) + 8)
```
- A) `50`
- B) `42`
- C) `428`
- D) An error

**Q188. [M]** What does this print?
```python
s = 'The Cat'
c = 0
for ch in s:
    if ch.islower():
        c += 1
print(c)
```
- A) `2`
- B) `4`
- C) `6`
- D) `3`

**Q189. [H]** What does this print?
```python
a = 'listen'
b = 'silent'
print(len(a) == len(b) and a[0] != b[0])
```
- A) `False`
- B) `listen silent`
- C) `True`
- D) An error

**Q190. [M]** What does this print?
```python
s = 'go go go'
print(s.replace('go', 'run', 2))
```
- A) `run run run`
- B) `go go go`
- C) `run go go`
- D) `run run go`

**Q191. [M]** What does this print?
```python
s = 'abcdef'
half = len(s) // 2
print(s[:half])
```
- A) `abc`
- B) `def`
- C) `abcd`
- D) `ab`

**Q192. [H]** What does this print?
```python
s = 'aBcD'
r = ''
for ch in s:
    if ch.isupper():
        r = r + ch.lower()
    else:
        r = r + ch.upper()
print(r)
```
- A) `aBcD`
- B) `AbCd`
- C) `ABCD`
- D) `abcd`

**Q193. [M]** What does this print?
```python
words = 'red car red bus'.split()
print(words.count('red') * 10)
```
- A) `2`
- B) `10`
- C) `20`
- D) `40`

**Q194. [M]** What does this print?
```python
s = 'python'
print(s[:2] + s[-2:])
```
- A) `pyth`
- B) `onpy`
- C) `python`
- D) `pyon`

**Q195. [M]** What does this print?
```python
pin = '0421'
print(pin.isdigit() and pin[0] == '0')
```
- A) `True`
- B) `False`
- C) `0421`
- D) An error

**Q196. [H]** What does this print?
```python
s = 'moon noon'
c = 0
for w in s.split():
    if w == w[::-1]:
        c += 1
print(c)
```
- A) `2`
- B) `1`
- C) `0`
- D) `noon`

**Q197. [M]** What does this print?
```python
heading = 'top news today'
print(heading.title().count('T'))
```
- A) `1`
- B) `3`
- C) `2`
- D) `0`

**Q198. [M]** What does this print?
```python
s = '3,4'
a, b = s.split(',')
print(int(a) * int(b))
```
- A) `34`
- B) `7`
- C) An error
- D) `12`

**Q199. [H]** What does this print?
```python
s = 'level'
mid = len(s) // 2
print(s[:mid] == s[mid+1:][::-1])
```
- A) `True`
- B) `False`
- C) `le ve`
- D) An error

**Q200. [M]** What does this print?
```python
tag = '#Fun'
print(tag[1:].upper())
```
- A) `#FUN`
- B) `FUN`
- C) `fun`
- D) `Fun`

---

*End of Batch 4 — Q151–Q200. Difficulty: 4 [E] · 32 [M] · 14 [H]. Every answer verified by executing the code.*