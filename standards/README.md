# Standards

This directory documents every science-education standards system that Mission HydroSci can be aligned to. Each file describes one source of standards (national or state), captures the relevant standards verbatim where available, and maps them to MHS's internal objective codes (`W2.1`, `A3.1`, etc.) and the in-game activities they correspond to.

## Files

### National Framework

| File | Source | Coverage |
|---|---|---|
| [ngss.md](ngss.md) | Next Generation Science Standards | National framework; basis for ~22 states' standards. Contains the substantive PE-by-PE alignment to MHS for all 5 directly-cited PEs and 5 adjacent PEs, plus the SEP-7 argumentation thread. |

### Per-State Files (50 states + DC)

#### NGSS-direct or NGSS-equivalent (22 + DC)

For these states the alignment in `ngss.md` applies directly; per-state files note the local name, adoption year, and any state-specific framing:

| State | File | State | File |
|---|---|---|---|
| Arkansas | [arkansas.md](arkansas.md) | Maryland | [maryland.md](maryland.md) |
| California | [california.md](california.md) | Michigan | [michigan.md](michigan.md) |
| Connecticut | [connecticut.md](connecticut.md) | Nevada | [nevada.md](nevada.md) |
| Delaware | [delaware.md](delaware.md) | New Hampshire | [new-hampshire.md](new-hampshire.md) |
| District of Columbia | [dc.md](dc.md) | New Jersey | [new-jersey.md](new-jersey.md) |
| Hawaii | [hawaii.md](hawaii.md) | New Mexico | [new-mexico.md](new-mexico.md) |
| Illinois | [illinois.md](illinois.md) | Oregon | [oregon.md](oregon.md) |
| Indiana | [indiana.md](indiana.md) | Rhode Island | [rhode-island.md](rhode-island.md) |
| Iowa | [iowa.md](iowa.md) | Vermont | [vermont.md](vermont.md) |
| Kansas | [kansas.md](kansas.md) | Washington | [washington.md](washington.md) |
| Kentucky | [kentucky.md](kentucky.md) | | |
| Maine | [maine.md](maine.md) | | |

#### NGSS-influenced with state-specific frameworks (substantively close to NGSS)

These states use NGSS-derived three-dimensional structures with state-specific code formats. Alignment to MHS is via PE-by-PE crosswalk with NGSS:

| State | File | Notes |
|---|---|---|
| Alabama | [alabama.md](alabama.md) | 2023 Course of Study (3D) |
| Alaska | [alaska.md](alaska.md) | NGSS PEs with Alaska-specific clarifications |
| Arizona | [arizona.md](arizona.md) | AzSS 2018 (3D, NGSS-correlated) |
| Colorado | [colorado.md](colorado.md) | 2020 CAS (3D) |
| Idaho | [idaho.md](idaho.md) | Idaho Content Standards (3D) |
| Louisiana | [louisiana.md](louisiana.md) | LSS 2017 (3D, K-12 Framework) |
| Massachusetts | [massachusetts.md](massachusetts.md) | 2016 STE Framework (3D, NGSS-derived) |
| Minnesota | [minnesota.md](minnesota.md) | 2019 / adopted 2021 (3D) |
| Montana | [montana.md](montana.md) | 2016 (NGSS lead state, 3D) |
| Nebraska | [nebraska.md](nebraska.md) | NCCRS-S 2017 |
| New York | [new-york.md](new-york.md) | NYSSLS 2017 (NGSS + ~14 NY additions) |
| North Carolina | [north-carolina.md](north-carolina.md) | NCSCOS 2023 |
| North Dakota | [north-dakota.md](north-dakota.md) | 2019 (NGSS-based, 3D) |
| Oklahoma | [oklahoma.md](oklahoma.md) | OAS 2020 (3D) |
| Pennsylvania | [pennsylvania.md](pennsylvania.md) | STEELS 2022 (3D, NGSS-aligned) |
| South Carolina | [south-carolina.md](south-carolina.md) | 2021 (3D) |
| South Dakota | [south-dakota.md](south-dakota.md) | Near-copy of NGSS |
| Tennessee | [tennessee.md](tennessee.md) | TAS 2022 (NGSS lead state) |
| Utah | [utah.md](utah.md) | SEEd 2015 (3D) |
| West Virginia | [west-virginia.md](west-virginia.md) | WVCCR-S (built on NGSS) |
| Wisconsin | [wisconsin.md](wisconsin.md) | WSS 2017 (DPI affirms equivalence to NGSS) |
| Wyoming | [wyoming.md](wyoming.md) | 2016 (NGSS-modeled) |

#### Distinct frameworks (notably divergent from NGSS)

These states have standards that are not built on NGSS or differ structurally enough that per-state code mapping is required:

| State | File | Framework |
|---|---|---|
| Florida | [florida.md](florida.md) | NGSSS 2008 (predates NGSS, *not* the same despite the similar name) |
| Georgia | [georgia.md](georgia.md) | GSE 2016 (Georgia-specific) |
| Mississippi | [mississippi.md](mississippi.md) | MS CCRS 2018 (3-strand, Mississippi-specific) |
| Missouri | [missouri.md](missouri.md) | MLS 2016 — **the codes MHS curriculum docs cite natively** |
| Ohio | [ohio.md](ohio.md) | OLS 2018 (Ohio-specific scope) |
| Texas | [texas.md](texas.md) | TEKS 2021 (very different from NGSS; thinner MHS coverage) |
| Virginia | [virginia.md](virginia.md) | SOL 2018 (watershed standard 6.8 is a strong match) |

## Convention

Each per-state file includes:

1. **About** — who publishes it, adoption year, and how it is structured.
2. **Code format** and overall structure (grade-level vs. grade-band, three-dimensional vs. two-dimensional).
3. **Standards aligned to MHS** — verbatim text where available, with mappings to MHS objective codes (`W*` and `A*`) and in-game activities.
4. **Notable differences from NGSS** (where applicable).
5. **Recommended alignment strategy for deployment** in that state.
6. **Adoption & status**.
7. **Sources** at the bottom.

## Eventual Top-Level Document

The repo root will host a single document that consolidates these per-source views into one alignment matrix — for any given MHS objective (`W2.1`, `A3.1`, etc.) and any given state, you'll see which standards apply and at what depth. That document depends on the per-state files in this directory as its data source.
