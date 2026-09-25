# 03 Configuring Applications for Collaboration

Objectives 03.1–03.9 (`GOAL.md` § Objectives). Weight 20%. **All four entries are `verified: yes`.**

## app-001 — narrowing a list with a condition
- objective: 03.1
- source: sources/servicenow-docs-excerpts.md § 03.1 — "You can create a filter to restrict what records appear in a list by providing a set of conditions." and "**To add a top-level condition** — Click AND or OR on the condition builder toolbar" (Brazil, updated 2026-09-10); objective 03.1 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You need a list to show only the records where the assignment group is Network and the state is not
     Closed, without touching the records themselves. What do you use?
- A: A filter, built with the condition builder: the selected field's type decides which operators and
  values are available, conditions combine with AND or OR, and Run applies the filter. Save keeps it for
  future use.
- Others: a tag is a text label associated with items like records and pages, used to group and organise
  them — it is not a condition; a breadcrumb narrows the list you are already looking at, and it carries
  conditions of its own, so it is a filter applied on top rather than a stored reusable one; a form layout
  decides which fields appear on a form, not which records appear in a list.
- to verify: whether the exam expects filters and breadcrumbs as distinct concepts. Sharing a filter with
  other users, or publishing it as a module, is **not** covered by the retrieved passage and must not be
  claimed from it.

## app-002 — where a form's related lists come from
- objective: 03.2
- source: sources/servicenow-docs-excerpts.md § 03.2 — "Related lists appear on forms and show records in tables that have relationships to the current record." (retrieved 2026-09-25); objective 03.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A form shows a list of related records underneath it, such as the tasks belonging to a request. What
     decides which related lists appear there?
- A: A form's configuration. Related lists appear on forms and show records in tables that have a
  relationship to the current record, and an administrator adds them by configuring the form.
- Others: the dictionary defines a table's fields and their types, not which related lists are shown on a
  form; an ACL decides who may see records; a UI policy changes a field's behaviour, not the related lists
  on display.
- note: the exam may want the underlying table relationship named rather than the act of configuring the
  form. The retrieved passage supports the second, which is what the key says.

## app-003 — which feature changes a form's layout
- objective: 03.3
- source: sources/servicenow-docs-excerpts.md § 03.3 — "Administrators or users with the personalize_form role can use the form design feature to quickly create new or change existing form views." (Brazil, updated 2026-09-10); objective 03.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You need to change which fields appear on an existing form, and in what order, for one view. Which
     feature does that work?
- A: Form design — the form designer — used to create new or change existing form views.
- Others: a UI policy changes a field's behaviour at run time rather than the layout; a list layout controls
  the columns of a list, not the fields of a form; the dictionary defines a field rather than where it
  appears on a form.
- to verify: whether the exam still expects form designer by that name, given the page says form designer is
  being prepared for deprecation in favour of Form Builder.

## app-004 — the base class behind Incident, Problem and Change
- objective: 03.6
- source: sources/servicenow-docs-excerpts.md § 03.6 — "The Task table is a base class that provides fields for the core ITSM applications such as Incident, Problem, and Change Management." (Brazil, updated 2026-09-10); objective 03.6 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: Add a new field to the Task table. It then appears on Incident, Problem and Change records. Why?
- A: Task is a base class: it provides fields for the core ITSM applications such as Incident, Problem and
  Change Management, and every application that extends it shares those fields in common.
- Others: they are not separate tables that happen to agree — they extend one base class; a form view only
  decides which of those fields are displayed, it does not create them; a dictionary override redefines
  something for one table rather than sharing it.
- to verify: the answer against the cited passage, and whether the exam tests the journal fields and the
  Reminder table that the same page lists.



