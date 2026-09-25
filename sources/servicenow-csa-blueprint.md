# Source — CSA mainline exam blueprint (KB0011554)

This is the primary document the goal is built on, transcribed here. The PDF itself is kept on disk and out of git.

| | |
| :--- | :--- |
| What | Certified System Administrator (CSA) Mainline Exam Blueprint |
| Article id | KB0011554, English (Original) |
| Version | **Updated January 2026** |
| Obtained | 2026-09-25, as a 6-page PDF: `sources/Certified System Administrator (CSA) Mainline Exam Blueprint - ServiceNow University.pdf` |
| In git | **the PDF is not committed** — `sources/*.pdf` is in `.gitignore`. This file is the transcription that is committed |
| Preparation note | the document credits the exam questions to "official ServiceNow training materials and the ServiceNow Product documentation", and says study materials posted elsewhere online "are not official and should not be used to prepare for the examination" |

## Exam scope, transcribed verbatim

The document's own framing: "This table shows the exam domains, weightings, sub-topics, and the percentage of questions represented in each domain. The listed sub-skills should NOT be considered an all-inclusive list of the exam content."

| # | Exam domain | Sub-topics (verbatim) | Percent |
| ---: | :--- | :--- | ---: |
| 1 | Platform Overview and Navigation | ServiceNow Platform overview · Platform capabilities and services · The ServiceNow Instance · Next Experience Unified Navigation | 7% |
| 2 | Instance Configuration | Installing applications and plugins · Personalizing/customizing the instance · Common user interfaces in the Platform | 10% |
| 3 | Configuring Applications for Collaboration | Lists, Filters, and Tags · List and Form anatomy · Form Configuration · Form templates and saving options · Advanced Form Configuration · Task Management · Visual Task Boards (VTBs) · Visualizations, Dashboards, and Platform Analytics · Notifications | 20% |
| 4 | Self Service & Automation | Knowledge Management · Service Catalog · Workflow Studio · Virtual Agent | 20% |
| 5 | Database Management and Platform Security | Data Schema · Application/Access Control · Importing Data · CMDB and CSDM · Security Center · Shared Responsibility Model | 30% |
| 6 | Data Migration and Integration | UI Policies · Business Rules · System update sets · Scripting in ServiceNow | 13% |
| | **Total** | | **100%** |

## Exam structure, quoted

> The exam duration is 90 minutes.

> The exam consists of 60 questions.

> **Multiple Choice (single answer)** — For each multiple-choice question on the exam, there are at least three possible responses. Select the correct response.

> **Multiple Select (select all that apply)** — There are at least four possible responses for each multiple-select question on the exam. The question will state how many responses should be selected. Select ALL correct responses. Partial credit is not provided.

> Each question on the exam is worth one point. Your total score is compared to a predetermined cut score - this score is not publicly shared and is not always 70% - to determine a pass or fail outcome. **The section percentages on the exam result notification show how you performed in each domain, but they do not determine your overall result, should not be averaged, and do not indicate expertise.**

That last sentence governs how results are logged: the per-domain percentages are a report, never a readiness score, and are not to be averaged.

## Registration, quoted — and the clock it starts

> Registration = payment. This step secures your exam attempt.

> You can register at any time. Once registered, you have **90 days** to schedule and complete your exam.

> Exam fees are non-refundable. Register only when you are prepared to schedule your exam.

> From the My Exams page, you will be directed to **Pearson**. Choose to take your exam at a Pearson test center or online with **OnVUE**, where proctors observe via a webcam.

> If you do not complete your exam within 90 days, your registration will expire, and you will need to register and pay the full exam fee again.

The clock that matters is not a target date invented in advance: it is the **90-day window that starts at registration**, with a non-refundable fee. That is why this goal has no target date and is paced by testing results instead.

## Recommended preparation, and the official practice route

> ServiceNow recommends completing these training course(s): Welcome to ServiceNow · ServiceNow Administration Fundamentals

> Official practice exams are available through our trusted partner, MeasureUp — please refer to Knowledge Article KB0013408 for more information on how to access them.

Recommended experience, verbatim: "Three to six months of experience using and/or maintaining a ServiceNow instance."

Two consequences for this goal:

- **ServiceNow Administration Fundamentals** — the course already underway — is one of the two the vendor names
- **MeasureUp is the vendor's own practice route**, and therefore the most representative paper available when a checkpoint fires

Retakes require a waiting period and a fresh fee each attempt. Certification is maintained through annual delta exams and the yearly Certification Maintenance Program fee.

## Sample questions

The document publishes five sample items with answers: which application is available to all users, which module displays a group's not-yet-assigned tasks, the definition of transform maps, what type of elements Multiple Choice / Single Line Text / Select Box are, and the scripting language.

They are ServiceNow's own and are **not copied into `bank/`** — every bank entry is authored for this goal and verified against a cited passage. Their use here is stylistic only.
