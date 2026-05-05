# Assessment Item Types — Status (2026-05-05)

This document captures the current state of the MHS pre/post-test item-type categorization after the curriculum team's 2026-05-05 review of [`assessment-item-types.md`](assessment-item-types.md) and [`assessment-item-types-comparison.md`](assessment-item-types-comparison.md).

---

## Where we are now

The categorization is **resolved and locked**. The MHS curriculum team has reviewed both documents and confirmed (with one correction) their Spring 2026 categorization. Eric on the curriculum team:

1. **Clarified the rationale for placing items 32, 33, 34, 35, 42, 43, 44 in Arg Alignment.** It is *not* simply because there is a picture on the page. It is because the question challenges the student to determine **which argument piece would fit with a picture that represents student thinking**. In items 32–35 the pictures depict what two students think happened to the dissolved sugar; the question presents argument pieces (e.g., pieces of evidence) and asks which fits each student's picture. Items 42–44 are the same construct with a different scenario.
2. **Agreed item 39 belongs in Arg Alignment**, not Identification (the prior team mapping had item 39 in Identification, while my categorization had it in Alignment). Eric has updated the team's record.

The team's current authoritative mapping for the **Argumentation Assessment** is:

| Concept | Items | Count |
|---|---|---:|
| Identification | 26, 27, 28, 29, 36, 37, 38, 45, 46, 47, 48 | 11 |
| Arg Alignment | 25, 32, 33, 34, 35, 39, 42, 43, 44, 49 | 10 |
| Critique/Evaluation | 30, 31, 40, 41, 50, 51 | 6 |

The **Water Systems Assessment** mapping is unchanged from the previous round (full leaf-level agreement was already established):

| Concept | Items | Count |
|---|---|---:|
| Ground Water | 1, 2, 10, 11 | 4 |
| Atmospheric Water | 3, 8, 19, 20, 21, 22 | 6 |
| Water Cycle | 4, 5, 7 | 3 |
| Surface Water (Watersheds) / Topography | 6, 9, 12, 13, 14, 15, 16, 17, 18, 23, 24 | 11 |

---

## What changed in `assessment-item-types.md`

The previous version of the file used my own categorization, which differed from the team's mapping on 8 items in Section 3 (and previously included a flagged inconsistency on item 39). It is now updated to match the team's authoritative mapping.

### Section 3 — Argumentation (substantive changes)

| Change | Detail |
|---|---|
| Renamed buckets | "Structure" → **Identification**; "Alignment" → **Arg Alignment**; "Critique" → **Critique/Evaluation** |
| Items 32, 33, 34, 35 | Moved from Structure → **Arg Alignment** |
| Items 42, 43, 44 | Moved from Structure → **Arg Alignment** |
| Item 39 | Stays in the alignment-equivalent bucket (now **Arg Alignment**) — matches my original placement; the team confirmed it on this round |
| Definitions | Rewrote the Identification vs. Arg Alignment definitions per Eric's clarification: Arg Alignment is about aligning an argument piece with a **representation of student thinking**, not about whether a picture appears on the page |

### Section 2 — Water Systems (presentational changes only)

| Change | Detail |
|---|---|
| Atmospheric Water | Now shown as its own top-level category alongside Water Cycle (matching the team's mapping). Previously it was folded into Water Cycle with a sub-split. |
| Note added | Folding Atmospheric Water back into Water Cycle recovers Jim's original four-category framing; that view is also mentioned in the coverage summary. |

No item moved between Section 2 buckets — Section 2 was already in full leaf-level agreement with the team in the previous round.

### Other changes

- Headline note at the top of the document now states the categorization reflects the team's Spring 2026 authoritative mapping (refined on 2026-05-05).
- The "Notes on the Categorization" section was rewritten under the team's definitions, replacing my earlier "Structure vs. Alignment" framing.

---

## Resolution of the previous open questions

The earlier comparison document (`assessment-item-types-comparison.md`) flagged two open questions. **Both are now resolved.**

### 1. Item 39 vs. Item 49 — RESOLVED

The previous team mapping placed item 39 in Identification but item 49 in Arg Alignment, despite their structural parallel ("which [statement/evidence] contradicts [character]'s representation?"). Eric agreed item 39 should be in Arg Alignment and has updated the team's record. Both items now sit in Arg Alignment, where their parallel structure suggests they belong.

### 2. Working definition of Identification vs. Arg Alignment — RESOLVED

My inferred rule was "written-source = Identification; picture-source = Arg Alignment." Eric refined this:

> The line is not whether a picture is on the page — it is whether the question challenges the student to determine which argument piece fits with a **representation of student thinking**.

In practice this produces the same classification as the picture-source heuristic for the current items, but the underlying construct is **alignment between an argument piece and a representation of thinking**. That is the construct the team is measuring, and it is what the rule should be stated as for any new items.

For the current 51 items, every Arg Alignment item satisfies the team's construct:

- **Item 25** — students align each piece of information with the cadet (Matt vs. Cathy) whose idea it supports.
- **Items 32–35** — students align an argument piece (claim or evidence) with each student's picture of what happened to the dissolved sugar.
- **Item 39** — students identify which statement contradicts Laura's representation.
- **Items 42–44** — same construct as 32–35 with a different scenario.
- **Item 49** — students identify which evidence contradicts Amanda's representation.

---

## What this means for downstream work

For the four mhscurriculum goals (dashboard messaging, LLM-driven evaluation, supplemental-activity targeting, curriculum→game wiring), the team's mapping in [`assessment-item-types.md`](assessment-item-types.md) is now the canonical concept-to-item index.

- **Dashboard messaging.** Pre/post performance can be reported by the team's three argumentation concepts (Identification, Arg Alignment, Critique/Evaluation), each carrying distinct learning meaning. Identification weakness implies the student can't pick parts of an argument out of written prose; Arg Alignment weakness implies the student can't connect argument pieces to a representation of thinking; Critique/Evaluation weakness implies the student can't judge between two argument quality levels.
- **LLM evaluation prompts.** Concept-level prompts should use the team's labels and item lists.
- **Supplemental-activity targeting.** Per-concept targeting can use the team's mapping directly.
- **Future items.** Any new pre/post-test items should be classified per the team's refined Arg Alignment definition (does the item ask the student to align an argument piece with a representation of thinking?) rather than by stem inspection or codebook tag alone.

The codebook itself still tags every Identification *and* Arg Alignment item with the single label `Identification`. Anyone consuming the codebook tags directly downstream will need this document (or the team's mapping) to recover the team's three-way split.

---

## Open questions

**None at this time.** The two questions raised in the comparison document are resolved. The categorization is the team's, and the working definitions are the team's. If new items are added or scenarios evolve in a future revision of the assessment, the categorization should be re-confirmed with the team at that time.

A possible follow-up worth noting (not blocking):

- **Codebook update.** The codebook (`MHS pre-test_10.14.25_codebook_clean.md` and post-test counterpart) still uses a single `Identification` tag for items the team now splits into Identification vs. Arg Alignment. If downstream consumers read the codebook directly, they will not see the three-way split. A future codebook revision could introduce an explicit `Arg Alignment` tag to make the split machine-readable; the team would decide whether that is worth doing for the next assessment cycle.
