# INT108 · Unit 3 — Build & Seed Plan

**Unit title (university-formal):** Functions and Recursion
**Course:** INT108 Python Programming · Mongo COURSE_ID `6a2e4cc57654e58bf4a0a105`
**Decisions locked:** full bespoke visualizer per lesson · build Lesson 01 end-to-end first as the reference sample, then 02–08 in that mold.

---

## 1. What already exists

- **Source content (done, ultra-premium):** `Material/INT108 Python/Unit 3/*.md` — 8 lesson bodies, MCQ + coding banks per lesson, `powerSkill/` (coding banks 01–04 + MCQ batches 1–9), 3 unit tests. Tone already matches the active bar.
- **The gap:** source is linear markdown. Active lessons are **helper-authored interactive HTML modules** + **DB-seeded MCQs/coding problems**. Porting = rewrite each `.md` → `lessons3/*.js`, add a live visualizer, then seed into Mongo.

## 2. System pipeline (confirmed — the exact live Unit-2 path)

There are two content tracks. **The live app course = the rich Mongo seed done by `src/scripts/seed-int108-unit2.js`** (imports the visualizer lesson modules), NOT the thin `int108Course/chapters/unit02.js`. We replicate the rich path.

Three source files per lesson, glued by one seeder:

- **Content module:** `courses/int108/lessons3/NN-slug.js` — exports `{ slug, title, subtitle, estimatedTime, demo, pills, hero, sections, scripts }`. Built from helpers: `_helpers.js` (`section, lead, p, callout, code, table, steps, mermaid`), `_book.js` (`walkthrough, mistakes, keypoints, typecards`), `_experience.js` (`predict, misconceptions, scenario, simple`), viz layer.
- **Assessment module:** `courses/int108/assessments3/NN-slug.js` — exports `{ slug, mcqs:[{level,label,question,code?,options,correctAnswer,explanation}], code:[{title,statement,inputFormat,outputFormat,constraints,starter,solution,tests:[{input,output,sample,explanation}]}] }`. Source = Material MCQ + coding banks. **Solutions compiler-verified** before seeding.
- **Visualizer CSS:** reuse `UNIT2_STYLES` (`.viz .term .statebox .verdict .fnode`) + add a small `_unit3-ui.js` for function-specific components (call-stack frames, scope boxes, param↔arg binding wires). Each lesson's `scripts` = self-contained IIFE building animation frames + Play/Step/Reset.
- **Seeder:** `src/scripts/seed-int108-unit3.js` = clone of `seed-int108-unit2.js`. Tag `int108-u3`, COURSE_ID `6a2e4cc57654e58bf4a0a105`. Finds the Unit 3 parent, deactivates old children (recoverable), builds tree **Unit 3 → Parts → topic(content) → MCQ + code children** via `buildAssessmentChildren` reading `assessments3/`. Idempotent, non-destructive, `--dry`. Run: `node src/scripts/seed-int108-unit3.js --dry` → verify → drop `--dry`.
- **Build (static HTML preview, optional):** `courses/int108/build-unit3.js` (clone `build-unit2.js`) → `unit3/*.html` for local eyeballing before seeding.
- **PowerSkill big bank (optional, phase 2):** Material `powerSkill/` (100+ coding, 9 MCQ batches) → `src/scripts/powersprint_u3/{mcq,code}.json` + `seed-u3-powersprint.js` (clone of `seed-u2p2-powersprint.js`) → one timed `Assignment` drawing N at random.

**Parts:** 3, matching the curriculum stages (each ends with an existing Material test):
Part 1 · What Functions Are (L01–03 · Test 1) · Part 2 · Using Functions Properly (L04–06 · Test 2) · Part 3 · Modules & Recursion (L07–08 · Test 3).

## 3. The 8 lessons (book-formal names → reference chapters)

| # | slug | Title | Ref | Visualizer |
|---|------|-------|-----|-----------|
| 01 | 01-introduction-to-functions | Introduction to Functions | 11.1–11.2 | 3 calls → 1 function, answers flow back |
| 02 | 02-built-in-functions | Built-in Functions | 11.3 | type conversion / coercion tracer |
| 03 | 03-user-defined-functions | User-Defined Functions | 11.4–11.8 | def→call flow-of-control stepper |
| 04 | 04-parameters-and-arguments | Parameters and Arguments | 11.9–11.14 | param↔arg binding + default fill-in |
| 05 | 05-return-values | Return Values | 11.15–11.19 | return vs print, value flows back |
| 06 | 06-scope-of-variables | Scope of Variables | 11.20–11.23 | local/global scope boxes, lifetime |
| 07 | 07-the-math-module | The Math Module | 12.14 + import | import → dot-call → result |
| 08 | 08-recursion | Recursion | 11.31 (full) | **call-stack unwind** + Fibonacci tree |

Then **3 tests** (`test-01..03`) + **powerSkill** banks → sprints.

## 4. Workflow order

1. **Scaffold** — `lessons3/`, `_unit3-ui.js`, `build-unit3.js`, `seed-int108-unit3.js` (placeholder lesson to prove pipeline).
2. **Lesson 01 end-to-end** — full module + bespoke visualizer + MCQs, `--dry` seed → **you approve the pattern.**
3. **Lessons 02–08** — port each `.md` in the approved mold, one visualizer each.
4. **Assessments** — MCQ + coding banks into DB schema.
5. **Tests + powerSkill** — port 3 tests + power banks as sprints.
6. **Seed + verify** — `--dry` → apply → run app, open Unit 3, confirm render + code judges.

## 5. Guardrails

- Do **not** touch or reseed Units 1–2 or any other course. Unit 3 only, tag `int108-u3`.
- No forward references: recursion/lists/etc. not used before taught.
- Titles stay university-syllabus-formal; tone stays academic/book. Match active Unit 2 voice.
