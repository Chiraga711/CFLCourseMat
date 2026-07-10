# INT108 · Unit 3 — Per-Lesson Design Blueprint

**Unit:** Functions and Recursion · **Course:** INT108 (Mongo `6a2e4cc57654e58bf4a0a105`) · tag `int108-u3`
**Locked template (from approved Lesson 01):** every lesson is built only from the active-content palette —
`hero · simple(one-line) · section · lead · runExample(side-by-side) · walkthrough(line-by-line) · mistakes(avoid↔instead) · callout(incl. Memory hook + Real-world) · table · typecards · cheat · mermaid · keypoints` **+ at least one bespoke live visualizer.**

## The fixed shape every lesson follows

1. **Hero** — headline + 2 intro paragraphs + 3 stat chips
2. **`simple()`** — the whole idea in one line
3. **The problem** — why this topic exists (a pain the student already feels)
4. **Core teaching** — concept → `runExample` → `walkthrough`, built up in small sections
5. **Bespoke visualizer** — the watch-it-run centrepiece (see per-lesson below); a 2nd viz where it earns its place
6. **Real-world example** — code they’d actually ship (`callout` "why" + runExample)
7. **Common beginner mistakes** — `mistakes()` cards, each Avoid ↔ Instead + the *why*
8. **Memory hook** — a `tip` callout with a mnemonic
9. **Quick reference** — glossary `table` + do/don't `cheat`
10. **Summary** — `keypoints` + one-line bridge to the next lesson

Assessments live in the tab, not the page: **5 MCQ + 5 coding** per lesson (Lesson 01 = 5 MCQ, 0 coding — no syntax yet). Sourced from Material MCQ/coding banks; every coding solution compiler-verified before seeding.

---

## Unit architecture — a three-act journey (Beginner → Mastery)

Tagline: **"From copy-paste to a toolkit that thinks."** Mapped to Course Outcome **CO3**. Three acts, each closing with a milestone checkpoint, then a capstone that fuses everything.

| Act | Difficulty | Lessons | Promise | Milestone |
|---|---|---|---|---|
| **I · Foundations of Functions** | Beginner → Core | 01 · 02 · 03 | Read function-based programs, use built-ins, write & call your own | 🏁 Checkpoint 1 · Function Fundamentals |
| **II · Designing Robust Functions** | Core | 04 · 05 · 06 | Pass data in cleanly, return answers for reuse, reason about scope | 🏁 Checkpoint 2 · Parameters, Returns & Scope |
| **III · Modular Code & Recursion** | Core → Mastery | 07 · 08 | Pull power from the math module, solve problems with recursion | 🏁 Checkpoint 3 · Math Module & Recursion |
| **🏆 Capstone · Function Toolkit** | Mastery | project | Ship a reusable library solving the syllabus practicals | badge / portfolio piece |

Each **Act landing page** shows: a difficulty badge, a "🎯 By the end you can…" promise, the ordered subtopics, and a "🏁 Milestone" banner naming the checkpoint. The **Unit landing page** shows the full three-act roadmap + capstone, colour-coded, under a CO3 badge. *(Both already wired in `seed-int108-unit3.js`.)*

---

## Act I · Foundations of Functions

### 01 · Introduction to Functions  ✅ built
- **Concepts:** why functions exist; the four advantages (reusability, modularity, easy debugging, readability); built-in vs user-defined; define vs call.
- **Visualizers:** (1) **call-flow** — 3 calls flow through one `digit_sum` body, digits peel, answers flow back; (2) **growth simulator** — slider drives copy-paste bar (5 lines each) vs flat function bar.
- **Real-world:** online store 18% GST → one `final_price()`.
- **Mistakes:** define-but-never-call · copy-paste-instead-of-call.
- **Memory hook:** DRY vs WET. · **MCQ 5 · Code 0.**

### 02 · Built-in Functions
- **Concepts:** formalize `print`, `input`, `int`, `float`; new `len`, `type`, `str`, `max`, `min`, `sum`, `round`; type conversion & coercion; `round()` banker's-rounding tie to `:.2f`; `len(str(n))` as one-line digit count vs their loop.
- **Visualizer:** **function machine** — pick a built-in from a dropdown, feed a value, watch input → box → output + resulting `type`. Second mini-demo: `round()` banker's-rounding (2.5→2, 3.5→4) side by side with naive expectation.
- **Real-world:** shopping cart total with `sum()` + `round(total, 2)` for a rupee-accurate bill.
- **Mistakes:** `round(2.5)` "should be 3" surprise · `int("3.5")` ValueError vs `int(float("3.5"))`.
- **Memory hook:** "`str→int→float` — widen, never assume." · **MCQ 5 · Code 5.**

### 03 · User-Defined Functions
- **Concepts:** `def`, name, body, the call; naming rules; **definition runs nothing until called**; calling twice; flow-of-control.
- **Visualizer:** **flow-of-control stepper** — highlight how `def` only *registers*, then a call *jumps* into the body, runs it, and *returns* to the exact next line in the caller (arrows animate the jump down and back).
- **Real-world:** a `greet(name)` used across a login, a welcome email, and a dashboard header.
- **Mistakes:** missing colon / indentation · calling before defining (NameError).
- **Memory hook:** "Define = teach the recipe. Call = cook it." · **MCQ 5 · Code 5.**

---

## Act II · Designing Robust Functions  → **Checkpoint 1** after 03, **Checkpoint 2** after 06

### 04 · Parameters and Arguments
- **Concepts:** parameter vs argument (tested explicitly); positional order matters; keyword arguments; default arguments incl. **defaults-must-come-last `SyntaxError`**.
- **Visualizer:** **argument-binding animator** — arguments fly into parameter slots by position; toggle to keyword mode and watch them reorder correctly; a default value auto-fills an empty slot.
- **Real-world:** `book_ticket(movie, seats=1, snack="none")` — defaults for the common case.
- **Mistakes:** wrong positional order (silent wrong result) · a default before a non-default (`SyntaxError`).
- **Memory hook:** "Position is where; keyword is which." · **MCQ 5 · Code 5.**

### 05 · Return Values
- **Concepts:** no-return → `None` (the `print(f())` → `None` trap); **return vs print** (flagship confusion); return exits immediately; returning multiple values with `x, y = f()` unpack (light touch).
- **Visualizer:** **two-lane flow** — `return` lane stores a value into a variable (reusable, glows), `print` lane emits to the terminal and is gone. Step a function and watch which lane fires. Mini-demo: code after `return` never runs.
- **Real-world:** `calculate_tax()` that *returns* so the total can be reused, vs one that only prints and dead-ends.
- **Mistakes:** `print` inside function then trying to reuse the "answer" · code written after `return`.
- **Memory hook:** "`print` = show the user. `return` = hand it to the program." · **MCQ 5 · Code 5.**

### 06 · Scope of Variables
- **Concepts:** local vs global; parameters are local; lifetime; shadowing; `UnboundLocalError`; `global` shown once and discouraged.
- **Visualizer:** **scope boxes** — a global frame; on a call a local frame appears holding its own variables; on return the local frame **vanishes** (greys out). Shadowing shown as a same-named variable living in two boxes. `UnboundLocalError` demo.
- **Real-world:** a running `score` — why a function’s local `score` doesn’t clobber the global one.
- **Mistakes:** expecting a local to survive after return · assigning to a global inside a function → `UnboundLocalError`.
- **Memory hook:** "What’s born inside, dies inside." · **MCQ 5 · Code 5.**

---

## Act III · Modular Code & Recursion  → **Checkpoint 3** after 08

### 07 · The Math Module
- **Concepts:** `import math`; dot syntax; `sqrt`, `pow`, `ceil`, `floor`; **`math.pow(2,3)` → `8.0` float trap**; `ceil`/`floor` vs `//` and the old ceiling-division trick; `sqrt` + `:.2f`.
- **Visualizer:** **import & dot-call** — an `import math` brings a labelled `math` box on screen holding `sqrt · pow · ceil · floor · pi`; `math.sqrt(16)` reaches into the box and returns `4.0`. Toggle showing what’s NOT available without the import (NameError).
- **Real-world:** distance between two points with `math.sqrt`; rounding seats up with `math.ceil`.
- **Mistakes:** `sqrt(16)` without `math.` (NameError) · expecting `math.pow(2,3)` to be `8` not `8.0`.
- **Memory hook:** "Import the toolbox, then reach in with a dot." · **MCQ 5 · Code 5.**

### 08 · Recursion  ← the flagship
- **Concepts:** meaning; base condition; recursive call; **call-stack unwind**; recursive factorial & Fibonacci with full trace tables + Fibonacci call tree; advantages vs limitations; `RecursionError` from a missing base case.
- **Visualizers (two):** (1) **call-stack animator** — frames *push* as `factorial(4)→factorial(0)` descends to the base, then *pop and return* unwinding back up (4→3→2→1 multiplying out); (2) **Fibonacci call tree** — the branching tree grows, showing repeated sub-calls (why naive fib is slow).
- **Real-world:** folder-inside-folder traversal; "countdown then blast-off" as the base case.
- **Mistakes:** missing/rong base case → `RecursionError` (stack overflow) · recursing without moving toward the base.
- **Memory hook:** "Every recursion needs a way OUT (base) and a way DOWN (smaller call)." · **MCQ 5 · Code 5.**

---

## 🏆 Capstone · Build Your Own Function Toolkit  (Mastery)

A single guided project that fuses every skill in the unit and doubles as the student’s first reusable library — the "wow" the client remembers. Straight from the syllabus **List of Practicals**, so it is fully in scope.

- **Brief:** build `toolkit.py`, a small module of clean, reusable functions:
  `is_perfect(n)`, `is_armstrong(n)`, `factorial(n)` (recursive), `fibonacci(n)` (recursive), `is_palindrome(s)`.
- **Ties together:** `def` + parameters (03/04) · `return` for reuse (05) · local scope discipline (06) · a `math` helper (07) · recursion with a base case (08).
- **Premium extras:** a live **"toolkit console"** visualizer — call any toolkit function from a dropdown and watch its result; a walkthrough of turning five separate scripts into one importable module; a "ship it" checklist.
- **Assessment:** 1 multi-part coding problem + a short reflection MCQ set. Optionally feeds the **powerSkill mega-bank** (`powersprint_u3`).

---

## Build order (per approved plan)

Author each lesson as `lessons3/NN-slug.js` + `assessments3/NN-slug.js`, register in `build-unit3.js` + `seed-int108-unit3.js`, build → eyeball HTML → move on. New per-lesson viz CSS goes in `_unit3-ui.js`. After 08: wire the 3 tests, optionally the powerSkill mega-bank (`powersprint_u3`), then `seed --dry` → apply. Nothing outside Unit 3 is touched.

## Totals

8 lessons · ~11 bespoke visualizers · 7×(5 MCQ) + 5 = **40 MCQ** · 7×5 = **35 coding** · 3 tests · optional powerSkill bank (100+ coding, 9 MCQ batches from Material).
