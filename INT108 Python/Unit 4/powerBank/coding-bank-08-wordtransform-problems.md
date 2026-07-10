# Strings Coding Bank — Batch 8: Word-Level Transforms (141–160)

*Rewriting sentences one word at a time: filters, swaps, rotations, and rebuilds.*
*Judge-format: read input with `input()` in the exact order given (no prompt text), print exact-match output. Every output is a computed value — never a guessable label. Money/real values use `f"{x:.2f}"`. Difficulty: [E] easy · [M] medium · [H] hard.*
*Reference solutions in `coding-bank-08-wordtransform-solutions.md`.*

---

## 141 — Reverse Each Word  [M]

Reverse every word individually, keeping the word order.

**Input Format:** One line — a sentence.
**Output Format:** The sentence with each word reversed.

**Sample Input:**
```
abc def
```
**Sample Output:**
```
cba fed
```
---

## 142 — Pig-Latin Lite  [M]

Transform every word: move its first letter to the end and add `ay`.

**Input Format:** One line — a sentence of lowercase words.
**Output Format:** The transformed sentence.

**Sample Input:**
```
hello world
```
**Sample Output:**
```
ellohay orldway
```
---

## 143 — Capitalise Alternate Words  [M]

Capitalise the 1st, 3rd, 5th… words; leave the others as they are.

**Input Format:** One line — a sentence of lowercase words.
**Output Format:** The styled sentence.

**Sample Input:**
```
one two three four
```
**Sample Output:**
```
One two Three four
```
---

## 144 — Drop Short Words  [M]

Print only the words with at least `k` characters, in order (at least one word qualifies).

**Input Format:** Two lines — the sentence, then `k`.
**Output Format:** The filtered sentence.

**Sample Input:**
```
the cat jumped
4
```
**Sample Output:**
```
jumped
```
---

## 145 — Every Second Word  [E]

Print the 1st, 3rd, 5th… words, joined by spaces.

**Input Format:** One line — a sentence.
**Output Format:** The alternate words.

**Sample Input:**
```
a b c d e
```
**Sample Output:**
```
a c e
```
---

## 146 — First Word to End  [E]

Move the first word of a sentence to the end.

**Input Format:** One line — a sentence (at least two words).
**Output Format:** The rotated sentence.

**Sample Input:**
```
the cat sat
```
**Sample Output:**
```
cat sat the
```
---

## 147 — Duplicate Each Word  [M]

Print every word twice in a row.

**Input Format:** One line — a sentence.
**Output Format:** The doubled sentence.

**Sample Input:**
```
go home
```
**Sample Output:**
```
go go home home
```
---

## 148 — Word Lengths  [E]

Print the length of each word, joined by `-`.

**Input Format:** One line — a sentence.
**Output Format:** The lengths, dashed.

**Sample Input:**
```
hi there
```
**Sample Output:**
```
2-5
```
---

## 149 — Swap Adjacent Words  [H]

The sentence has an even number of words. Swap each pair: words 1↔2, 3↔4, …

**Input Format:** One line — a sentence with an even word count.
**Output Format:** The pair-swapped sentence.

**Sample Input:**
```
a b c d
```
**Sample Output:**
```
b a d c
```
---

## 150 — Title the Long Words  [M]

Capitalise only the words longer than 3 characters; shorter ones stay as they are.

**Input Format:** One line — a sentence of lowercase words.
**Output Format:** The selectively titled sentence.

**Sample Input:**
```
the quick cat ran fast
```
**Sample Output:**
```
the Quick cat ran Fast
```
---

## 151 — Shout the Longest  [H]

Print the sentence with the longest word (the first, if tied) in full uppercase and every other word unchanged.

**Input Format:** One line — a sentence.
**Output Format:** The sentence with one word shouted.

**Sample Input:**
```
we like coding a lot
```
**Sample Output:**
```
we like CODING a lot
```
---

## 152 — Ends of Each Word  [M]

For every word print its first and last characters joined; separate the words' results with spaces. (A one-letter word uses the same character twice.)

**Input Format:** One line — a sentence.
**Output Format:** The first+last pairs.

**Sample Input:**
```
hello world
```
**Sample Output:**
```
ho wd
```
---

## 153 — Word Report  [E]

Print each word on its own line, followed by a space and its length.

**Input Format:** One line — a sentence.
**Output Format:** One line per word: `word length`.

**Sample Input:**
```
hi there
```
**Sample Output:**
```
hi 2
there 5
```
---

## 154 — Remove a Word  [M]

Print the sentence with **every** occurrence of a given word removed (as a whole word). At least one word remains.

**Input Format:** Two lines — the sentence, then the word to remove.
**Output Format:** The cleaned sentence.

**Sample Input:**
```
the cat the dog
the
```
**Sample Output:**
```
cat dog
```
---

## 155 — Replace a Word  [M]

Replace every **whole word** equal to `old` with `new`. (Note how `ago` survives when replacing `go` — `s.replace` would have mangled it.)

**Input Format:** Three lines — the sentence, the old word, the new word.
**Output Format:** The rewritten sentence.

**Sample Input:**
```
go cat go
go
run
```
**Sample Output:**
```
run cat run
```
---

## 156 — Shortest Word  [M]

Print the shortest word of the sentence (the first, if tied).

**Input Format:** One line — a sentence.
**Output Format:** The shortest word.

**Sample Input:**
```
we all go far
```
**Sample Output:**
```
we
```
---

## 157 — Words Between  [H]

A sentence contains two marker words, each appearing exactly once (the first marker comes earlier). Print how many words lie strictly between them.

**Input Format:** Three lines — the sentence, the first marker, the second marker.
**Output Format:** The count of words between.

**Sample Input:**
```
start a b c end
start
end
```
**Sample Output:**
```
3
```
---

## 158 — Rotate Words Left  [H]

Rotate the words left by `k` places (words wrap to the end).

**Input Format:** Two lines — the sentence, then `k` (0 ≤ k ≤ word count).
**Output Format:** The rotated sentence.

**Sample Input:**
```
a b c d
1
```
**Sample Output:**
```
b c d a
```
---

## 159 — Camel Join  [M]

Join the words into one token: the first word lowercased, every later word capitalised, no spaces.

**Input Format:** One line — a sentence.
**Output Format:** The camelCase token.

**Sample Input:**
```
hello world now
```
**Sample Output:**
```
helloWorldNow
```
---

## 160 — Pad Words to Width  [H]

Find the longest word's length, then pad every word with `.` on the right to that length. Print the padded words separated by spaces.

**Input Format:** One line — a sentence.
**Output Format:** The aligned sentence.

**Sample Input:**
```
hi there you
```
**Sample Output:**
```
hi... there you..
```
---

*End of Batch 8 — 20 problems. Difficulty: 4 [E] · 11 [M] · 5 [H]. All reference solutions verified by execution.*