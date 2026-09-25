# Source — public ServiceNow documentation

Quoted from `servicenow.com/docs`. These are the cited passages the bank is checked against. Short verbatim quotes only; the pages themselves are linked.

Every passage below is quoted from ServiceNow's public product documentation, with the page and its release. The bank cites these sections, so a question can always be traced back to the page it came from.

## 03.1 Lists, Filters, and Tags — condition builder

| | |
| :--- | :--- |
| Page | Create a filter in List |
| URL | https://www.servicenow.com/docs/r/yokohama/platform-user-interface/t_CreatingFilters.html |
| Release | Yokohama — updated 2025-01-30 |

> You can create a filter to restrict what records appear in a list by providing a set of conditions. When you run the filter, only records that meet the specified conditions are listed.

> Open the condition builder by clicking the show/hide filter icon. … Select a field from the list. The field type determines the available operators and values.

> Optional: Click Save to keep the filter for future use. … Click Run to apply the filter.

Also on the page: `If the icon is disabled and the breadcrumb has a related list condition in it, you must remove the related list condition to open the filter` — the breadcrumb carries conditions of its own, which is the distinction a question can turn on.

What this passage does **not** cover: whether a filter can be shared with other users or published as a module. No claim to that effect may be cited here.

## 03.2 List and Form anatomy — related lists

| | |
| :--- | :--- |
| Page | Related lists |
| URL | https://www.servicenow.com/docs/r/platform-user-interface/c_RelatedLists.html |
| Release | Brazil — updated 2026-09-10 |

> Related lists appear on forms and show records in tables that have relationships to the current record. Users can view and modify information in related lists like any other list. Administrators can configure related lists to appear on forms and in hierarchical lists by configuring a form.

> Note: Creating a record using a related list applies the list filter to the record and auto-populates the related field.

> Create defined related lists — You can add default related lists to the form for all users to see when viewing records.

## 06.3 System update sets — the move between instances

| | |
| :--- | :--- |
| Page | Working with update sets |
| URL | https://www.servicenow.com/docs/r/zurich/application-development/system-update-sets/using-system-update-sets.html |
| Release | Zurich — updated 2025-08-07 |

> These procedures help you manage your customizations and resolve potential collisions before you move them to another instance.

> create an update set and use it to change a development instance. You can report on updates, merge update sets, and compare update sets to ensure that the desired changes are ready to move. When the update set is completed, you can transfer the update set to another instance according to your test process.

> Administrators can preview local and remote (retrieved) update sets and compare the sets with one another to resolve conflicting changes.

Page structure on the same page, in order: *Retrieve an update set* → *Preview a remote update set* → *Commit an update set* → *Back out an update set*. That order is the workflow, and the four steps are the vocabulary.

What this passage does **not** cover: the effect of **commit order** when several update sets are applied in sequence. That claim needs its own passage before it is used.

## Brazil release

Release **Brazil**, every page dated **updated 2026-09-10**, so the version is consistent across the batch.

### 01.1 Platform overview

| | |
| :--- | :--- |
| Page | How the ServiceNow AI Platform works |
| URL | https://www.servicenow.com/docs/r/platform-administration/how-now-platform-works.html |

Passage pending a second read: the page opens with an AI-generated summary block that must not be quoted, and the authored text below it has not been read yet.

### 01.4 Next Experience Unified Navigation

| | |
| :--- | :--- |
| Page | Unified Navigation |
| URL | https://www.servicenow.com/docs/r/platform-user-interface/using-the-next-experience-global-header.html |

> The Next Experience Unified Navigation provides controls for navigating your instance, accessing records and data, checking notifications, and setting your preferences.

> The Next Experience Unified Navigation appears at the top of every page and includes controls for navigating your instance. Access your workspaces and classic environment, search your instance, and receive notifications.

### 02.1 Installing applications and plugins

| | |
| :--- | :--- |
| Page | Activate a plugin |
| URL | https://www.servicenow.com/docs/r/platform-administration/t_ActivateAPlugin.html |

> You can activate most plugins to expand features and functionalities in the ServiceNow AI Platform.

> Navigate to All > System Applications > All Available Applications > All. Find the plugin using the filter criteria and search bar. … Select Install to start the installation process.

Not supported here: any contrast between a *plugin* and an *application*. That distinction is not made on this page, so no question may key it from here.

### 02.2 Personalising and customising the instance

| | |
| :--- | :--- |
| Page | Add a system property |
| URL | https://www.servicenow.com/docs/r/platform-administration/t_AddAPropertyUsingSysPropsList.html |

> Some properties in the system aren't visible in an instance by default and must be added to the System Property [sys_properties] table.

> System properties store configuration information that rarely or never changes. Each time you change or add a system property, the system flushes the cache to keep all nodes in the cluster in sync. This cache flush has a very high performance cost for one to 10 minutes… don't use a system property to store configuration information that changes more than once or twice a month. Instead, use a custom table.

> Private — Set this property to true to exclude this property from being imported via update sets. Keeping system properties private prevents settings in one instance from overwriting values in another instance.

### 02.3 Common user interfaces

| | |
| :--- | :--- |
| Page | Primary interfaces |
| URL | https://www.servicenow.com/docs/r/application-development/primary-interfaces.html |

> In ServiceNow, the primary methods for users to interact with data models are through forms, lists, or mobile devices.

> A form displays information from one record in a data table and a list displays a set of records from a table.

> If users will interact with the application on their mobile devices and will need native iOS or Android functionality, such as geolocation or offline access to application data, use the ServiceNow Agent app.

### 03.1 Filters — and the AND/OR clause this file previously lacked

| | |
| :--- | :--- |
| Page | Create a filter in List |
| URL | https://www.servicenow.com/docs/r/platform-user-interface/t_CreatingFilters.html |

> You can create a filter to restrict what records appear in a list by providing a set of conditions. When you run the filter, only records that meet the specified conditions are listed.

> The field type determines the available operators and values.

> **To add a top-level condition** — Click AND or OR on the condition builder toolbar, above the conditions. **To add a dependent condition** — Click AND or OR beside the condition.

> Optional: Click Save to keep the filter for future use. … Click Run to apply the filter.

This Brazil page documents AND/OR grouping, which the Yokohama page quoted earlier does not.

### 03.1 Tags

| | |
| :--- | :--- |
| Page | Tags |
| URL | https://www.servicenow.com/docs/r/platform-user-interface/c_Tags.html |

> Tags are text labels that you can associate with items like records and pages. Tags enable you to group and organize the items. Tags can be visible to any user (global), visible only to specific groups or users (shared), or visible to a single user (private).

> Tags are stored in the Tag [label] table.

### 03.3 Form configuration

| | |
| :--- | :--- |
| Page | Form designer |
| URL | https://www.servicenow.com/docs/r/platform-administration/c_FormDesign.html |

> Administrators or users with the personalize_form role can use the form design feature to quickly create new or change existing form views.

> Starting with the Australia release, form designer is being prepared for future deprecation. Try configuring your forms with Form Builder instead. Form Builder has all of the Form Designer and Form Layout options.

### 03.6 Task management

| | |
| :--- | :--- |
| Page | Task table structure |
| URL | https://www.servicenow.com/docs/r/platform-administration/table-administration-and-data-management/task-table-structure.html |

> The Task table structure provides a framework to organize and store task-related data, and includes extensive customization options.

> The Task table is a base class that provides fields for the core ITSM applications such as Incident, Problem, and Change Management. All applications that extend the Task table share these fields in common.

### 03.7 Visual Task Boards

| | |
| :--- | :--- |
| Page | Visual Task Boards |
| URL | https://www.servicenow.com/docs/r/platform-user-interface/visual-task-boards/c_VisualTaskBoards.html |

> Visual Task Boards (VTB) transform the navigation of lists and forms into an interactive graphical experience.

> Note: Core UI or Next Experience is required to use Visual Task Boards.

### 04.1 Knowledge Management

| | |
| :--- | :--- |
| Page | Knowledge management |
| URL | https://www.servicenow.com/docs/r/platform-administration/ia-knowledge-mgmt.html |

> Set up a knowledge base: Configure the knowledge base to define where articles are stored, how content is structured, and who can access it.

> Article templates: Predefined forms provide a consistent content structure by enabling authors to create articles using standard fields such as Problem and Solution.

> Review the flows: Define and configure workflows for article creation, review, approval, and publication, including approval stages and reviewer assignments.

### 04.2 Service Catalog variables

| | |
| :--- | :--- |
| Page | Service catalog variables |
| URL | https://www.servicenow.com/docs/r/servicenow-platform/service-catalog/c_ServiceCatalogVariables.html |

> Service catalog variables capture and pass on information about choices a customer makes when ordering a catalog item. Variables help define the structure of a catalog item form that is displayed to the customer.

> Service Catalog provides several types of variables, which are also referred to as questions. Variables can be stored, accessed from multiple places, and passed between tasks in a process when fulfilling a request. They can be displayed on the Requested Item and Catalog Task forms after an item has been ordered.

### 04.4 Virtual Agent

| | |
| :--- | :--- |
| Page | Virtual Agent |
| URL | https://www.servicenow.com/docs/r/application-development/virtual-agent.html |

> Consider Virtual Agent, ServiceNow's conversational bot platform. Use ServiceNow Virtual Agent (VA) to build and design bot conversations to help users quickly obtain information, make decisions, and perform common work tasks.

### 05.1 Data Schema

| | |
| :--- | :--- |
| Page | System dictionary |
| URL | https://www.servicenow.com/docs/r/platform-administration/table-administration-and-data-management/c_SystemDictionary.html |

> Each row in the system dictionary represents either a table or a column in one of the tables. The system dictionary provides options for administrators to modify tables and fields, which in turn define lists and forms.

> Use caution when changing system dictionary records because changes can have a high impact on functionality. In particular, changes to dictionary entries for system tables, which are tables that begin with sys_, can create system-wide issues such as the inability to use update sets.

> dictionary changes automatically apply to all extended tables unless a dictionary override is defined.

> In most cases, use the following interfaces rather than creating entries directly on the system dictionary: To create tables and fields, use the Tables module. To create fields, configure the table form.

### 05.4 CMDB and CSDM

| | |
| :--- | :--- |
| Page | Configuration Management Database (CMDB) |
| URL | https://www.servicenow.com/docs/r/servicenow-platform/configuration-management-database-cmdb/c_ITILConfigurationManagement.html |

> Use the ServiceNow® Configuration Management Database (CMDB) application to build logical representations of assets, services, and the relationships between them that comprise the infrastructure of your organization. Details about these components are stored in the CMDB as configuration items (CIs), which you can use to monitor the infrastructure.

> Unified Map — View a hierarchical map of CIs and the relationships between them.

Not supported here: that a CI relationship is **its own record** in its own table. This page describes CIs as records and relationships as something mapped and viewed, and no more. A question keying the storage of relationships needs a different passage.

### 06.1 UI Policies

| | |
| :--- | :--- |
| Page | UI policies |
| URL | https://www.servicenow.com/docs/r/platform-administration/t_CreateAUIPolicy.html |

> UI policies dynamically change the behavior of information on a form and control custom process flows for tasks. For example, you can use UI policies to make the number field on a form read-only, make the short description field mandatory, and hide other fields. Basic UI policies do not require any scripting, however for more advanced actions, use the Run scripts option.

> You can also use client scripts to perform all of these actions, but for faster performance use UI policies.

### 06.3 Commit an update set

| | |
| :--- | :--- |
| Page | Commit an update set |
| URL | https://www.servicenow.com/docs/r/application-development/system-update-sets/t_CommitAnUpdateSet.html |

> After resolving any issues from previewing, commit the update set to apply all changes and generate a local copy with records of each update.

> You can't commit an update set until all problems are resolved.

> Change the state to Ignore when you're no longer working on the update set, but don't want it transferred to another instance.

Still not covered anywhere: the effect of **commit order** when several update sets are applied in sequence.

### 01.1 Platform overview — the authored text, not the AI summary

| | |
| :--- | :--- |
| Page | How the ServiceNow AI Platform works |
| URL | https://www.servicenow.com/docs/r/platform-administration/how-now-platform-works.html |

Note: this page opens with an AI-generated summary block headed "Summarized using AI … not guaranteed to be accurate or complete". The passages below are the page's own authored text, not that summary.

> The ServiceNow AI Platform is the unified foundation for every ServiceNow product. It brings together AI, data, workflows, and security to execute work across areas such as IT, CRM, employee experience, risk and security, and application development.

> Services on the ServiceNow AI Platform are provided on a **multi-instance** basis, instead of running one instance with multiple users. Administrators can segregate their data between business entities in a multi-instance architecture, offering different experiences per instance while they all remain centrally managed through the platform.

Note the vendor's word is **multi-instance**, not "multi-tenant" — a question should key the document's term.

### 01.2 Platform capabilities and services

| | |
| :--- | :--- |
| Pages | the same overview page (different sections), plus the capabilities landing page |
| URLs | https://www.servicenow.com/docs/r/platform-administration/how-now-platform-works.html · https://www.servicenow.com/docs/r/servicenow-platform/capabilities-bundle-landingpage.html |

> Extend the platform through the **ServiceNow Store**, where partner-built applications and integrations are available for deployment. A robust partner ecosystem means solutions exist for many industries, use cases, and technology environments.

> **Administration** — The ServiceNow AI Platform Admin Center gives business administrators at-a-glance information and access to configuration management and AI-powered implementation.

> The ServiceNow AI Platform delivers regular releases on a predictable cadence, with automated testing tools and upgrade options that keep your operations running through every update.

> The capabilities landing page — "Extend the ServiceNow AI Platform with additional applications and features."

### 01.3 The ServiceNow Instance

| | |
| :--- | :--- |
| Page | Instance Clone |
| URL | https://www.servicenow.com/docs/r/platform-administration/system-clone-landing.html |

> Clone copies data and metadata from one ServiceNow instance (**source instance**) to another ServiceNow instance (**target instance**).

> Request a clone to copy data from a **production** instance to a **non-production** instance.

The blueprint's sub-topic is "The ServiceNow Instance" and this is the page where the documentation treats instances as objects an administrator manages. A question should key the clone direction and vocabulary, which is what this page states, rather than the sub-topic's broad wording.

### 04.3 Workflow Studio — and the name it changed from

| | |
| :--- | :--- |
| Page | Flow Designer |
| URL | https://www.servicenow.com/docs/r/application-development/flow-designer.html |

> When to Use Flow Designer vs. Business Rules — Use Flow Designer for most automation needs **unless** business logic must run in a precise sequence with other Business Rules, execute immediately before or after database writes in the same thread, or only call a Script Include.

**A naming caveat worth carrying:** the blueprint of January 2026 calls this sub-topic **Workflow Studio**, while the documentation page is still titled **Flow Designer**. Other pages in the same bundle already say "from Workflow Studio", so the rename is in flight. A question must use the blueprint's word and must not offer the other as a distractor — that would be a trivia trap, not a test of the material.

### 05.2 Application/Access Control

| | |
| :--- | :--- |
| Page | Access Control Lists (ACLs) |
| URL | https://www.servicenow.com/docs/r/platform-security/access-control/access-control-rules.html |

> Access control lists (ACLs) restrict access to data by requiring users to pass a set of requirements before they can interact with it.

The page's own structure continues into *Explore ACLs*, *Configure ACLs*, *Contextual Security Manager* and *Advanced ACL Configuration*.

### 05.3 Importing Data

| | |
| :--- | :--- |
| Page | Import Sets API |
| URL | https://www.servicenow.com/docs/r/application-development/servicenow-sdk/fluent-import-sets-api.html |

> The Import Sets API defines **transform maps** `[sys_transform_map]` that specify how to transform and map data from the import set **staging table** to **target tables**.

> Every import operation to a production table requires at least one transform map associated with an import set.

Caveat: this is the SDK page for import sets, not the administrator's guide to them. It states the staging → transform map → target model clearly, which is the examinable shape, and nothing beyond that model may be keyed from it.

### 05.5 Security Center

| | |
| :--- | :--- |
| Page | Security Center |
| URL | https://www.servicenow.com/docs/r/platform-security/security-center/sec-center-v2.html |

> ServiceNow Security Center is an application that consists of a set of tools designed to help your organization maintain the security of your ServiceNow deployments. Using Security Center, you can improve security posture and strengthen compliance levels with a seamless user experience.

> Security Center is a free application that administrators can download from the ServiceNow Store. It's installed by default starting with the **Vancouver** release.

### 05.6 Shared Responsibility Model

| | |
| :--- | :--- |
| Document | Shared Responsibility Model — a ServiceNow data sheet, `Shared Responsibility Model-mini_v4.2` |
| Dated | 4 August 2026, release **Australia** |
| URL | https://www.servicenow.com/content/dam/servicenow-assets/public/en-us/doc-type/resource-center/white-paper/wp-shared-responsibility-model.pdf |
| Note | published as a PDF; the passages below are its text |

> Security is a partnership between ServiceNow and the customer, both with specific responsibilities. Therefore, it is essential that each party understands their role in this partnership.

> As the **data controller**, the customer determines access rights to their instance and the data it contains. Security controls within the instance enable customers to implement policies appropriate to their own requirements and make decisions on data classification.

> As the **data processor**, ServiceNow secures the platform infrastructure and provides tools for security management and monitoring according to customer requirements.

> The **colocation facility** and the third-party **cloud service provider (CSP)** also have shared responsibilities with the data controller (customer) and data processor (ServiceNow).

Its responsibility table assigns **Instance management**, **Secure instance configuration** and **Identity and access management** to the customer; **Cloud infrastructure security management** is shared; **Physical security and environment controls** sit with the colocation and hyperscaler sites. That table is the ground for any question about who owns what.

### 06.2 Business rules

| | |
| :--- | :--- |
| Page | Business rules and script includes |
| URL | https://www.servicenow.com/docs/r/application-development/business-rules-and-script-includes.html |

This page also opens with an AI summary block; the quotes are from the authored text below it.

> Business rules are **server-side** actions that can be run during CRUD (Create, Read, Update, Delete) operations on instance records.

> Business Rules can be configured to run before or after a database operation. They can also be configured to run asynchronously and also before displaying a form or executing a query.

> **Before** — Synchronously before the database operation. Set or update values on the current object as part of the save operation. Validate and abort execution if required.

### 06.4 Scripting in ServiceNow

| | |
| :--- | :--- |
| Pages | Client scripts · Server-side scripting |
| URLs | https://www.servicenow.com/docs/r/api-reference/scripts/client-scripts.html · https://www.servicenow.com/docs/r/api-reference/scripts/c_ServerScripting.html |

> Client scripts allow the system to run JavaScript on the **client** (web browser) when client-based events occur, such as when a form loads, after form submission, or when a field changes value.

> Client scripts can: make fields hidden or visible · make fields read only or writable · make fields optional or mandatory based on the user's role · set the value in one field based on the value in other fields · modify the options in a choice list based on a user's role.

> Server-side scripts run on the **server or database**. They can change the appearance or behavior of ServiceNow or run as business rules when records and tables are accessed or modified.

> Server-side scripts run in either the **global scope** or a **scoped application scope**, which determines which APIs are accessible.

Client versus server is the discrimination this pair supports, and it is one the exam is known to lean on.

## Coverage of the thirty objectives

| Objective | Cited passage |
| :--- | :--- |
| 01.1 | overview page, authored text — the multi-instance passage |
| 01.2 | overview page + capabilities landing page |
| 01.3 | Instance Clone |
| 01.4 | Unified Navigation |
| 02.1 | Activate a plugin |
| 02.2 | Add a system property |
| 02.3 | Primary interfaces |
| 03.1 | Create a filter in List |
| 03.2 | Related lists |
| 03.3 | Form designer |
| **03.4 Form templates and saving options** | **nothing yet** |
| **03.5 Advanced Form Configuration** | **nothing yet** |
| 03.6 | Task table structure |
| 03.7 | Visual Task Boards |
| **03.8 Visualizations, Dashboards, and Platform Analytics** | **nothing yet** |
| **03.9 Notifications** | **nothing yet** |
| 04.1 | Knowledge management |
| 04.2 | Service catalog variables |
| 04.3 | Flow Designer — the blueprint calls it Workflow Studio |
| 04.4 | Virtual Agent |
| 05.1 | System dictionary |
| 05.2 | Access Control Lists (ACLs) |
| 05.3 | Import Sets API |
| 05.4 | Configuration Management Database (CMDB) |
| 05.5 | Security Center |
| 05.6 | Shared Responsibility Model data sheet |
| 06.1 | UI policies |
| 06.2 | Business rules and script includes |
| 06.3 | Working with update sets · Commit an update set |
| 06.4 | Client scripts · Server-side scripting |

**Twenty-six of thirty objectives now have a cited passage.** The four gaps — 03.4, 03.5, 03.8, 03.9 — all sit in domain 03, which is 20% of the exam. Also still uncovered: the effect of **commit order** when several update sets are applied in sequence.

Two different kinds of limit, worth not confusing with each other:

- the **participant guide** is unobtainable, full stop — the eBook platform does not permit export, so no amount of searching changes that. Its content only enters this repo if the learner types or pastes it
- several doc pages **open with an AI-generated summary block** that must never be quoted. The authored text below it is what every passage above cites, and two of those pages say so explicitly

The four gaps are named above rather than left implicit, and they are the work queue.

