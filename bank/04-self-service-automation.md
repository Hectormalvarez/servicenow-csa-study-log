# 04 Self Service & Automation

Objectives 04.1–04.4 (`GOAL.md` § Objectives). Weight 20%. **All four entries are `verified: yes`.**

## ssa-001 — the item a user orders, and what carries its questions
- objective: 04.2
- source: sources/servicenow-docs-excerpts.md § 04.2 — "Service catalog variables capture and pass on information about choices a customer makes when ordering a catalog item." and variables "are also referred to as questions" (Brazil, updated 2026-09-10); objective 04.2 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A user opens the catalog and requests a laptop. The request form asks about the model and the delivery
     location, and the answers do not exist as fields on any table until the request is submitted. What are
     those questions called?
- A: Variables. They belong to the catalog item and hold the user's answers; the item is what the user sees
  and orders, and the variables are what make that one item ask different things or produce different
  fulfilment.
- Others: a record producer creates a task record from a form rather than placing something in a cart; an
  order guide bundles several catalog items into one guided order; a category is only a grouping in the
  catalog's navigation.
- to verify: the answer against a cited passage on the Service Catalog, and whether the blueprint treats
  variables and catalog item options as one topic or two.

## ssa-002 — the article structure users actually read
- objective: 04.1
- source: sources/servicenow-docs-excerpts.md § 04.1 — "Configure the knowledge base to define where articles are stored, how content is structured, and who can access it." and "Article templates: Predefined forms provide a consistent content structure" (Brazil, updated 2026-09-10); objective 04.1 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A knowledge base needs a set of articles that all share the same format and follow one approval
     process. What do you create?
- A: A knowledge base with a template — the template fixes the structure of each article, and the knowledge
  base carries the workflow and the permissions for its articles.
- Others: a category inside a knowledge base groups articles but does not define their structure; a catalog
  item is for ordering something, not for reading; a UI policy acts on a form, not on an article.
- to verify: the answer against a cited passage on Knowledge Management, and whether templates are exam
  scope at the level of the blueprint statement.

## ssa-003 — the platform's conversational bot
- objective: 04.4
- source: sources/servicenow-docs-excerpts.md § 04.4 — "Consider Virtual Agent, ServiceNow's conversational bot platform." (Brazil, updated 2026-09-10); objective 04.4 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: A user asks a question in plain language in a chat window, and the bot answers and performs the task
     behind it. Which platform capability is that?
- A: Virtual Agent — ServiceNow's conversational bot platform, used to build and design bot conversations so
  that users can obtain information, make decisions and perform common work tasks.
- Others: a knowledge article answers the same question but is a document to read, not a conversation;
  notifications push a message out rather than holding one; the Service Catalog is an ordering interface,
  and a Virtual Agent conversation may reach it — but the conversation itself is Virtual Agent.
- to verify: whether the exam expects conversation topics as the unit of authoring, which the guidance on
  the same page implies without naming it as a testable item.

## ssa-004 — automation where the logic has to run in a precise order
- objective: 04.3
- source: sources/servicenow-docs-excerpts.md § 04.3 — "Use Flow Designer for most automation needs unless business logic must run in a precise sequence with other Business Rules, execute immediately before or after database writes in the same thread, or only call a Script Include." (Brazil, updated 2026-09-10; the blueprint names this sub-topic **Workflow Studio**); objective 04.3 in `GOAL.md`
- verified: yes — separate context, 2026-09-25
- seen: never · misses: 0 · interval: —
- Q: You are choosing where to build an automation. It has to run in a precise sequence with existing Business
     Rules and immediately before a database write, in the same thread. What does the documentation say to
     use?
- A: Business Rules, not the automation designer. The guidance is to use Flow Designer — the blueprint's
  Workflow Studio — for most automation, **except** when logic must run in a precise sequence with other
  Business Rules, execute immediately before or after database writes in the same thread, or only call a
  Script Include.
- Others: the exception is not about volume or complexity of the flow, so "build it in the designer anyway"
  is wrong; a Scheduled Job runs on a schedule rather than inside the write; a UI policy is client-side form
  behaviour and never touches the database write.
- note on naming: the documentation page is titled **Flow Designer**, while the January 2026 blueprint calls
  the sub-topic **Workflow Studio**. The blueprint's word is the one to use, and the other must not be offered
  as a distractor — that would test trivia about a rename rather than the material.
