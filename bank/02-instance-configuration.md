# 02 Instance Configuration

Objectives 02.1–02.3 (`GOAL.md` § Objectives). Weight 10%. **All three entries are `verified: yes`.**

## ic-001 — a setting that must apply to everyone
- objective: 02.2
- source: sources/servicenow-docs-excerpts.md § 02.2 — "must be added to the System Property [sys_properties] table" and "System properties store configuration information that rarely or never changes." (Brazil, updated 2026-09-10); objective 02.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: An administrator needs a behaviour to apply to every user in the instance, not only to their own
     session or their own view. Which mechanism is that?
- A: A system property (`sys_properties`, reached through System Properties). It is instance-wide and
  admin-controlled.
- Others: a user preference applies only to that user's own interface; personalising a list or form changes
  that user's layout of it; a UI policy acts on a form at run time rather than being a stored system
  setting.
- to verify: the answer against a cited passage covering instance customisation, and whether the exam wants
  the table name or the module path.

## ic-002 — where a platform plugin gets installed
- objective: 02.1
- source: sources/servicenow-docs-excerpts.md § 02.1 — "You can activate most plugins to expand features and functionalities in the ServiceNow AI Platform." and "Navigate to All > System Applications > All Available Applications > All … Select Install" (Brazil, updated 2026-09-10); objective 02.1 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You need to add a capability that ServiceNow ships with the platform to your instance. Where do you find it
     and install it?
- A: In the plugin list — All > System Applications > All Available Applications > All. Most plugins can be
  activated to expand features and functionality, and installation starts with Install.
- Others: an update set moves your own configuration between instances rather than adding vendor capability;
  a system property changes a setting, it does not install anything; a dictionary entry defines a field, it
  adds no feature.
- to verify: the plugin-versus-application distinction is **not** drawn by the cited page. A passage that
  draws it is needed before any item may key that discrimination.

## ic-003 — recognising the interfaces a user works in
- objective: 02.3
- source: sources/servicenow-docs-excerpts.md § 02.3 — "In ServiceNow, the primary methods for users to interact with data models are through forms, lists, or mobile devices." and "A form displays information from one record in a data table and a list displays a set of records from a table." (Brazil, updated 2026-09-10); objective 02.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A user needs to see every open incident assigned to their group, and then open one of them to edit it.
     Which two of the platform's primary interfaces are they moving between?
- A: A list and a form. A list shows a set of records from a table; a form shows the information from one
  record. Together with mobile, those are the primary ways users interact with the platform's data.
- Others: a Visual Task Board is a graphical way of working those same records, not a primary interface; a
  report presents data without letting you edit a record; a dashboard shows indicators rather than a table's
  records.
- to verify: whether the exam counts Visual Task Boards and dashboards as "interfaces in the Platform" for
  this sub-topic. The cited page names only forms, lists and mobile, so a question should stay inside those.
