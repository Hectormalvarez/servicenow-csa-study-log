# 05 Database Management and Platform Security

Objectives 05.1–05.6 (`GOAL.md` § Objectives). Weight 30% — the largest domain, and the one that gets the most session time by construction. **All six entries are `verified: yes`.**

## db-001 — where a field's definition lives
- objective: 05.1
- source: sources/servicenow-docs-excerpts.md § 05.1 — "Each row in the system dictionary represents either a table or a column in one of the tables." (Brazil, updated 2026-09-10); objective 05.1 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A new field is needed on the incident table, with a specific type, a default value, and a target it
     points at. Which record holds that definition?
- A: The dictionary entry for the field — the table's Dictionary, reached from the form's context menu or
  from the table's own Dictionary module. The table defines the structure; the dictionary defines each
  field on it.
- Others: a form layout decides where the field appears and in what order; a UI policy changes its behaviour
  on the form at run time; an ACL decides who may read or write it. None of those defines what the field is.
- to verify: the answer against a cited passage covering the data schema, and whether the exam expects the
  table name for the dictionary by name.

## db-002 — what the server is, and how the CMDB shows its connections
- objective: 05.4
- source: sources/servicenow-docs-excerpts.md § 05.4 — "Details about these components are stored in the CMDB as configuration items (CIs)" (Brazil, updated 2026-09-10); objective 05.4 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A server in the CMDB is one record. The connections to the services it supports, and to the things that
     depend on it, appear as links between records. What are those two things called?
- A: The server is a **configuration item (CI)**. The CMDB holds logical representations of the assets and
  services that make up the infrastructure, and the details of those components are stored as CIs. The
  connections are the **relationships between CIs** — what the CMDB maps, and what **Unified Map** presents
  as a hierarchical map of CIs and the relationships between them.
- Others: a catalog item is something a user orders, not a record of infrastructure; a knowledge article may
  describe the server without being the CMDB's record of it; a task raised about the server is a piece of work
  rather than the record the configuration lives in.
- to verify: whether the exam expects the relationship's own table by name. The cited page does **not** say
  that relationships are stored as their own records, so nothing may be keyed about that from it. The three
  distractors are grounded elsewhere in the sources file (§ 04.2, § 04.1, § 03.6), not in § 05.4 itself.

## db-003 — what stops a user changing a record they can open
- objective: 05.2
- source: sources/servicenow-docs-excerpts.md § 05.2 — "Access control lists (ACLs) restrict access to data by requiring users to pass a set of requirements before they can interact with it." (Brazil, updated 2026-09-10); objective 05.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A user can open a record but cannot save a change to it. Which mechanism decides that?
- A: The access control lists that apply to that data. An ACL restricts access to data by requiring users to
  pass a set of requirements before they can interact with it, and this user is failing one of them.
- Others: a UI policy changes what a form lets a user do, but it is not the security check and does not apply
  through every interface; a business rule runs logic on the server rather than granting or refusing access;
  an instance hardening setting reduces risk across the instance rather than deciding one user's access to one
  record.
- to verify: whether the exam tests read and write as separate ACL requirements. The quoted sentence states
  only the general mechanism, so that distinction needs its own passage before a question can key it.

## db-004 — the path data takes before it reaches a table
- objective: 05.3
- source: sources/servicenow-docs-excerpts.md § 05.3 — "The Import Sets API defines transform maps `[sys_transform_map]` that specify how to transform and map data from the import set staging table to target tables." (Brazil, updated 2026-09-10); objective 05.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: Records arrive from a spreadsheet and must be validated and reshaped before they land in the incident
     table. What does that work, and where do the records sit first?
- A: A transform map. The records land in an import set **staging table** first, and the transform map
  specifies how to transform and map them from there to the **target table**.
- Others: an update set moves configuration between instances and never loads records; a business rule runs
  when records are written, so it is not what maps the incoming columns; a dictionary entry defines a field
  rather than mapping an incoming one.
- to verify: the answer against the cited passage, and whether a question should require the transform map
  table name `sys_transform_map`. The cited page is the developer SDK page, so its wording is developer-facing.

## db-005 — the application for security posture
- objective: 05.5
- source: sources/servicenow-docs-excerpts.md § 05.5 — "ServiceNow Security Center is an application that consists of a set of tools designed to help your organization maintain the security of your ServiceNow deployments." (Brazil, updated 2026-09-10); objective 05.5 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You want to see how your instance's security posture measures up and to track compliance. Which
     application does that, and where does it come from?
- A: Security Center. It consists of a set of tools for maintaining the security of your ServiceNow
  deployments; it is a free application administrators can download from the ServiceNow Store, and it has
  been installed by default since the Vancouver release.
- Others: ACLs govern access to individual data and are part of the instance's own configuration rather than
  an application; instance hardening settings are settings an administrator applies, not the application that
  reports on them; the Shared Responsibility Model describes how responsibilities are divided with
  ServiceNow, and is not a tool.
- to verify: whether the exam expects the ServiceNow Store as the source, or merely that it ships with the
  platform from Vancouver onward. Both are stated, so a question should not force one.

## db-006 — who secures what
- objective: 05.6
- source: sources/servicenow-docs-excerpts.md § 05.6 — "As the data controller, the customer determines access rights to their instance and the data it contains." and "As the data processor, ServiceNow secures the platform infrastructure and provides tools for security management and monitoring" (Shared Responsibility Model data sheet, 4 August 2026, release Australia); objective 05.6 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: Security on the platform is described as a partnership with specific responsibilities on each side. Which
     of these is the customer's?
- A: Deciding who may reach the instance and what its data is. The customer is the **data controller**: it
  determines access rights to its instance and the data it contains, and applies the security controls within
  the instance to meet its own policies and data classification decisions.
- Others: securing the platform infrastructure and providing the tools for security management and
  monitoring is ServiceNow's side as the **data processor**; physical security and environment controls sit
  with the colocation and hyperscaler sites, which carry their own shared responsibilities; the customer does
  not patch the platform's own code or administer its release cycle.
- to verify: the answer against the data sheet's responsibility table, which assigns instance management,
  secure instance configuration and identity and access management to the customer. Whether the exam tests
  individual rows of that table is not known.
