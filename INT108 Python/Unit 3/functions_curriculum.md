# Functions — Course Outline

## Stage 1 — What Functions Are (Lessons 01–03)

| # | Lesson | Content covers | MCQ | Coding |
|---|--------|----------------|:---:|:------:|
| 01 | **Introduction to Functions** | Why functions exist; the four advantages (reusability, modularity, easy debugging, readability), each shown with a before/after code pair — same task written twice vs. written once as a function. | 5 | — |
| 02 | **Built-in Functions** | `print`, `input`, `int`, `float` (formalizing what they've used all unit); new: `len`, `type`, `str`, `max`, `min`, `sum`, `round` — incl. `round()` banker's-rounding note tying back to the `:.2f` recipe, and `len(str(n))` as a one-line digit count vs. their loop. | 5 | 5 |
| 03 | **User-Defined Functions** | `def`, call, body, naming rules; definition runs nothing until called; calling twice; flow-of-control diagram. | 5 | 5 |

**→ TEST 1: Function Fundamentals** (after 03) — theory + built-ins + first defs; the natural first checkpoint.

> **Note:** Lesson 01 gets no coding block — there's no function syntax yet to code with, so per the "if it naturally fits" rule, it's content + MCQ only.

---

## Stage 2 — Using Functions Properly (Lessons 04–06)

| # | Lesson | Content covers | MCQ | Coding |
|---|--------|----------------|:---:|:------:|
| 04 | **Parameters & Arguments** | Parameter vs. argument (the vocabulary distinction, tested explicitly); positional order matters; keyword arguments; default arguments incl. defaults-must-come-last `SyntaxError`. | 5 | 5 |
| 05 | **Return Values** | No-return functions return `None` (the `print(f())` → `None` trap); return vs. print as the flagship confusion; return exits immediately; returning multiple values with `x, y = f()` unpacking (light touch, no tuple theory). | 5 | 5 |
| 06 | **Scope of Variables** | Local vs. global; parameters are local; lifetime; shadowing; the `UnboundLocalError` mistake; `global` keyword shown once and discouraged. | 5 | 5 |

**→ TEST 2: Parameters, Returns & Scope** (after 06) — these three are one conceptual cluster; scope bugs only make sense once returns exist.

---

## Stage 3 — Modules & Recursion (Lessons 07–08)

| # | Lesson | Content covers | MCQ | Coding |
|---|--------|----------------|:---:|:------:|
| 07 | **Math Module** | `import math`; dot syntax; `sqrt`, `pow`, `ceil`, `floor`; the `math.pow` returns a float trap (`math.pow(2,3)` → `8.0`); `ceil`/`floor` vs. `//` and their old ceiling-division trick; `sqrt` + `:.2f`. | 5 | 5 |
| 08 | **Recursion** | Meaning; base condition; recursive call; stack-working diagram (new PNG type: call-stack unwind); recursive factorial and Fibonacci with full trace tables + Fibonacci call tree; advantages vs. limitations table; `RecursionError` from a missing base case. | 5 | 5 |

**→ TEST 3: Math Module & Recursion**
