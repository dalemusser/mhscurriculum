# Next Generation Science Standards (NGSS)

## About

The **Next Generation Science Standards** (NGSS) are a national consensus framework for K–12 science education in the United States, developed by Achieve, the National Research Council, the National Science Teachers Association, and the American Association for the Advancement of Science. They were first released in **April 2013** and are built on the *Framework for K-12 Science Education* (NRC, 2012).

NGSS is **voluntarily adopted** by states; the U.S. has no legally-binding national education standards. Around 20 states + DC use NGSS directly; most non-NGSS states publish their own standards but heavily borrow NGSS structure and content.

### Three-Dimensional Structure

Every NGSS Performance Expectation (PE) is a single integrated learning goal that combines three dimensions:

1. **Science and Engineering Practices (SEPs)** — 8 practices describing what scientists *do*. The MHS argumentation arc (objectives `A1.1`–`A5.1`) maps directly to **SEP 7: Engaging in Argument from Evidence**.
2. **Disciplinary Core Ideas (DCIs)** — the science content, organized as PS (Physical Science), LS (Life Science), ESS (Earth & Space Science), and ETS (Engineering, Technology & Applications of Science).
3. **Crosscutting Concepts (CCs)** — 7 concepts that bridge disciplines (Patterns; Cause and Effect; Scale, Proportion, and Quantity; Systems and System Models; Energy and Matter; Structure and Function; Stability and Change).

PE codes follow the pattern `<grade-band>-<DCI-domain><DCI-number>-<PE-number>`, e.g. `MS-ESS2-4` = Middle School, Earth and Space Science 2, Performance Expectation 4.

### Why NGSS is the natural anchor for MHS

Mission HydroSci's curriculum docs cite standards using **Missouri Learning Standards (MLS) codes** (e.g. `6-8.ESS2.C.1`) — but the underlying standards themselves are NGSS PEs in nearly verbatim form. Anchoring on NGSS first lets us:

- Cover ~20 states automatically.
- Crosswalk from NGSS to each non-NGSS state's framework via a single-step mapping rather than mapping each state directly to MHS.
- Use NGSS's three-dimensional structure to power LLM evaluation of student work (the dimensions tell the LLM what to look for: a model? a constructed explanation? an argument?).

---

## Performance Expectations Directly Cited by MHS

These five NGSS PEs are explicitly cited (in MLS notation) in `docs/curriculum/Game Wide Docs/MHS Learning Progression.md` and `docs/curriculum/Game Wide Docs/Base Camp Tasks.md`.

### MS-ESS2-4 — Cycling of Water Through Earth's Systems

> **Develop a model to describe the cycling of water through Earth's systems driven by energy from the sun and the force of gravity.**

| | |
|---|---|
| **MLS code in MHS docs** | `6-8.ESS2.C.1` |
| **Clarification** | Emphasis is on the ways water changes its state as it moves through the multiple pathways of the hydrologic cycle. Examples of models can be conceptual or physical. |
| **Assessment Boundary** | A quantitative understanding of the latent heats of vaporization and fusion is not assessed. |
| **SEP** | **Developing and Using Models** — *Develop a model to describe unobservable mechanisms.* |
| **DCI: ESS2.C — The Roles of Water in Earth's Surface Processes** | Water continually cycles among land, ocean, and atmosphere via transpiration, evaporation, condensation and crystallization, and precipitation, as well as downhill flows on land. Global movements of water and its changes in form are propelled by sunlight and gravity. |
| **CC** | **Energy and Matter** — *Within a natural or designed system, the transfer of energy drives the motion and/or cycling of matter.* |

**MHS objectives served:** `W2.1`, `W2.2`, `W3.1`, `W3.2`, `W4.1`, `W4.2`, `W4.3`, `W5.1` (essentially the entire Water Systems thread)
**MHS in-game activities:** Toppo lessons in Units 2–5, all glyph puzzles (topographic, watershed-flow, particle-dissolving, infiltration, evaporation), pollution sensor placement, well drill task, solar-still activity, all unit-end argumentation arguments

---

### MS-ESS3-1 — Earth's Resources

> **Construct a scientific explanation based on evidence for how the uneven distributions of Earth's mineral, energy, and groundwater resources are the result of past and current geoscience processes.**

| | |
|---|---|
| **MLS code in MHS docs** | `6-8.ESS3.A` |
| **Clarification** | Emphasis is on resource limitations and non-renewable status, with distributions changing significantly through human removal. Examples include petroleum, metal ores, and soil. |
| **SEP** | **Constructing Explanations and Designing Solutions** — *Construct a scientific explanation based on valid and reliable evidence obtained from sources (including students' own experiments) and the assumption that theories and laws that describe the natural world operate today as they did in the past and will continue to do so in the future.* |
| **DCI: ESS3.A — Natural Resources** | Humans depend on Earth's land, ocean, atmosphere, and biosphere for many different resources. Minerals, fresh water, and biosphere resources are limited, and many are not renewable or replaceable over human lifetimes. These resources are distributed unevenly around the planet as a result of past geologic processes. |
| **CC** | **Cause and Effect** — *Cause and effect relationships may be used to predict phenomena in natural or designed systems.* |

**MHS objectives served:** Implicit framing for the entire game — TK and crew are stranded on WAT247 specifically because water is unevenly distributed and they must find it. Most directly aligned with `W4.1`–`W4.3` (groundwater is the prototypical unevenly-distributed resource).
**MHS in-game activities:** Unit 4 well drill task, base camp well placement, Aryn's water collection sites in Unit 5, the Mission HydroSci framing premise.

---

### MS-ESS3-3 — Monitoring and Minimizing Human Impact

> **Apply scientific principles to design a method for monitoring and minimizing a human impact on the environment.**

| | |
|---|---|
| **MLS code in MHS docs** | `6-8.ESS3.C.2` |
| **Clarification** | Examples include water usage (withdrawal from streams/aquifers, dams, levees), land usage (urban development, agriculture, wetland removal), and pollution (air, water, land). |
| **SEP** | **Constructing Explanations and Designing Solutions** — *Apply scientific principles to design an object, tool, process or system.* |
| **DCI: ESS3.C — Human Impacts on Earth Systems** | Human activities have significantly altered the biosphere, damaging habitats and causing extinctions, though environmental changes have varied impacts on different organisms. As human populations and resource consumption increase, negative Earth impacts typically follow unless activities and technologies are engineered otherwise. |
| **CC** | **Cause and Effect** — *Relationships can be classified as causal or correlational, and correlation does not necessarily imply causation.* |

**MHS objectives served:** Unit 6 human impacts; pollution-tracking activities across U3.
**MHS in-game activities:** U3 pollution sensor placement, U6 critique side quest, base-camp fish-hatchery (U3) and bug-tracking (U5) tasks.

---

### MS-ESS3-4 — Population & Per-Capita Consumption

> **Construct an argument supported by evidence for how increases in human population and per-capita consumption of natural resources impact Earth's systems.**

| | |
|---|---|
| **MLS code in MHS docs** | `6-8.ESS3.C.1` |
| **Clarification** | Examples of evidence include grade-appropriate databases on human populations and the rates of consumption of food and natural resources (such as freshwater, mineral, and energy). Examples of impacts can include changes to the appearance, composition, and structure of Earth's systems as well as the rates at which they change. The consequences of increases in human populations and consumption of natural resources are described by science, but science does not make the decisions for the actions society takes. |
| **SEP** | **Engaging in Argument from Evidence** — *Construct an oral and written argument supported by empirical evidence and scientific reasoning to support or refute an explanation or a model for a phenomenon or a solution to a problem.* |
| **DCI: ESS3.C — Human Impacts on Earth Systems** | Typically as human populations and per-capita consumption of natural resources increase, so do the negative impacts on Earth unless the activities and technologies involved are engineered otherwise. |
| **CC** | **Cause and Effect** — *Cause and effect relationships may be used to predict phenomena in natural or designed systems.* |

**MHS objectives served:** Unit 6 (`Predict the spread of dissolved materials through a watershed` + `Identify and describe the human activities that have impacted the different water systems`); the entire argumentation arc culminates in a PE like this one.
**MHS in-game activities:** Unit 6 final argumentation, U3 pollution argument, all unit-end arguments that combine evidence into a claim.

---

### MS-ETS1-1 — Defining a Design Problem

> **Define the criteria and constraints of a design problem with sufficient precision to ensure a successful solution, taking into account relevant scientific principles and potential impacts on people and the natural environment that may limit possible solutions.**

| | |
|---|---|
| **MLS code in MHS docs** | `6-8.ETS1.A` |
| **SEP** | **Asking Questions and Defining Problems** — *Define a design problem that can be solved through the development of an object, tool, process or system and includes multiple criteria and constraints, including scientific knowledge that may limit possible solutions.* |
| **DCI: ETS1.A — Defining and Delimiting Engineering Problems** | The more precisely a design task's criteria and constraints can be defined, the more likely it is that the designed solution will be successful. Specification of constraints includes consideration of scientific principles and other relevant knowledge that are likely to limit possible solutions. |
| **CC** | **Influence of Science, Engineering, and Technology on Society and the Natural World** — *All human activity draws on natural resources and has both short and long-term consequences, positive as well as negative, for the health of people and the natural environment. The uses of technologies and limitations on their use are driven by individual or societal needs, desires, and values; by the findings of scientific research; and by differences in such factors as climate, natural resources, and economic conditions.* |

**MHS objectives served:** `A1.1` (parts of an argument framed as a design problem with criteria), foundational for all argumentation activities.
**MHS in-game activities:** U1 introduction to argumentation, all unit-end arguments (where claim/evidence/reasoning constraints are made explicit), critique side quest.

---

## Adjacent Performance Expectations

These NGSS PEs are not cited in the MHS curriculum docs but the in-game content directly addresses their substance. Including these in alignment claims would strengthen the case for MHS in any NGSS-adopting state.

### MS-PS1-4 — Phase Change with Thermal Energy *(strong adjacency — Unit 5)*

> **Develop a model that predicts and describes changes in particle motion, temperature, and state of a pure substance when thermal energy is added or removed.**

**Clarification:** Emphasis is on qualitative molecular-level models of solids, liquids, and gases to show that adding or removing thermal energy increases or decreases kinetic energy of the particles until a change of state occurs. Examples of models could include drawing and diagrams. Examples of particles could include molecules or inert atoms. Examples of pure substances could include water, carbon dioxide, and helium.

**SEP:** Developing and Using Models — *Develop a model to predict and/or describe phenomena.*
**DCIs:** PS1.A (states of matter — molecular structure), PS3.A (thermal energy and temperature)
**CC:** Cause and Effect — *Cause and effect relationships may be used to predict phenomena in natural or designed systems.*

**Why MHS hits this:** Unit 5's Toppo lesson on evaporation/condensation is **almost a perfect match for MS-PS1-4** — it walks through particle motion at a microscopic scale, energy added/removed, and state change. The Toppo Lesson Scripts even use the exact NGSS phrasing ("particles gain energy and begin to move faster and spread out"). Listing this PE makes Unit 5 alignment explicit.
**MHS objectives served:** `W5.1`
**MHS activities:** U5 Toppo lesson on evaporation/condensation, U5 dungeon temperature puzzles, solar still.

---

### MS-ESS2-2 — Geoscience Processes Shape Earth's Surface *(moderate adjacency — Unit 2)*

> **Construct an explanation based on evidence for how geoscience processes have changed Earth's surface at varying time and spatial scales.**

**Clarification:** Emphasis on processes changing Earth's surface at large scales (plate motions, mountain uplift) or small scales (landslides, geochemical reactions). Examples include weathering and deposition by water, ice, and wind movements affecting local geographic features.

**SEP:** Constructing Explanations and Designing Solutions
**DCI:** ESS2.A — *Earth's planet's systems interact over scales ranging from microscopic to global in size, operating over fractions of a second to billions of years.*
**CC:** Scale, Proportion, and Quantity — *Time, space, and energy phenomena can be observed at various scales using models to study systems that are too large or too small.*

**Why MHS hits this:** Unit 2 topography (W2.1) implicitly shows that landscape shape determines where water flows. Less central than MS-ESS2-4 but listing it strengthens Unit 2 alignment.
**MHS objectives served:** `W2.1`
**MHS activities:** Unit 2 topographic glyph puzzle, hovercraft assembly using terrain reading.

---

### MS-ETS1-2 — Evaluate Competing Design Solutions *(strong adjacency — argumentation/critique)*

> **Evaluate competing design solutions using a systematic process to determine how well they meet the criteria and constraints of the problem.**

**SEP:** **Engaging in Argument from Evidence** — *Evaluate competing design solutions based on jointly developed and agreed-upon design criteria.*
**DCI:** ETS1.B — *There are systematic processes for evaluating solutions with respect to how well they meet the criteria and constraints of a problem.*

**Why MHS hits this:** The Toppo Critique Side Quest (`docs/curriculum/Toppo Side Quest_ Critique Details/`) is structurally **exactly this PE** — players critique fellow cadets' arguments against agreed-upon argumentation criteria (claim + evidence + reasoning), and `A5.1` (counter-argument) is a direct expression of this practice.
**MHS objectives served:** `A5.1`, supporting `A3.1`–`A4.1`
**MHS activities:** Toppo Critique Side Quest, U5 counter-argument, all peer-critique dialogue interactions with Jasper / Tera / Anderson.

---

### MS-LS2-1 — Resource Availability and Population Effects *(moderate adjacency — Unit 3 + base camp)*

> **Analyze and interpret data to provide evidence for the effects of resource availability on organisms and populations of organisms in an ecosystem.**

**Clarification:** Emphasis is on cause and effect relationships between resources and growth of individual organisms and the numbers of organisms in ecosystems during periods of abundant and scarce resources.

**SEP:** Analyzing and Interpreting Data — *Analyze and interpret data to provide evidence for phenomena.*
**DCI:** LS2.A — *Organisms, and populations of organisms, are dependent on their environmental interactions both with other living things and with nonliving factors. In any ecosystem, organisms and populations with similar requirements for food, water, oxygen, or other resources may compete with each other for limited resources, access to which consequently constrains their growth and reproduction. Growth of organisms and population increases are limited by access to resources.*
**CC:** Cause and Effect

**Why MHS hits this:** Unit 3 seed-planting (Tera asks player to plant superfruit seeds in optimal locations based on watershed flow) and the base-camp fish-hatchery scenario are both about resource (water + nutrients) availability driving plant/population success.
**MHS objectives served:** `W3.1`, `W3.2`
**MHS activities:** U3 seed planting, U3 base-camp fish hatchery scenario, U5 base-camp bug-tracking.

---

### MS-LS2-4 — Ecosystem Disruptions Affect Populations *(strong adjacency — Unit 6)*

> **Construct an argument supported by empirical evidence that changes to physical or biological components of an ecosystem affect populations.**

**Clarification:** Emphasis is on recognizing patterns in data and making warranted inferences about changes in populations, and on evaluating empirical evidence supporting arguments about changes to ecosystems.

**SEP:** **Engaging in Argument from Evidence** — *Construct an oral and written argument supported by empirical evidence and scientific reasoning to support or refute an explanation or a model for a phenomenon or a solution to a problem.*
**DCI:** LS2.C — *Ecosystems are dynamic in nature; their characteristics can vary over time. Disruptions to any physical or biological component of an ecosystem can lead to shifts in all its populations.*
**CC:** Stability and Change — *Small changes in one part of a system might cause large changes in another part.*

**Why MHS hits this:** Unit 6 is explicitly about human-induced changes to water systems and their ecosystem consequences; pairs naturally with MS-ESS3-4.
**MHS objectives served:** Unit 6 objectives (human impacts on water systems)
**MHS activities:** U6 final argumentation, U3 pollution argument generalized.

---

## The Argumentation Thread: SEP 7 in MHS

MHS's six-unit argumentation arc (`A1.1`–`A5.1`) is a literal classroom implementation of **NGSS Science and Engineering Practice 7: Engaging in Argument from Evidence**, in its grade 6–8 progression. The mapping is essentially one-to-one:

| MHS objective | Unit | NGSS SEP 7 element (grades 6–8) |
|---|---|---|
| A1.1 — Identify and define the parts of a scientific argument | U1 | Foundational — identify components |
| A2.1 — Support a claim with evidence | U2 | *Construct, use, and present oral and written arguments supported by empirical evidence and scientific reasoning* |
| A3.1 / A3.2 — Identify and construct a warrant (reasoning) | U3 | Same SEP element — adding the warrant/reasoning component |
| A4.1 — Generate a complete argument (claim + evidence + reasoning) | U4 | Full SEP 7 expression |
| A5.1 — Provide a counter-argument to a faulty claim | U5 | *Compare and critique two arguments on the same topic and analyze whether they emphasize similar or different evidence and/or interpretations of facts.* + *Respectfully provide and receive critiques about one's explanations, procedures, models, and questions by citing relevant evidence and posing and responding to questions that elicit pertinent elaboration and detail.* |
| Unit 6 — Provide a counter-critique | U6 | *Evaluate competing design solutions based on jointly developed and agreed-upon design criteria* (= MS-ETS1-2 SEP) |

This means **any state's standards that include argumentation as a science practice** (which is essentially all of them, NGSS-derived or not) will align to MHS's argumentation thread without needing to cite a specific PE.

---

## State Adoption

States that have **adopted NGSS directly or substantively NGSS-based standards** — 22 states + DC:

> Arkansas, California, Connecticut, Delaware, District of Columbia, Hawaii, Illinois, Indiana (2022), Iowa, Kansas, Kentucky, Maine, Maryland, Michigan, Nevada, New Hampshire, New Jersey, New Mexico, Oregon, Rhode Island, Vermont, Washington

For these states, NGSS PE codes (e.g. `MS-ESS2-4`) are the alignment language; some states (Indiana, Kentucky) brand them under their own academic-standards name but the substance is NGSS. Each has a per-state file in this directory referencing this document.

States that have **their own standards influenced by NGSS** but use different code formats (each will have its own file in this directory):

> Alabama, Alaska, Arizona, Colorado, Florida (NGSSS — *not* NGSS), Georgia, Idaho, Louisiana, Massachusetts, Minnesota, Mississippi, Missouri (MLS), Montana, Nebraska, New York (NYSSLS — NGSS-based with additions), North Carolina, North Dakota, Ohio, Oklahoma, Pennsylvania (STEELS), South Carolina, South Dakota, Tennessee, Texas (TEKS), Utah, Virginia (SOL), West Virginia, Wisconsin, Wyoming

(State-by-state adoption status changes over time — verify current status when alignment matters for a deployment decision.)

---

## Sources

- [NGSS — Home](https://www.nextgenscience.org/)
- [MS-ESS2-4 — Earth's Systems](https://www.nextgenscience.org/pe/ms-ess2-4-earths-systems)
- [MS-ESS3-1 — Earth and Human Activity](https://www.nextgenscience.org/pe/ms-ess3-1-earth-and-human-activity)
- [MS-ESS3-3 — Earth and Human Activity](https://www.nextgenscience.org/pe/ms-ess3-3-earth-and-human-activity)
- [MS-ESS3-4 — Earth and Human Activity](https://www.nextgenscience.org/pe/ms-ess3-4-earth-and-human-activity)
- [MS-ETS1-1 — Engineering Design](https://www.nextgenscience.org/pe/ms-ets1-1-engineering-design)
- [MS-PS1-4 — Matter and Its Interactions](https://www.nextgenscience.org/pe/ms-ps1-4-matter-and-its-interactions)
- [MS-ESS2-2 — Earth's Systems](https://www.nextgenscience.org/pe/ms-ess2-2-earths-systems)
- [MS-ETS1-2 — Engineering Design](https://www.nextgenscience.org/pe/ms-ets1-2-engineering-design)
- [MS-LS2-1 — Ecosystems](https://www.nextgenscience.org/pe/ms-ls2-1-ecosystems-interactions-energy-and-dynamics)
- [MS-LS2-4 — Ecosystems](https://www.nextgenscience.org/pe/ms-ls2-4-ecosystems-interactions-energy-and-dynamics)
- *A Framework for K-12 Science Education* — National Research Council, 2012 (the foundational document NGSS is built on)
