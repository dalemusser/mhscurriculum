# Mission HydroSci Curriculum

This repository is the home for the **Mission HydroSci (MHS) curriculum**: the source materials provided by the MHS curriculum team, working documents derived from those sources, and reference material that supports the downstream systems that use MHS to evaluate and report on student learning.

Mission HydroSci is a 6-unit middle-school NGSS-aligned science game in which the player (cadet TK) and an AI companion (DANI) crash-land on planet WAT247 and must learn water science to survive. Across the six units the curriculum interleaves a **Water Systems** progression (topography → watersheds → pollution → groundwater → atmospheric water → human impacts) with an **Argumentation** progression (identify parts → claim+evidence → reasoning → full argument → counter-argument → counter-critique).

## What this repo is for

The work in this repo serves four related goals:

1. **Better dashboard messaging** — give teachers (via the [stratahub](https://github.com/dalemusser/stratahub) MHS Dashboard) clearer, more curricular feedback about what each student is doing well and where they need help.
2. **LLM-driven evaluation of student work and progress** — provide structured, well-organized curriculum information that an LLM can use to assess student responses and game-play traces.
3. **Supplemental activities and materials** — supply curriculum context that can be used to generate targeted resources for students who are under-performing on specific objectives.
4. **Human-readable understanding of how the game implements the curriculum** — make it easy to see, at any level of detail, what the curriculum goals are and how each in-game activity addresses them.

## How this repo connects to the rest of Mission HydroSci

| Repo | Role |
|---|---|
| **[mhscurriculum](.)** *(this repo)* | Curriculum source materials, working documents, and standards alignment |
| [mhsgrading](https://github.com/dalemusser/mhsgrading) | Per-progress-point grading rules (event keys, success/yellow nodes, reason codes, instructor messages) that consume student log entries |
| [stratalog](https://github.com/dalemusser/stratalog) | The logging service that ingests in-game events from the Unity game |
| [stratahub](https://github.com/dalemusser/stratahub) | The web app whose MHS Dashboard surfaces grades, color-coded progress, and instructor messages to teachers |

The flow is: **Unity game → stratalog → mhsgrading rules → stratahub dashboard.** This repo is the upstream curricular truth that the grading rules and dashboard messaging are derived from.

## Repository contents

### [`alignment-matrix.md`](alignment-matrix.md) — Standards ↔ MHS quick reference

A simplified two-direction matrix:
- **Standard → MHS:** for each NGSS Performance Expectation MHS targets, what unit, objective, and in-game activities implement it.
- **MHS → Standard:** for each MHS objective code (`W2.1`, `A3.1`, etc.), which standards it satisfies.

This is the document to start with when you want to see the alignment at a glance. Deeper detail lives in the per-source files in `standards/`.

### [`state-mismatches.md`](state-mismatches.md) — Where MHS and non-NGSS states diverge

The flip side of the alignment matrix. Documents, for the seven states whose science frameworks are substantively different from NGSS (TX, FL, VA, GA, OH, MS, MO), where MHS exceeds what the state requires and where the state requires content MHS does not cover. Includes deployment guidance and cross-cutting patterns (e.g., MHS consistently exceeds non-NGSS states on particle-level phase change and infiltration mechanics; MHS consistently does not cover plate tectonics, cellular biology, or forces/motion).

### [`standards/`](standards/) — Standards alignment

A complete documentation of every U.S. science-education standards system that MHS can be aligned to. Includes:

- **[`standards/ngss.md`](standards/ngss.md)** — the canonical Next Generation Science Standards alignment, with verbatim text for the 5 NGSS Performance Expectations directly cited by MHS, 5 adjacent PEs that MHS content addresses, and the SEP-7 argumentation thread that anchors `A1.1`–`A5.1` and Unit 6.
- **[`standards/missouri.md`](standards/missouri.md)** — Missouri Learning Standards (the codes MHS curriculum docs cite natively, since the MHS team is at the University of Missouri).
- **50 per-state files + DC** — every U.S. jurisdiction with its standards system, code format, adoption year, and alignment to MHS objectives.
- **[`standards/README.md`](standards/README.md)** — index and conventions for the directory.

### [`docs/curriculum/`](docs/curriculum/) — Curriculum source materials

The full set of curriculum documents provided by the MHS curriculum team, converted to Markdown with embedded images extracted alongside each document. Coverage includes:

- Per-unit curricular docs (Units 1–6)
- Toppo lesson scripts and per-unit lesson slides
- Game-wide docs (Teacher Guide, Learning Progression, Embedded Assessment, Loading Screen tips, Base Camp tasks, etc.)
- Side-quest content (Alien Glyphs, Aryn's Crates, DANI Charts, Tera Side Quest, Toppo Critique Side Quest)
- Assessment instruments and pre/post-test codebooks
- Followup activities

This is the canonical curriculum source for the repo — every other working document, including the standards alignment in [`standards/`](standards/), is derived from these materials.

### [`ai/`](ai/) — AI assistant context

[`ai/context.md`](ai/context.md) is an orientation document for AI assistants working in this repo: it describes the curriculum structure, how the various pieces connect (game → stratalog → mhsgrading → stratahub), and known data quirks worth being aware of when working with the source materials.

## What's coming

The per-source standards files in `standards/` are step one. The next layer of work consolidates them into a single top-level alignment matrix — given any MHS objective code (`W3.1`, `A4.1`, etc.), the matrix will show every state's standards that the objective satisfies, plus the in-game activities and grading touchpoints that demonstrate it. Other planned working documents will support the four goals above.
