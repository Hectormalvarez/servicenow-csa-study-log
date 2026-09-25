# 06 Data Migration and Integration

Objectives 06.1–06.4 (`GOAL.md` § Objectives). Weight 13%. **All five entries are `verified: yes`.**

## dmi-001 — moving your own configuration between instances
- objective: 06.3
- source: sources/servicenow-docs-excerpts.md § 06.3 — "When the update set is completed, you can transfer the update set to another instance" (retrieved 2026-09-25); objective 06.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You configured a table, a form layout and a business rule on a sub-production instance. You need the
     same configuration in production. What carries it, and what does previewing it show you?
- A: An update set. Changes are recorded into it on the development instance, the completed set is
  transferred to the other instance, and there it is retrieved, previewed and committed. The preview is what
  lets an administrator compare the set against what is already there and resolve conflicting changes before
  they land.
- Others: activating a plugin adds vendor capability rather than carrying your changes; exporting and
  importing records moves data rather than configuration; a clone copies an entire instance's database, so
  it is a whole-instance operation rather than a selective move of configuration.
- note: the effect of commit order across several update sets is not covered by the retrieved passage, so no
  claim about ordering may be made from it.

## dmi-002 — changing a form's behaviour without writing a script
- objective: 06.1
- source: sources/servicenow-docs-excerpts.md § 06.1 — "UI policies dynamically change the behavior of information on a form … make the number field on a form read-only, make the short description field mandatory, and hide other fields" (Brazil, updated 2026-09-10); objective 06.1 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A field must become read-only and another must become required as a user fills in a form, before they
     save — and the requirement is that it is done without writing any script. Which mechanism does that?
- A: A UI policy. UI policies dynamically change the behaviour of information on a form: making a field
  read-only, making a field mandatory, hiding fields. Basic UI policies need no scripting at all.
- Others: an ACL is enforced on read and write regardless of the form being used, so it is security rather
  than form usability; a business rule runs on the server when a record is queried, updated or inserted, not
  as the user types; a client script would do the job but is scripting, which the requirement excludes.
- to verify: whether the exam distinguishes UI policy from client script by performance — the page says
  client scripts can perform all of these actions "but for faster performance use UI policies".

## dmi-004 — where a rule runs, and when
- objective: 06.2
- source: sources/servicenow-docs-excerpts.md § 06.2 — "Business rules are server-side actions that can be run during CRUD (Create, Read, Update, Delete) operations on instance records." (Brazil, updated 2026-09-10; authored text, not the page's AI summary block); objective 06.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A rule must set a value on a record as part of the save, and be able to stop the save if the value is
     invalid. Where does it run?
- A: Server-side, as a business rule, configured to run **before** the database operation — synchronously,
  setting or updating values on the current object as part of the save and validating or aborting the
  execution if required.
- Others: after the database operation is too late to abort the save; asynchronous runs do not block the
  save at all; the display option runs when a form is shown, which is not part of the save.
- to verify: the answer against the cited passage, in particular the before/after/async/display distinction
  and whether the exam tests the query option.

## dmi-005 — client-side or server-side
- objective: 06.4
- source: sources/servicenow-docs-excerpts.md § 06.4 — "Client scripts allow the system to run JavaScript on the client (web browser) when client-based events occur" and "Server-side scripts run on the server or database." (Brazil, updated 2026-09-10); objective 06.4 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A script must make a field read-only and mandatory on a form **as the user works in it, before saving**.
     Where does that script run?
- A: On the client, in the browser. Client scripts run JavaScript on the client when client-based events
  occur, such as when a form loads, after submission, or when a field changes value — and making fields read
  only, optional, mandatory or hidden is exactly what they are for.
- Others: a server-side script runs on the server or database when records and tables are accessed or
  modified, which is after the user's interaction rather than during it; scope determines which APIs a
  server-side script may reach, not where it runs; a UI policy is the declarative alternative to this script,
  not a location.
- to verify: the answer against the cited pair of pages, and whether the exam expects scope (global versus
  scoped application) as a separate testable fact — the server-side passage states it, so it may be its own
  item.

## dmi-003 — what must happen before an update set can be committed
- objective: 06.3
- source: sources/servicenow-docs-excerpts.md § 06.3 — "You can't commit an update set until all problems are resolved." (Brazil, updated 2026-09-10); objective 06.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: On the target instance you retrieve an update set and try to commit it, but the system will not let you
     proceed. What has to be dealt with first?
- A: The problems that previewing found. An update set cannot be committed until all problems are resolved;
  after that, committing applies the changes and generates a local copy with records of each update.
- Others: activating a plugin is unrelated to committing your own configuration; retrieving happens before
  previewing, so the set is already retrieved; marking a set Complete is an action on the source instance,
  and a set that is no longer wanted is set to Ignore rather than committed.
- to verify: the answer against the cited passage, and whether the exam expects the commit log and the
  unsafe edit warnings that the same page describes.



