# 01 Platform Overview and Navigation

Objectives 01.1–01.4 (`GOAL.md` § Objectives). Weight 7%. **All four entries are `verified: yes`.**

## pn-001 — the delivery model behind "your own instance"
- objective: 01.1
- source: sources/servicenow-docs-excerpts.md § 01.1 — "Services on the ServiceNow AI Platform are provided on a multi-instance basis, instead of running one instance with multiple users." (Brazil, updated 2026-09-10; authored text, not the page's AI summary block)
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: Each customer gets their own instance on one shared codebase, and the release cadence is the same for
     everyone. Which term does ServiceNow use for how the platform is delivered?
- A: Multi-instance. Services are provided on a multi-instance basis rather than running one instance with
  multiple users, and administrators can segregate data between business entities while every instance stays
  centrally managed.
- Others: "multi-tenant" is not the vendor's term for this; domain separation divides data *within* one
  instance rather than between customers; a personal developer instance is a free sandbox for learning, not
  a delivery model.

## pn-003 — what the strip at the top of every page is for
- objective: 01.4
- source: sources/servicenow-docs-excerpts.md § 01.4 — "The Next Experience Unified Navigation provides controls for navigating your instance, accessing records and data, checking notifications, and setting your preferences." (Brazil, updated 2026-09-10); objective 01.4 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: From anywhere in the interface you need to reach your workspaces, search the instance and change your own
     preferences. Where do those controls live?
- A: In the Next Experience Unified Navigation. It provides the controls for navigating the instance, for
  accessing records and data, for checking notifications and for setting preferences, and it appears at the
  top of every page.
- Others: a list's breadcrumb narrows the list you are looking at; the application menu reaches modules rather
  than your own preferences; a form's context menu acts on the one record open in front of you.
- to verify: whether the exam uses an older name for this region — earlier releases called it the banner
  frame. The cited page does not use that term, so it may not be keyed from here.

## pn-004 — where a partner-built application comes from
- objective: 01.2
- source: sources/servicenow-docs-excerpts.md § 01.2 — "Extend the platform through the ServiceNow Store, where partner-built applications and integrations are available for deployment." (Brazil, updated 2026-09-10); objective 01.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You want to add an application that a ServiceNow partner built, rather than build it yourself. Where is it
     available for deployment?
- A: The ServiceNow Store. Partner-built applications and integrations are available there for deployment, on
  top of the platform's own capabilities.
- Others: an update set carries your own configuration between instances — it is not where someone else's
  application comes from; the Admin Center is where administrators configure and manage the instance, not a
  source of applications; the platform's own capabilities are what the platform already provides, not what a
  partner adds.
- to verify: the answer against the cited passage. Deliberately dropped: any claim contrasting a plugin with
  an application, because the sources file records that no retrieved page draws that distinction.

## pn-005 — what a clone copies, and in which direction
- objective: 01.3
- source: sources/servicenow-docs-excerpts.md § 01.3 — "Clone copies data and metadata from one ServiceNow instance (source instance) to another ServiceNow instance (target instance)." (Brazil, updated 2026-09-10); objective 01.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A non-production instance needs refreshing with production data. Which way does the copy run, and what
     travels?
- A: From the production instance as the **source** to the non-production instance as the **target**, and it
  copies both data and metadata.
- Others: an update set carries configuration only, and never record data; an import set loads records from a
  file or a data source rather than from another instance; activating a plugin changes what the platform can
  do, not what data it holds.
- to verify: whether the exam tests cloning under this sub-topic at all. The blueprint's wording is "The
  ServiceNow Instance", which is broader than the page cited here — this is the closest documented page, not
  a perfect match for the sub-topic.

