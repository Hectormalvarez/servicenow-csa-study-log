# ServiceNow Certified System Administrator (CSA)

Created 2026-09-25 · track `exam` · **no target date by choice** — paced by results, not by a calendar

## Source

| | |
| :--- | :--- |
| What | Certified System Administrator (CSA) Mainline Exam Blueprint, **KB0011554** — the objectives transcribed in `sources/servicenow-csa-blueprint.md` |
| Version | **Updated January 2026** |
| Obtained | 2026-09-25, as a PDF. The PDF itself is **gitignored**; the transcription is what lives in git |
| Course | ServiceNow University "ServiceNow Administration Fundamentals". The participant guide is an eBook behind a login and its platform does not allow export, so **its text is not available here**; the lab assets that came with the course are on disk, listed in `sources/course-materials-on-disk.md` |
| Where | `sources/` holds the passages the bank cites, and states plainly what could not be obtained |

**Re-check for a blueprint revision later than January 2026 before booking.** The objectives and weights in this file are transcribed from that document and agree with it statement for statement.

## Facts

| | |
| :--- | :--- |
| Questions | 60 — vendor-stated ("The exam consists of sixty questions") |
| Time | 90 minutes — vendor-stated |
| Types | multiple choice (single answer) with at least three responses, and multiple select with at least four — the multi-select says how many to pick and **partial credit is not provided** |
| Pass | a predetermined cut score, **not publicly shared and not always 70%**. The result is conditional and can be audited |
| Result report | a percentage per section is shown, and the document is explicit that these **do not determine the overall result, should not be averaged, and do not indicate expertise**. Logged here as a report, never as a readiness score |
| Delivery | Pearson — a test centre, or online with OnVUE where a proctor watches by webcam |
| Registration | registration **is** payment. Non-refundable, and it starts a **90-day window** to schedule and sit. Expiry means paying again |
| Practice papers | **MeasureUp** is the vendor's official practice partner (KB0013408) — the most representative paper available at a checkpoint |
| Recommended experience | three to six months using or maintaining an instance; the vendor names *Welcome to ServiceNow* and *ServiceNow Administration Fundamentals* as the courses |
| Target | **none, by the learner's choice** (2026-09-25) — pacing is by testing results, not by a calendar |
| Hours | shape approved 2026-09-25: the bulk **after work**, morning micro only. Proposed 45 min evening + 10 min morning, six days a week — the minutes still need a yes |
| Hands-on | the exam is scenario-driven and the learner uses ServiceNow daily at work. Lab results are logged as practice and are never counted as verified questions |

## Domains

| Key | Id prefix | Domain | Weight |
| :--- | :--- | :--- | ---: |
| `01-platform-navigation` | `pn` | Platform Overview and Navigation | 7 |
| `02-instance-configuration` | `ic` | Instance Configuration | 10 |
| `03-apps-collaboration` | `app` | Configuring Applications for Collaboration | 20 |
| `04-self-service-automation` | `ssa` | Self Service & Automation | 20 |
| `05-database-platform-security` | `db` | Database Management and Platform Security | 30 |
| `06-data-migration-integration` | `dmi` | Data Migration and Integration | 13 |

Weights total 100. Domain 05 alone is 30% — it gets the most session time by construction, not by preference.

## Objectives

Statements grouped by domain, transcribed **verbatim from the primary document** (KB0011554, updated January 2026, obtained 2026-09-25). One correction to what this section claimed earlier: the published document lists each domain's sub-topics **without individual ids**, so the ids used here (`01.1`, `05.6`, …) are sequential positions within a domain, assigned once by this goal and never renumbered. The wording is the document's, character for character; the numbering is this repo's bookkeeping.

### 01 Platform Overview and Navigation — 7%

- 01.1 ServiceNow Platform overview
- 01.2 Platform capabilities and services
- 01.3 The ServiceNow Instance
- 01.4 Next Experience Unified Navigation

### 02 Instance Configuration — 10%

- 02.1 Installing applications and plugins
- 02.2 Personalizing/customizing the instance
- 02.3 Common user interfaces in the Platform

### 03 Configuring Applications for Collaboration — 20%

- 03.1 Lists, Filters, and Tags
- 03.2 List and Form anatomy
- 03.3 Form Configuration
- 03.4 Form templates and saving options
- 03.5 Advanced Form Configuration
- 03.6 Task Management
- 03.7 Visual Task Boards (VTBs)
- 03.8 Visualizations, Dashboards, and Platform Analytics
- 03.9 Notifications

### 04 Self Service & Automation — 20%

- 04.1 Knowledge Management
- 04.2 Service Catalog
- 04.3 Workflow Studio
- 04.4 Virtual Agent

### 05 Database Management and Platform Security — 30%

- 05.1 Data Schema
- 05.2 Application/Access Control
- 05.3 Importing Data
- 05.4 CMDB and CSDM
- 05.5 Security Center
- 05.6 Shared Responsibility Model

### 06 Data Migration and Integration — 13%

- 06.1 UI Policies
- 06.2 Business Rules
- 06.3 System update sets
- 06.4 Scripting in ServiceNow

Thirty statements across six domains.

## Plan

**Shape approved 2026-09-25.** The learner's words: the bulk has to be **after work**; the morning is **getting ready** — cooking lunch and dinner — with maybe a quick quiz; and *"no date, let's go based strictly off testing results"*. **The shape is settled. The minutes below are still a proposal.**

The daily shape, built around a 04:00 wake-up, a 06:30–15:00 shift, then the gym — the minutes are the proposal, the shape is not:

| Block | Length | What it is for |
| :--- | ---: | :--- |
| evening, after work and the gym | 45 min | the bulk — yesterday's misses first, then due items, then new coverage on the highest-priority domain |
| morning, while cooking | 10 min | optional micro pass only: a quick retrieval set. Never new material, and skipped without guilt when the kitchen wins |
| one weekend block | 90 min | a full paper in the exam's shape, whenever a checkpoint fires |

Six days a week, one rest day: about 5.5 hours a week, with the evening block carrying roughly 80% of it. **The 45 and the 10 are the open question** — the learner has not named their minutes yet, and the next revision uses whatever they say.

Phases advance on their signal, never because a week went by:

| Phase | Advances when | Blocks |
| :--- | :--- | :--- |
| learning | domain 05 and domain 03 hold coverage, and the bank can fill a paper in the exam's shape | 1 × 45 min + 1 × 10 min, six days a week |
| immersion | paper #1 is scored and its misses are cleared | same daily blocks, a full paper each weekend until the decision |

Checkpoints fire on **state**, not on a date. No bar is in force until the learner approves it:

| Checkpoint | Fires when | Bar |
| :--- | :--- | :--- |
| paper #1 | the bank holds enough verified items to fill 60 questions in the exam's shape | none. A score in the 45–60% band is expected data, not failure |
| paper #2 | the misses from paper #1 are cleared | propose ≥ 70% |
| decision | two papers exist and the trend is rising | propose SIT after two papers at ≥ 75% · EXTEND below 70% |
| booking | a SIT recommendation is accepted | the learner sets the target date at that moment, re-checks for a blueprint revision newer than January 2026, and knows that **registering starts a non-refundable 90-day clock** |

**On papers, proposed and not in force:** the vendor's own practice route is **MeasureUp** (KB0013408), which makes it the most representative paper available. When a checkpoint fires, the two options are a MeasureUp practice exam or a paper assembled from this repo's bank — the bank route being the fallback while it is thin. Both are scored strictly, no partial credit. Which one is used is the learner's call, not mine.

Why it is shaped this way: the track is `exam`, so the driver is failure — papers come early and coverage fills in underneath them. With no date, the only honest trigger for a checkpoint is a state change: verified items in the bank, or a scored paper. The learner's aim of 2–3 weeks is theirs to hold, but I will not turn an aim into a deadline they never approved. If paper #1 lands below 45%, the shape of this plan is wrong, and the digest says so rather than moving a threshold.

## Verification

| | |
| :--- | :--- |
| Objectives | all 30 statements transcribed **verbatim** from the blueprint (KB0011554, updated January 2026). The id numbering is this repo's own, and `## Objectives` says so |
| Weights | 7 / 10 / 20 / 20 / 30 / 13 — read from the blueprint, summing to 100 |
| Format | 60 questions, 90 minutes, three or more responses per single-answer item, four or more per multi-select, no partial credit, Pearson delivery, cut score not published and not always 70% — all from the blueprint |
| Source passages | `sources/servicenow-docs-excerpts.md` cites a passage for **26 of the 30 objectives**, each from the public product documentation (release Brazil, updated 2026-09-10), and each stating what the page does and does not support |
| Questions | **26 in the bank, every one `verified: yes`** against its cited passage. Nothing is unverified or blocked |
| Not obtainable | the official participant guide — the eBook platform does not allow export. A question needing detail beyond an objective statement or a cited doc page would need that text |
| Still uncovered | 03.4, 03.5, 03.8 and 03.9 have no cited passage, 03.7 has a passage but no question, and commit order across several update sets is uncovered |
