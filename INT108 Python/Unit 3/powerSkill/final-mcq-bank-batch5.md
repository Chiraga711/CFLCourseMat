# Functions & Recursion — Final MCQ Bank, Batch 5 (Q201–Q245)

*Bonus set: Functions with Loops, Conditionals & Operators. 45 trace questions where a function wraps loops, nested loops, conditionals, and arithmetic/logical operators.*
*Tags: [E] easy · [M] medium · [H] hard. Answers in `final-mcq-bank-batch5-answers.md`.*

---

**Q201. [M]** What does this print?
```python
def calc(a,b):
 if a>b:
  return a+b*2
 else:
  return (a+b)*2
print(calc(5,3))
```
- A) `11`
- B) `16`
- C) `13`
- D) `10`

**Q202. [E]** What does this print?
```python
def fun(n):
 total=0
 for i in range(1,n+1):
  total+=i*2
 return total
print(fun(4))
```
- A) `10`
- B) `20`
- C) `24`
- D) `30`

**Q203. [E]** What does this print?
```python
def check(x):
 if x%2==0:
  return x//2
 else:
  return x*3
print(check(7))
```
- A) `3`
- B) `10`
- C) `21`
- D) `14`

**Q204. [M]** What does this print?
```python
def count_pairs(n):
 count=0
 for i in range(n):
  for j in range(n):
   if i+j==2:
    count+=1
 return count
print(count_pairs(4))
```
- A) `2`
- B) `4`
- C) `5`
- D) `3`

**Q205. [M]** What does this print?
```python
def result(a,b):
 if a%b==0:
  return a//b
 return a+b
print(result(17,4))
```
- A) `21`
- B) `24`
- C) `42`
- D) `5`

**Q206. [E]** What does this print?
```python
def power_sum(n):
 s=0
 for i in range(1,n+1):
  s+=i*i
 return s
print(power_sum(3))
```
- A) `6`
- B) `14`
- C) `9`
- D) `18`

**Q207. [M]** What does this print?
```python
def mystery(n):
 ans=1
 for i in range(1,n):
  ans*=i
 return ans
print(mystery(5))
```
- A) `120`
- B) `20`
- C) `24`
- D) `15`

**Q208. [M]** What does this print?
```python
def test(a,b):
 if a>0 and b>0:
  return a*b
 elif a>0 or b>0:
  return a+b
 else:
  return 0
print(test(-2,5))
```
- A) `-10`
- B) `5`
- C) `0`
- D) `3`

**Q209. [M]** What does this print?
```python
def nested(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   total+=j
 return total
print(nested(3))
```
- A) `10`
- B) `6`
- C) `12`
- D) `14`

**Q210. [M]** What does this print?
```python
def find(n):
 c=0
 for i in range(1,n+1):
  if i%2==0:
   c+=i
  else:
   c-=i
 return c
print(find(5))
```
- A) `3`
- B) `-3`
- C) `-5`
- D) `5`

**Q211. [M]** What does this print?
```python
def logic(x):
 if x%3==0:
  if x%2==0:
   return 'A'
  else:
   return 'B'
 return 'C'
print(logic(9))
```
- A) `A`
- B) `C`
- C) `B`
- D) `Error`

**Q212. [M]** What does this print?
```python
def loop_math(n):
 total=0
 for i in range(n):
  total+=i+1
 return total*2
print(loop_math(4))
```
- A) `10`
- B) `16`
- C) `24`
- D) `20`

**Q213. [M]** What does this print?
```python
def compare(a,b,c):
 if a+b>c:
  return a*b
 else:
  return b*c
print(compare(2,3,6))
```
- A) `18`
- B) `5`
- C) `6`
- D) `12`

**Q214. [H]** What does this print?
```python
def count_even(n):
 count=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if (i*j)%2==0:
    count+=1
 return count
print(count_even(3))
```
- A) `4`
- B) `5`
- C) `6`
- D) `9`

**Q215. [M]** What does this print?
```python
def value(x):
 if x>10:
  x=x-5
 if x>5:
  x=x*2
 return x
print(value(12))
```
- A) `7`
- B) `12`
- C) `14`
- D) `24`

**Q216. [M]** What does this print?
```python
def series(n):
 s=0
 for i in range(1,n+1):
  if i%2==0:
   s+=i*i
 return s
print(series(5))
```
- A) `30`
- B) `10`
- C) `40`
- D) `20`

**Q217. [M]** What does this print?
```python
def fun(a):
 total=0
 for i in range(a):
  if i%2==1:
   total+=i
 return total
print(fun(6))
```
- A) `9`
- B) `6`
- C) `12`
- D) `15`

**Q218. [H]** What does this print?
```python
def nested_check(n):
 ans=0
 for i in range(1,n+1):
  for j in range(1,3):
   if i%j==0:
    ans+=1
 return ans
print(nested_check(3))
```
- A) `3`
- B) `4`
- C) `5`
- D) `6`

**Q219. [M]** What does this print?
```python
def calculate(x,y):
 if x//y==2:
  return x%y
 else:
  return x+y
print(calculate(11,5))
```
- A) `2`
- B) `10`
- C) `1`
- D) `16`

**Q220. [H]** What does this print?
```python
def pattern_sum(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   if j%2==0:
    total+=j
 return total
print(pattern_sum(4))
```
- A) `6`
- B) `8`
- C) `12`
- D) `10`

**Q221. [M]** What does this print?
```python
def update(n):
 x=0
 for i in range(1,n+1):
  if i%3==0:
   x+=i
  else:
   x+=1
 return x
print(update(6))
```
- A) `13`
- B) `10`
- C) `11`
- D) `12`

**Q222. [E]** What does this print?
```python
def small(a,b):
 if a<b:
  return a*a
 else:
  return b*b
print(small(6,4))
```
- A) `36`
- B) `16`
- C) `10`
- D) `24`

**Q223. [M]** What does this print?
```python
def total_count(n):
 count=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if i==j:
    count+=i
 return count
print(total_count(4))
```
- A) `4`
- B) `6`
- C) `10`
- D) `16`

**Q224. [M]** What does this print?
```python
def mix(x):
 if x%2==0:
  if x>10:
   return x//2
  else:
   return x+2
 else:
  return x*2
print(mix(8))
```
- A) `4`
- B) `16`
- C) `8`
- D) `10`

**Q225. [H]** What does this print?
```python
def final(n):
 s=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   if (i+j)%2==0:
    s+=1
 return s
print(final(3))
```
- A) `4`
- B) `2`
- C) `3`
- D) `5`

**Q226. [H]** What does this print?
```python
def grid_score(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if i<j:
    total+=i*j
   else:
    total+=i-j
 return total
print(grid_score(3))
```
- A) `12`
- B) `15`
- C) `18`
- D) `21`

**Q227. [M]** What does this print?
```python
def calc(n):
 x=0
 for i in range(1,n+1):
  if i%2==0:
   x+=i//2
  else:
   x+=i*2
 return x
print(calc(5))
```
- A) `18`
- B) `20`
- C) `21`
- D) `25`

**Q228. [H]** What does this print?
```python
def series(n):
 s=0
 for i in range(1,n):
  for j in range(i,n):
   if (i+j)%3==0:
    s+=i+j
   else:
    s+=1
 return s
print(series(4))
```
- A) `10`
- B) `11`
- C) `15`
- D) `13`

**Q229. [M]** What does this print?
```python
def result(a,b):
 if a>b:
  if a%b==0:
   return a//b
  else:
   return a+b
 return b-a
print(result(14,5))
```
- A) `19`
- B) `2`
- C) `9`
- D) `70`

**Q230. [H]** What does this print?
```python
def triangle_sum(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   total+=i*j
 return total
print(triangle_sum(3))
```
- A) `18`
- B) `25`
- C) `21`
- D) `30`

**Q231. [H]** What does this print?
```python
def update(n):
 ans=0
 for i in range(1,n+1):
  if i%2==0 and i%3==0:
   ans+=i
  elif i%2==0:
   ans+=2
  else:
   ans-=1
 return ans
print(update(6))
```
- A) `5`
- B) `6`
- C) `7`
- D) `9`

**Q232. [M]** What does this print?
```python
def count_large(n):
 count=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if i*j>4:
    count+=1
 return count
print(count_large(3))
```
- A) `2`
- B) `4`
- C) `5`
- D) `3`

**Q233. [H]** What does this print?
```python
def while_calc(x):
 total=0
 while x>0:
  if x%2==0:
   total+=x//2
  else:
   total+=x
  x-=1
 return total
print(while_calc(5))
```
- A) `12`
- B) `10`
- C) `14`
- D) `15`

**Q234. [H]** What does this print?
```python
def loop_value(n):
 s=0
 for i in range(n):
  for j in range(n-i):
   if j==0:
    s+=i
   else:
    s+=j
 return s
print(loop_value(4))
```
- A) `12`
- B) `16`
- C) `14`
- D) `18`

**Q235. [M]** What does this print?
```python
def expression(a,b,c):
 if a+b*c>20:
  return (a+b)//c
 else:
  return a*b-c
print(expression(4,5,3))
```
- A) `3`
- B) `12`
- C) `17`
- D) `19`

**Q236. [M]** What does this print?
```python
def mix(n):
 p=1
 for i in range(1,n+1):
  if i%2==0:
   p*=i
  else:
   p+=i
 return p
print(mix(4))
```
- A) `20`
- B) `24`
- C) `32`
- D) `28`

**Q237. [H]** What does this print?
```python
def odd_even_grid(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if i%2==0:
    total+=j
   else:
    total-=j
 return total
print(odd_even_grid(3))
```
- A) `-6`
- B) `0`
- C) `6`
- D) `9`

**Q238. [H]** What does this print?
```python
def square_mix(n):
 s=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   if j==i:
    s+=i*i
   else:
    s+=j
 return s
print(square_mix(3))
```
- A) `14`
- B) `18`
- C) `16`
- D) `20`

**Q239. [H]** What does this print?
```python
def change(x,y):
 if x%2==0:
  y+=x//2
 if y%2==1:
  x+=y
 else:
  x-=y
 return x
print(change(8,3))
```
- A) `8`
- B) `11`
- C) `15`
- D) `18`

**Q240. [H]** What does this print?
```python
def count_score(n):
 c=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   if (i*j)%3==0:
    c+=2
   else:
    c+=1
 return c
print(count_score(4))
```
- A) `10`
- B) `12`
- C) `16`
- D) `14`

**Q241. [M]** What does this print?
```python
def limit_sum(n):
 s=0
 for i in range(1,n+1):
  if i*i>10:
   break
  s+=i*i
 return s
print(limit_sum(5))
```
- A) `14`
- B) `10`
- C) `20`
- D) `30`

**Q242. [H]** What does this print?
```python
def nested_math(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,4):
   if i+j>4:
    total+=i-j
   else:
    total+=i+j
 return total
print(nested_math(3))
```
- A) `16`
- B) `20`
- C) `18`
- D) `22`

**Q243. [M]** What does this print?
```python
def compute(a):
 result=0
 for i in range(1,a+1):
  if i%2==0:
   result=result+i*3
  else:
   result=result-i
 return result
print(compute(5))
```
- A) `6`
- B) `7`
- C) `9`
- D) `12`

**Q244. [H]** What does this print?
```python
def pair_sum(n):
 total=0
 for i in range(1,n+1):
  for j in range(1,n+1):
   if i+j<=n:
    total+=i+j
 return total
print(pair_sum(4))
```
- A) `16`
- B) `18`
- C) `24`
- D) `20`

**Q245. [H]** What does this print?
```python
def final_calc(n):
 ans=0
 for i in range(1,n+1):
  for j in range(1,i+1):
   if (i-j)%2==0:
    ans+=i-j
   else:
    ans+=i+j
 return ans
print(final_calc(3))
```
- A) `8`
- B) `12`
- C) `10`
- D) `14`

---

*End of Batch 5 — Q201–Q245. Difficulty: 4 [E] · 24 [M] · 17 [H]. Every answer verified by executing the code.*