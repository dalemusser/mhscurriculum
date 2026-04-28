# Missouri Learning Standards (MLS) — Science

## About

The **Missouri Learning Standards (MLS) for Science** are the science standards adopted by the Missouri State Board of Education in **Spring 2016** and are published by the [Missouri Department of Elementary and Secondary Education (DESE)](https://dese.mo.gov/college-career-readiness/curriculum/missouri-learning-standards). Missouri did **not adopt NGSS directly**, but the MLS is heavily NGSS-derived; nearly every MLS code corresponds to an NGSS Performance Expectation in close-to-verbatim form.

**Code format:** `<grade-band>.<DCI-domain><DCI-number>.<sub-component>.<index>` — e.g. `6-8.ESS2.C.1` reads as "grade band 6–8, Earth & Space Science 2 (Earth's Systems), component C (The Roles of Water in Earth's Surface Processes), standard 1."

**Grade-band organization:** MLS publishes science standards by grade band (K–5, 6–8, 9–12), not by individual grade. Middle school is treated as a single 6–8 unit.

**Three-dimensional structure:** Like NGSS, each MLS standard integrates a Science and Engineering Practice (the verb at the start of the standard — "Develop a model," "Construct an explanation," etc.), a Disciplinary Core Idea (the topic), and an implicit Crosscutting Concept. MLS does not list the dimensions separately on each standard the way NGSS does.

**Why this file matters:** MHS curriculum docs cite standards using **MLS codes** (`6-8.ESS2.C.1`, etc.). Mapping these to NGSS in `ngss.md` lets us claim NGSS alignment in 20+ states. This file is the source of truth for the Missouri citations.

---

## Standards Directly Cited by MHS

### 6-8.ESS2.C.1

> **Design and develop a model to describe the cycling of water through Earth's systems driven by energy from the sun and the force of gravity.**

**Clarification:** Emphasis is on mechanical and chemical investigations with water and a variety of solid materials to describe the multiple pathways of the hydrologic cycle.

**NGSS equivalent:** [MS-ESS2-4](ngss.md#ms-ess2-4--cycling-of-water-through-earths-systems) — wording is identical except MLS uses "Design and develop" where NGSS uses "Develop."

**Cited in:** `docs/curriculum/Game Wide Docs/MHS Learning Progression.md`, `docs/curriculum/Game Wide Docs/Base Camp Tasks.md`

**MHS objectives served:** `W2.1`, `W2.2`, `W3.1`, `W3.2`, `W4.1`, `W4.2`, `W4.3`, `W5.1`

---

### 6-8.ESS3.A.1

> **Construct a scientific explanation based on evidence for how the uneven distributions of Earth's mineral, energy, and groundwater resources are the result of past and current geoscience processes and human activity.**

**Clarification:** Emphasis is on how these resources are limited and typically non-renewable, and how their distributions are significantly changing as a result of human activity.

**NGSS equivalent:** [MS-ESS3-1](ngss.md#ms-ess3-1--earths-resources). MLS adds "**and human activity**" as a cause; NGSS attributes only to "geoscience processes."

**Cited in:** MHS Learning Progression, Base Camp Tasks (cited as `6-8.ESS3.A`, no `.1` suffix in those docs)

**MHS objectives served:** Implicit framing for the entire game (groundwater is the prototypical unevenly-distributed resource); most directly tied to `W4.1`–`W4.3`.

---

### 6-8.ESS3.C.1

> **Analyze data to define the relationship for how increases in human population and per-capita consumption of natural resources impact Earth's systems.**

**Clarification:** Examples of data include grade-appropriate databases on human populations and the rates of consumption of food and natural resources (such as freshwater, mineral, and energy).

**NGSS equivalent:** [MS-ESS3-4](ngss.md#ms-ess3-4--population--per-capita-consumption). **Important difference:** MLS asks students to *analyze data* (SEP: Analyzing and Interpreting Data) where NGSS asks them to *construct an argument* (SEP: Engaging in Argument from Evidence). Same content, different practice. For MHS the NGSS framing is the better fit since the curriculum's argumentation arc culminates in argumentation, not data analysis.

**Cited in:** MHS Learning Progression (cited as `6-8.ESS3.C.1`)

**MHS objectives served:** Unit 6 human impacts; the unit-end argumentation activities.

---

### 6-8.ESS3.C.2

> **Apply scientific principles to design a method for monitoring and minimizing a human impact on the environment.**

**Clarification:** Examples of the design process include examining human environmental impacts, assessing the kinds of solutions that are feasible, and designing and evaluating solutions that could reduce that impact.

**NGSS equivalent:** [MS-ESS3-3](ngss.md#ms-ess3-3--monitoring-and-minimizing-human-impact) — verbatim match.

**Cited in:** MHS Learning Progression, Base Camp Tasks

**MHS objectives served:** Unit 3 pollution sensor placement, Unit 6 critique side quest, base-camp scenarios (fish hatchery, bug-tracking).

---

### 6-8.ETS1.A.1

> **Define the criteria and constraints of a design problem with sufficient precision to ensure a successful solution, taking into account relevant scientific principles and potential impacts on people and the natural environment that may limit possible solutions.**

**NGSS equivalent:** [MS-ETS1-1](ngss.md#ms-ets1-1--defining-a-design-problem) — verbatim match.

**Cited in:** Base Camp Tasks

**MHS objectives served:** `A1.1` (parts of an argument framed as a design problem with criteria); foundational for the entire argumentation arc.

---

## Adjacent MLS Standards (Not Cited but Aligned to MHS Content)

### 6-8.PS1.A.4 — Phase change with thermal energy *(strong adjacency — Unit 5)*

> **Develop a model that describes changes in particle motion, temperature, and state of a pure substance when thermal energy is added or removed.**

**Clarification:** Emphasis is on qualitative molecular-level models of solids, liquids, and gases to show that adding or removing thermal energy increases or decreases kinetic energy of the particles until a change of state occurs.

**NGSS equivalent:** [MS-PS1-4](ngss.md#ms-ps1-4--phase-change-with-thermal-energy-strong-adjacency--unit-5) — verbatim match.

**Why MHS hits this:** The U5 Toppo lesson on evaporation/condensation is a near-perfect implementation of this standard — uses NGSS phrasing about particle motion, energy, and state change.

**MHS objectives served:** `W5.1`

---

### 6-8.PS3.A.3 — Thermal energy transfer device *(moderate adjacency — Unit 5)*

> **Apply scientific principles to design, construct, and test a device that either minimizes or maximizes thermal energy transfer.**

**Clarification:** Examples of devices could include an insulated box, a solar cooker, and a Styrofoam cup.

**NGSS equivalent:** [MS-PS3-3](https://www.nextgenscience.org/pe/ms-ps3-3-energy)

**Why MHS hits this:** The U5 **solar still / desalinator** activity is exactly this standard — students learn that the sun heats salt water, water evaporates leaving salt behind, and the device traps the condensed fresh water.

**MHS objectives served:** `W5.1` (applied) — MHS does not have a dedicated thermal-engineering objective, but the solar still gameplay genuinely teaches this.

---

### 6-8.LS2.A.1 — Resource availability and population effects *(moderate adjacency — Unit 3 + base camp)*

> **Analyze and interpret data to provide evidence for the effects of resource availability on individual organisms and populations of organisms in an ecosystem.**

**Clarification:** Emphasis is on cause and effect relationships between resources and growth of individual organisms and the numbers of organisms in ecosystems during periods of abundant and scarce resources.

**NGSS equivalent:** [MS-LS2-1](ngss.md#ms-ls2-1--resource-availability-and-population-effects-moderate-adjacency--unit-3--base-camp) — verbatim match.

**Why MHS hits this:** U3 Tera seed-planting (water flow drives where superfruit seeds thrive) and U3 base-camp fish-hatchery scenarios.

**MHS objectives served:** `W3.1`, `W3.2`

---

### 6-8.LS2.C.1 — Ecosystem disruptions affect populations *(strong adjacency — Unit 6)*

> **Construct an argument supported by empirical evidence that explains how changes to physical or biological components of an ecosystem affect populations.**

**Clarification:** Emphasis is on recognizing patterns in data and making inferences about changes in populations.

**NGSS equivalent:** [MS-LS2-4](ngss.md#ms-ls2-4--ecosystem-disruptions-affect-populations-strong-adjacency--unit-6) — verbatim match.

**Why MHS hits this:** Unit 6's framing (human impacts to water systems and downstream ecosystem consequences) is exactly this standard. Pairs naturally with `6-8.ESS3.C.1`.

**MHS objectives served:** Unit 6 objectives.

---

### 6-8.LS2.C.2 — Evaluate ecosystem-maintenance solutions *(adjacent — Unit 6)*

> **Evaluate benefits and limitations of differing design solutions for maintaining an ecosystem.**

**NGSS equivalent:** Aligns conceptually with [MS-LS2-5](https://www.nextgenscience.org/pe/ms-ls2-5-ecosystems-interactions-energy-and-dynamics) (Evaluate competing design solutions for maintaining biodiversity and ecosystem services).

**Why MHS hits this:** Unit 6 critique activities and the broader human-impact framing. Less central than MS-LS2-4 but worth listing.

---

### 6-8.ETS1.B.1 — Evaluate competing design solutions *(strong adjacency — argumentation/critique)*

> **Evaluate competing design solutions using a systematic process to determine how well they meet the criteria and constraints of the problem.**

**NGSS equivalent:** [MS-ETS1-2](ngss.md#ms-ets1-2--evaluate-competing-design-solutions-strong-adjacency--argumentationcritique) — verbatim match.

**Why MHS hits this:** The Toppo Critique Side Quest is structurally exactly this standard — players critique fellow cadets' arguments against agreed-upon argumentation criteria.

**MHS objectives served:** `A5.1`, supporting `A3.1`–`A4.1`.

---

### 6-8.ETS1.B.2 / 6-8.ETS1.B.3 — Iterative design *(weak adjacency)*

> **6-8.ETS1.B.2:** Analyze data from tests to determine similarities and differences among several design solutions to identify the best characteristics of each that can be combined into a new solution to better meet the criteria for success.
>
> **6-8.ETS1.B.3:** Develop a model to generate data for iterative testing and modification of a proposed object, tool, or process such that an optimal design can be achieved.

**NGSS equivalents:** [MS-ETS1-3](https://www.nextgenscience.org/pe/ms-ets1-3-engineering-design), [MS-ETS1-4](https://www.nextgenscience.org/pe/ms-ets1-4-engineering-design)

**Why MHS hits this:** Light alignment via the iterative refinement that happens across the argumentation arc (each unit's argument informs the next). Not a strong claim but listed for completeness.

---

## Notable Differences from NGSS

1. **6-8.ESS3.A.1** explicitly includes "and human activity" as a cause of uneven resource distribution; NGSS MS-ESS3-1 attributes only to geoscience processes.
2. **6-8.ESS3.C.1** uses "Analyze data" (SEP: Analyzing and Interpreting Data) where NGSS MS-ESS3-4 uses "Construct an argument" (SEP: Engaging in Argument from Evidence). The argumentation framing in NGSS is a better match for MHS's argumentation pedagogy.
3. **MLS does not list the three dimensions explicitly** on each standard; the SEP is encoded in the verb of the standard. CCs are not enumerated separately. NGSS's three-dimensional layout is more directly usable for LLM evaluation prompts.
4. **MLS uses grade-band 6–8** with no per-grade specificity. NGSS does the same at middle school.

---

## Adoption & Status

- **Adopted:** Spring 2016 by the Missouri State Board of Education.
- **Successor / Revisions:** Missouri reviews standards on a roughly six-year cycle; verify current status at [DESE](https://dese.mo.gov/college-career-readiness/curriculum/missouri-learning-standards) before making alignment claims for compliance purposes.
- **Use in MHS:** The MHS curriculum team is at the University of Missouri; MLS codes are the native citation language in MHS curriculum docs.

---

## Sources

- [Missouri Learning Standards — DESE landing page](https://dese.mo.gov/college-career-readiness/curriculum/missouri-learning-standards)
- [MLS Science Standards Grades 6–12 (PDF, Spring 2016)](https://dese.mo.gov/sites/dese/files/media/pdf/2026/04/curr-mls-standards-sci-6-12-sboe-2016_AOD.pdf)
