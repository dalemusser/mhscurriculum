# MHS Curriculum Repository Context

This repo is the home for **Mission HydroSci (MHS) curriculum**: source materials provided by the MHS curriculum team, working documents derived from them, and reference material that supports the downstream systems that use MHS to evaluate and report on student learning.

The curriculum content in **`docs/curriculum/`** is the canonical source for everything in this repo. Other repos consume this material indirectly:

- **[stratalog](https://github.com/dalemusser/stratalog)** — receives in-game log events (`logdata` collection in MongoDB) emitted by the Unity game and the dialogue/quest system.
- **[mhsgrading](https://github.com/dalemusser/mhsgrading)** — encodes the grading rules per unit/progress-point (event keys, success/yellow nodes, reason codes) that consume those log entries.
- **[stratahub](https://github.com/dalemusser/stratahub)** (MHS Dashboard feature) — surfaces the resulting per-student scores, color (green/yellow/red), and instructor messages to teachers/leaders.

---

## Game-wide framing

- **Mission HydroSci (MHS)** is a 6-unit middle-school science game (NGSS grades 6–8). Setting: spaceship cadet TK and AI companion DANI crash-land on planet WAT247 and must learn water science to survive.
- **NPC cast:** Captain **Toppo** (delivers lessons), **DANI** (AI companion), **Anderson**, **Tera**, **Aryn**, **Jasper** (other cadets, each tied to a different side quest).
- **NGSS standards directly cited:** `MS-ESS2-4` (water cycle), `MS-ESS3-1` (uneven distribution of resources), `MS-ESS3-3` / `MS-ESS3-4` (human impact, monitoring), `MS-ETS1-1` (engineering design). Cited in MHS docs using Missouri Learning Standards format (`6-8.ESS2.C.1`, etc.) — see `standards/missouri.md`.
- **Two intertwined progressions:**
  1. **Water Systems (W):** topography → watersheds → pollution flow → groundwater → water cycle/atmosphere.
  2. **Argumentation (A):** identify parts → claim+evidence → reasoning/warrant → full CRE argument → counter-argument/critique.

## Unit map (titles match `mhsgrading/`)

| Unit | Title | Topic | Water LOs | Arg LO |
|---|---|---|---|---|
| 1 | Get Your Space Legs | Argumentation intro | — | A1.1 (parts of argument) |
| 2 | Find the Flow | Watersheds / topography | W2.1, W2.2 | A2.1 (claim+evidence) |
| 3 | Clean the Stream | Pollution / soluble materials | W3.1, W3.2 | A3.1, A3.2 (reasoning/warrant) |
| 4 | Dig Deeper | Groundwater / infiltration | W4.1, W4.2, W4.3 | A4.1 (full CRE argument) |
| 5 | Rise and Return | Atmospheric water / water cycle | W5.1 | A5.1 (counter-argument) |
| 6 | (Human Impacts) | Human impacts wrap-up | — | Provide counter-critique |

Unit 6 has a 2.0 curricular doc but is **not yet present in `mhsgrading/`** — only U1–U5 have point-level grading rules.

## Progress points (the grading unit)

The `mhsgrading/` repo breaks each unit into numbered **progress points** (e.g. U2P1 "Escape the Ruin"). For each point a markdown file defines:

- **Trigger event key** (start/end) — e.g. `questFinishEvent:21`
- **Success node** event key (green if present)
- **Yellow nodes** (any present → yellow grade)
- **Reason codes** with short/long instructor messages and teacher guidance
- **Three scripts** per point: data-analytics (Python), analytics-matching (Mongo JS), production attempt-windowed (Mongo JS), the last using the previous trigger event as the attempt window's start so a replay re-grades correctly.
- **Reason-code parameter quantities** (e.g. `{attempts_number}`, `{wrong_number}`) substituted into the instructor message.

Reason codes used so far: `WRONG_ARG_SELECTED`, `MISSING_SUCCESS_NODE`, `TOO_MANY_NEGATIVES`, `BAD_FEEDBACK`, `HIT_YELLOW_NODE`. Authoritative table: `mhsgrading/Reason-codes-and-instructor-messages.md`.

Unit-start anchors live in `mhsgrading/mhs-unit-start.md` (e.g. Unit 1 = `questActiveEvent:28`).

---

## Top-level repo layout

| Path | What it is |
|---|---|
| `README.md` | Repo home page; describes purpose and links to the working sets below. |
| `docs/curriculum/` | **Canonical curriculum source materials.** Markdown rendering of every doc the MHS curriculum team provided, with embedded images extracted alongside. |
| `standards/` | Standards alignment — one file per U.S. standards system, plus the master `ngss.md` document. See `standards/README.md` for the index. |
| `ai/context.md` | This file. |
| `LICENSE` | Repo license. |

The original `.docx` / `.pptx` / `.pdf` source files (formerly under `docs/OriginalCurriculum/`) were removed once the Markdown rendering in `docs/curriculum/` was validated. **`docs/curriculum/` is now the single source of truth** for curriculum content; if a re-render is ever needed, the originals would have to come back from the curriculum team.

---

## Key foundational docs in `docs/curriculum/`

### Game-wide (`Game Wide Docs/`)
- **`MHS 2.0 Embedded Assessment.md`** — the score-calculation table (Unit / Topic / Task / Student Action / Log Tag / Score formula). Each row corresponds to a graded in-game activity. This is the bridge from curriculum → log events → scores. (Updated working version: `MHS 2.0 Embedded Assessment Working Doc.md`.)
- **`MHS Learning Progression.md`** — master objectives table (W2.1–W5.1, A1.1–A5.1) with curricular element progression and embedded + post-game assessment items per LO.
- **`Mission HydroSci Teacher Guide.md`** and the *Last Minute Manual* (PDF-derived: `MHS Last Minute Manual - Draft - 12May2025.docx.md`) — full teacher-facing manuals. The Teacher Guide PDF was image-heavy; the extracted Markdown captures the table of contents and prose, but specific figures may need to be opened in the original PDF if it is reintroduced.
- **`MHS FT2 Teacher Guide.md`** (DOCX-derived) and **`MHS FT2 Teacher Guide.pdf.md`** (PDF-derived) — earlier (FT2) field-test guide; the two suffixes resolve a basename collision between the same content in DOCX and PDF form.
- **`Loading Screen Content.md`** — 36 numbered "Toppo Tips" organized by unit, shown on loading screens.
- **`Updates to Orientation Course.md`** — Canvas orientation course updates needed; flags Module 5 (assessment) needs rework for **Abt** (replacing Qualtrics) and Module 6 (Dashboard) needs to reflect the new dashboard.
- **`Base Camp Tasks.md`** — U3 fish-hatchery, U4 well-placement, U5 bug-tracking base-camp scenarios that tie human-impact LOs back to specific units.
- **`Backing Info.md`** — placeholder/visual references for in-game backing-information tools (per unit).
- **`Animal Side Quest Descriptors.md`** — side-quest descriptors.
- **`Curriculum Alignment Brainstorm.md`** — alignment brainstorming.
- **`Water Science Assessment Instrument.md`** — full assessment instrument (also `Assessment/(OLD) ...` and `Assessment/Annotated ...`).

### Per-unit curricular docs (`Unit N Curriculum Docs/`)
Each unit has both a **1.0** and a **2.0 Revision** curricular doc (U1 has 2.0 only, U6 has 2.0 only). These define driving question, underlying facts/principles, target ideas vs. **alternative conceptions/misconceptions** (with literature citations), learning resources, extension activities, and assessment items mapped to the LO. The 2.0 versions are the current source of truth.

### Toppo Lessons (`Toppo Lessons/` + `Toppo Lesson Scripts.md`)
- Per-unit Markdown (U1–U5, derived from PPTX) with proposed slide updates for MHS 2.0; Miro source: `https://miro.com/app/board/uXjVM22X5Lc=/`.
- `Toppo Lesson Scripts.md` contains the canonical NEW lesson scripts at target Flesch–Kincaid grade levels (mostly 5.5–6, U5 evap/cond at 7.3) plus the older v1 scripts for reference. Lessons: U1 Argumentation; U2 Topography; U3 Watersheds; U3 Water Flow; U4 Soil Infiltration; U5 Evaporation/Condensation; U5 Water Cycle (which also covers the solar desalinator).

### Toppo Side Quest — Critique (`Toppo Side Quest_ Critique Details/`)
- `Argumentation Side Quest_ Design Documentation.md` — design for the cross-unit critique side quest where the player critiques other cadets' flawed arguments. Rewards = uniform unlocks tied to in-game ranks (Deck Cadet → Third/Second/First Mate → Honorary Captain) at 2/5/9/13/all arguments completed.
- `2.0 {Anderson U4-U5, Jasper U2-U5, Tera U3-U5} Critique Scenario.md` — per-character critique sequences. (1.0 versions in subfolder.)

### Side-quest content
- **Alien Glyphs** (`Alien Glyphs/`) — per-unit puzzle requirements + glyph-feedback markdown (U2–U5). Glyphs are in-room puzzles where the player assembles topographic/watershed/pollution/infiltration concept models; outcome routes through the dialogue system and emits success/yellow nodes.
- **Aryn's Crates** (`Aryn_s Crates/`) — U2/U3 crate placement locations + dialogue feedback (U3 = the "Supply Run" progress point).
- **DANI Charts** (`DANI Charts/`) — U2–U4 DANI dialogue/data-display chart designs.
- **Tera Side Quest** (`Tera Side Quest/`) — U2–U5 dialogue + feedback markdown.
- **Mini Game (Curricular)** — `Mini Game Brainstorm.md`, `Nanomachine Mini-Game Topography.md`, side-quest curricular ideas.
- **`Checkpoint Breakdown.md`** — every checkpoint by unit (U1.C1 … U2.C20 etc.) with start/end conditions; defines save-point granularity. Note: ends with "POTENTIAL REVISION DUE TO TEACHER DASHBOARD DISCUSSIONS," i.e. checkpoint definitions are still in flux based on dashboard needs.

### Followup activities (`FollowUp PPTs/`)
- `Argumentation Introduction 2.0.md`, `Argumentation Review.md` — out-of-game argumentation lessons.
- `U2/U3/U4/U5 Followup.md` — per-unit teacher-led followup discussions reinforcing the unit's embedded activity.

### Assessment (`Assessment/`)
- `FINAL/MHS pre-test_10.14.25_codebook_clean.md` and `FINAL/MHS post-test_10.14.25_codebook_clean.md` — finalized 10/14/2025 codebooks for the pre/post Water Science Assessment Instrument. Item codes follow `S{section}Q{n}` plus topic tag (e.g. `S2Q3; atmospheric water`). Items 1–11 = water systems; 12+ topographic-map / watershed; later items cover argumentation. Demographics in S1 (grade, age, sex, ethnicity, race).
- Earlier revisions: `MHS 2 Assessment revisions_2024.md`, `(OLD) Water Science Assessment Instrument.md`, `Annotated Assessment.md`.

### Archive (`Archive/`)
Historical/superseded materials: old curricular visuals, U1–3 to-do/questions/concerns, July-2023 topographic character hunt PPT.

---

## Standards alignment (`standards/`)

`standards/` documents every U.S. science-education standards system MHS can be aligned to. One file per source. Index at `standards/README.md`.

- **`standards/ngss.md`** — the substantive PE-by-PE alignment to NGSS for the 5 directly-cited Performance Expectations and 5 adjacent PEs, plus the SEP-7 argumentation thread that anchors `A1.1`–`A5.1` and Unit 6. This is the canonical alignment document; states that adopt NGSS or NGSS-equivalent standards (~22 states + DC) point back to it.
- **`standards/missouri.md`** — Missouri Learning Standards. The MHS team is at the University of Missouri, and the curriculum docs in `docs/curriculum/` cite Missouri-format codes (`6-8.ESS2.C.1` etc.). This file is the source of truth for the codes appearing in curriculum docs.
- **48 other per-state files** — every U.S. state and DC, with adoption status, code format, and alignment-to-MHS notes.

The eventual top-level alignment matrix (planned, not yet built) will consolidate these per-source files into a single view: per MHS objective code (`W3.1`, `A4.1`, etc.), see every state's standards that the objective satisfies, plus the in-game activities and grading touchpoints that demonstrate it.

---

## Reading patterns / known data quirks

- **`docs/curriculum/` is Markdown, not source files.** Office docs (`.docx`/`.pptx`) were converted with `pandoc -t gfm --wrap=none` and embedded images extracted to `<base>.media/` next to each Markdown file (image refs are relative and render in any Markdown viewer). PDFs were converted with `pdftotext -layout` and saved with `.md` extensions; their content is plain text but valid Markdown. Where a docx and pdf share a basename, the PDF version uses `<base>.pdf.md` to avoid collision.
- **Many `.media/` folders are large** (most of the ~227 MB working set is extracted PNGs from PowerPoint slides). When grepping curriculum content, restrict to `*.md` to avoid noise.
- **PPTX-derived Markdown loses positional layout.** Slide numbers and headings are present, but multi-column layout, callouts, image labels, and speaker-note hierarchies are flattened. If layout matters, the originals are no longer in this repo — they would need to be requested from the curriculum team.
- **PPTX-derived Markdown has many images per slide deck.** A short-looking text body is often paired with dozens of images in `<base>.media/` — don't assume low-line-count = low content.
- **Docs reference Miro** (`https://miro.com/app/board/uXjVM22X5Lc=/`) as the live update target; the local copies describe themselves as drafts.
- **Two parallel naming conventions in `mhsgrading/` vs `docs/curriculum/`.** Curriculum docs use checkpoint codes like `U2.C7`. Grading docs use progress points like `U2P1`. They are *not* a 1:1 mapping — progress points are a coarser grain (e.g. `U2P1` "Escape the Ruin" covers `U2.C6+C7+C8` from the checkpoint breakdown). When linking curriculum text to a grading rule, use **activity name** + **trigger event key**, not the checkpoint code.

## Cross-repo wiring

```
Unity game → emits events → stratalog (logdata coll, fields: game="mhs", playerId, eventKey)
                                              ↓
                  mhsgrading rules (event keys, success/yellow nodes, reason codes)
                                              ↓
                  stratahub MHS Dashboard feature → green/yellow/red + instructor messages
```

Event-key shape: `DialogueNodeEvent:{node}:{branch}`, `questFinishEvent:{n}`, `questActiveEvent:{n}`. The grading scripts query `db.logdata` directly. Production scripts use **attempt windowing** (latest trigger as window end, previous trigger as window start) so replay regrades cleanly — the analytics-matching scripts do *not* window and will count all-time occurrences.

## Open / in-flight items found during review

- Unit 6 has a 2.0 curricular doc but **no point-level grading** in `mhsgrading/` yet.
- `MHS 2.0 Embedded Assessment.md` rows for U4 (water table, argumentation, critique, groundwater), U5 (argumentation, four evap/conden tasks), and U6 (evidence alignment, critique, argumentation) have **empty Student Action / Log Tag / Score columns** — score formulas not yet defined.
- Updates to Orientation Course flags Module 5 (Abt assessment workflow) and Module 6 (new dashboard) as **major** rewrites still needed.
- Toppo Side Quest design doc has unresolved "Topics for Discussion" (rewards mechanics, U4 arg out-of-date, no U5 critique content written yet).
- `Checkpoint Breakdown.md` ends with "POTENTIAL REVISION DUE TO TEACHER DASHBOARD DISCUSSIONS" — checkpoints may shift to align with dashboard needs.
- Top-level alignment matrix that consolidates the per-state files in `standards/` is planned but not yet built.
