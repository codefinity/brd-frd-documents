**BUSINESS REQUIREMENTS**

**SPECIFICATION**

\[Project / initiative name\]

\[Organization name\] · \[Business unit\]

|                      |                                               |
|----------------------|-----------------------------------------------|
| **Document ID**      | \[BRS-PRJ-001\]                               |
| **Version**          | \[0.1\]                                       |
| **Status**           | \[Draft / In review / Approved / Superseded\] |
| **Date**             | \[DD-MMM-YYYY\]                               |
| **Document owner**   | \[Name, role\]                                |
| **Business sponsor** | \[Name, role\]                                |
| **Classification**   | \[Public / Internal / Confidential\]          |

*Structured according to the Business Requirements Specification (BRS) content items in ISO/IEC/IEEE 29148:2018, clause 9.3. The guidance text in this template is original and does not reproduce the standard; refer to the standard itself for its normative wording.*

# How to use this template

A Business Requirements Specification (BRS) records why the organization is undertaking a change and what business outcomes it needs. It is written from the business point of view and stays independent of any particular solution. Stakeholder requirements (StRS) and system or software requirements (SyRS / SRS) are derived from it later.

### Conventions

- Shaded boxes marked "Guidance" explain what to write in each section. Delete them before the document is issued.

- Text in \[blue square brackets\] is a placeholder. Replace it with your own content.

- Table rows in grey italics are worked examples. Replace or delete them.

- Keep every section number, even if a section does not apply. Write "Not applicable" and give a one-line reason, so reviewers can see the topic was considered and the mapping to the standard stays intact.

- Use "shall" for binding requirements, "should" for preferences or goals, "will" for statements of fact or intent, and "may" for permitted options. Avoid unmeasurable words such as "fast", "easy", "user-friendly", "flexible" or "etc."

- Give every goal, rule, constraint and requirement a unique ID (for example G-01, RULE-01, C-01, BR-01) so it can be traced into downstream documents.

- To refresh the table of contents in Word, right-click it and choose Update Field → Update entire table.

### Mapping to ISO/IEC/IEEE 29148:2018

Clause numbers refer to the 2018 (second) edition. A third edition is in development and may renumber clauses; check the edition your organization has adopted.

| **Template section** | **Content** | **29148:2018 clause** |
|----|----|----|
| Document control | Identification, version history, approvals | 9.2.1, 9.2.2 |
| 1.1 – 1.3 | Purpose, audience, related documents | 9.3.1 |
| 1.4 | Definitions | 9.2.3 |
| 1.5 | References | 9.2.4 |
| 1.6 | Acronyms and abbreviations | 9.2.5 |
| 2 | Business purpose | 9.3.2 |
| 3 | Business scope | 9.3.3 |
| 4 | Business overview | 9.3.4 |
| 5 | Major stakeholders | 9.3.5 |
| 6 | Business environment | 9.3.6 |
| 7 | Mission, goals and objectives | 9.3.7 |
| 8 | Business model | 9.3.8 |
| 9 | Information environment | 9.3.9 |
| 10 | Business processes | 9.3.10 |
| 11 | Business operational policies and rules | 9.3.11 |
| 12 | Business operational constraints | 9.3.12 |
| 13 | Business operational modes | 9.3.13 |
| 14 | Business operational quality | 9.3.14 |
| 15 | Business structure | 9.3.15 |
| 16 | High-level operational concept | 9.3.16 |
| 17 | High-level operational scenarios | 9.3.17 |
| Appendices A – D | Requirements register, quality checklist, traceability matrix, issues log | Practical additions; not part of the 9.3 outline |

# Document control

### Revision history

| **Version** | **Date**          | **Author** | **Summary of changes**             |
|-------------|-------------------|------------|------------------------------------|
| *0.1*       | *\[DD-MMM-YYYY\]* | *\[Name\]* | *Initial draft for sponsor review* |
|             |                   |            |                                    |
|             |                   |            |                                    |
|             |                   |            |                                    |

### Review and approval

By approving, reviewers confirm that this BRS correctly states the business need and may be used as the basis for deriving stakeholder requirements.

| **Name** | **Role** | **Decision** | **Signature** | **Date** |
|----|----|----|----|----|
| \[Name\] | Business sponsor | \[Approved / Approved with comments / Rejected\] |  |  |
| \[Name\] | Business owner(s) of affected processes |  |  |  |
| \[Name\] | Lead business analyst / requirements engineer |  |  |  |
| \[Name\] | Enterprise / solution architect |  |  |  |
| \[Name\] | Compliance, legal or risk (if applicable) |  |  |  |

### Distribution

| **Name / group**       | **Role**       | **Purpose**                         |
|------------------------|----------------|-------------------------------------|
| \[Steering committee\] | \[Governance\] | \[Approval / Review / Information\] |
|                        |                |                                     |
|                        |                |                                     |

# Contents

If the list below is empty, right-click it and choose Update Field → Update entire table (Word), or Tools → Update → Update All (LibreOffice).

- [How to use this template](#how-to-use-this-template)
- [Document control](#document-control)
- [Contents](#contents)
- [1 Introduction](#1-introduction)
  - [1.1 Purpose of this document](#11-purpose-of-this-document)
  - [1.2 Intended audience](#12-intended-audience)
  - [1.3 Related documents](#13-related-documents)
  - [1.4 Definitions](#14-definitions)
  - [1.5 References](#15-references)
  - [1.6 Acronyms and abbreviations](#16-acronyms-and-abbreviations)
- [2 Business purpose](#2-business-purpose)
  - [2.1 Problem or opportunity statement](#21-problem-or-opportunity-statement)
  - [2.2 Business drivers](#22-business-drivers)
  - [2.3 Cost of inaction](#23-cost-of-inaction)
- [3 Business scope](#3-business-scope)
  - [3.1 In scope](#31-in-scope)
  - [3.2 Out of scope](#32-out-of-scope)
  - [3.3 Assumptions](#33-assumptions)
  - [3.4 Dependencies](#34-dependencies)
- [4 Business overview](#4-business-overview)
  - [4.1 Current state](#41-current-state)
  - [4.2 Key facts and figures](#42-key-facts-and-figures)
  - [4.3 Business context diagram](#43-business-context-diagram)
- [5 Major stakeholders](#5-major-stakeholders)
- [6 Business environment](#6-business-environment)
- [7 Mission, goals and objectives](#7-mission-goals-and-objectives)
  - [7.1 Mission and strategic alignment](#71-mission-and-strategic-alignment)
  - [7.2 Goals and objectives](#72-goals-and-objectives)
  - [7.3 Success criteria and benefits](#73-success-criteria-and-benefits)
- [8 Business model](#8-business-model)
- [9 Information environment](#9-information-environment)
  - [9.1 Information items](#91-information-items)
  - [9.2 Existing systems and data stores](#92-existing-systems-and-data-stores)
- [10 Business processes](#10-business-processes)
  - [10.1 Process inventory](#101-process-inventory)
  - [10.2 Process descriptions](#102-process-descriptions)
- [11 Business operational policies and rules](#11-business-operational-policies-and-rules)
- [12 Business operational constraints](#12-business-operational-constraints)
- [13 Business operational modes](#13-business-operational-modes)
- [14 Business operational quality](#14-business-operational-quality)
- [15 Business structure](#15-business-structure)
  - [15.1 Organizational units and roles](#151-organizational-units-and-roles)
  - [15.2 Organization chart](#152-organization-chart)
- [16 High-level operational concept](#16-high-level-operational-concept)
- [17 High-level operational scenarios](#17-high-level-operational-scenarios)
  - [17.1 Scenario summary](#171-scenario-summary)
  - [17.2 Scenario descriptions](#172-scenario-descriptions)
- [Appendix A — Business requirements register](#appendix-a--business-requirements-register)
- [Appendix B — Requirement quality checklist](#appendix-b--requirement-quality-checklist)
- [Appendix C — Traceability matrix](#appendix-c--traceability-matrix)
- [Appendix D — Open issues and decisions log](#appendix-d--open-issues-and-decisions-log)

# 1 Introduction

> ***Guidance:** Orient the reader: what this document covers, who it is written for, and how it fits with the other requirements and project documents.*

## 1.1 Purpose of this document

This Business Requirements Specification describes the business needs, goals, constraints and operating expectations for \[initiative name\]. Once approved, it is the agreed basis for \[approving the business case / selecting a solution / deriving stakeholder requirements\].

## 1.2 Intended audience

- \[Business sponsor and steering committee\]

- \[Owners and managers of the business processes in scope\]

- \[Business analysts and requirements engineers who will derive stakeholder and system requirements\]

- \[Solution architects, project managers, and compliance or risk reviewers\]

## 1.3 Related documents

| **Document** | **ID / location** | **Relationship to this BRS** |
|----|----|----|
| *Business case* | *\[ID / link\]* | *Justifies the investment; this BRS details the business needs behind it* |
| *Stakeholder Requirements Specification (StRS)* | *\[ID / link\]* | *Derived from this BRS* |
| *Operational concept (OpsCon / ConOps)* | *\[ID / link\]* | *Expands sections 16 and 17 of this BRS* |
|  |  |  |

## 1.4 Definitions

> ***Guidance:** Define business terms that readers could misread or that have a specific meaning in your organization. Use one definition per term and use the term consistently throughout.*

| **Term** | **Definition** |
|----|----|
| *Business requirement* | *A statement of what the organization needs to achieve or be able to do, expressed independently of any particular solution.* |
| *Complete application* | *An application for which every mandatory field and supporting document has been received.* |
|  |  |
|  |  |

## 1.5 References

| **Ref.** | **Title** | **Version / date** | **Source / location** |
|----|----|----|----|
| \[R1\] | ISO/IEC/IEEE 29148:2018 Systems and software engineering — Life cycle processes — Requirements engineering | 2018 | ISO / IEC / IEEE |
| \[R2\] | \[Corporate strategy or business plan\] |  |  |
| \[R3\] | \[Applicable policy, regulation or contract\] |  |  |
|  |  |  |  |

## 1.6 Acronyms and abbreviations

| **Acronym** | **Meaning**                            |
|-------------|----------------------------------------|
| BRS         | Business Requirements Specification    |
| StRS        | Stakeholder Requirements Specification |
| SyRS        | System Requirements Specification      |
| SRS         | Software Requirements Specification    |
| OpsCon      | Operational Concept                    |
| KPI         | Key performance indicator              |
|             |                                        |

# 2 Business purpose

> ***Guidance:** Explain why the organization is doing this. Describe the problem or opportunity, its effect on the business today, and what happens if nothing changes.*
>
> *Keep it short enough for a senior sponsor to read in two minutes, and do not describe a solution here.*

## 2.1 Problem or opportunity statement

|  |  |
|----|----|
| **The problem / opportunity of** | \[Describe the problem or opportunity\] |
| **affects** | \[Who is affected: customers, staff, partners, the organization\] |
| **the impact of which is** | \[Business impact: cost, revenue, risk, customer experience, compliance\] |
| **a successful outcome would** | \[Describe the desired end state in business terms\] |

## 2.2 Business drivers

- \[Driver, e.g. regulatory change effective DD-MMM-YYYY\]

- \[Driver, e.g. rising operating cost or customer attrition\]

- \[Driver, e.g. strategic objective from the corporate plan\]

## 2.3 Cost of inaction

\[Describe the consequences of not proceeding, with figures where possible: lost revenue, penalties, cost growth, risk exposure.\]

# 3 Business scope

> ***Guidance:** Set the boundaries of the business change: which business areas, processes, products, customer groups, locations and time period it covers. Being explicit about what is out of scope prevents scope creep later.*

## 3.1 In scope

| **ID** | **Scope item** | **Notes** |
|----|----|----|
| *S-01* | *Onboarding of new retail customers through branch and online channels* | *All regions* |
|  |  |  |
|  |  |  |

## 3.2 Out of scope

| **ID** | **Excluded item** | **Reason / where it is handled** |
|----|----|----|
| *X-01* | *Business and corporate customer onboarding* | *Planned for phase 2* |
|  |  |  |
|  |  |  |

## 3.3 Assumptions

| **ID** | **Assumption** | **Owner** | **Impact if false** |
|--------|----------------|-----------|---------------------|
|        |                |           |                     |
|        |                |           |                     |

## 3.4 Dependencies

| **ID** | **Dependency** | **Depends on** | **Needed by** |
|--------|----------------|----------------|---------------|
|        |                |                |               |
|        |                |                |               |

# 4 Business overview

> ***Guidance:** Describe the part of the business affected as it operates today: what it does, for whom, at what volume, and how it is organized at a high level.*
>
> *Include a context diagram showing the business area, its customers, suppliers, partners, regulators and other external parties, and the main flows between them. This gives reviewers from outside the area enough background to follow the rest of the document.*

## 4.1 Current state

\[Describe how the business area operates today.\]

## 4.2 Key facts and figures

| **Measure** | **Current value** | **Source** | **As of** |
|----|----|----|----|
| *Applications received per month* | *\[12,000\]* | *\[MI report\]* | *\[MMM-YYYY\]* |
| *Median time from application to account opening* | *\[10 working days\]* | *\[Process audit\]* | *\[MMM-YYYY\]* |
|  |  |  |  |
|  |  |  |  |

## 4.3 Business context diagram

\[Insert context diagram\]

# 5 Major stakeholders

> ***Guidance:** Identify the groups and individuals who are affected by the change, have influence over it, or have an interest in it, inside and outside the organization. Include groups that may resist it, as well as regulators and auditors.*
>
> *For each, note what they care about. This list is the starting point for eliciting stakeholder requirements (StRS).*

| **ID** | **Stakeholder (group / role)** | **Interests and concerns** | **Influence (H/M/L)** | **Impact on them (H/M/L)** | **Representative** |
|----|----|----|----|----|----|
| *SH-01* | *Retail customers* | *Faster, simpler onboarding; protection of personal data* | *L* | *H* | *\[Customer experience team\]* |
| *SH-02* | *Branch operations staff* | *Workload, training, fewer manual checks* | *M* | *H* | *\[Head of branch operations\]* |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

# 6 Business environment

> ***Guidance:** Describe the external and internal factors that shape the business need or limit the options: market and competition, laws and regulations, industry standards, economic conditions, technology trends, social expectations, and internal factors such as strategy and culture.*
>
> *Flag any factor expected to change during the life of the initiative.*

| **Category** | **Factor** | **Effect on the business need** | **Source** |
|----|----|----|----|
| *Regulatory* | *\[New data-protection rules effective DD-MMM-YYYY\]* | *Personal data collected at onboarding must be minimized and consent recorded* | *\[Regulation ref.\]* |
| Political |  |  |  |
| Economic |  |  |  |
| Social |  |  |  |
| Technological |  |  |  |
| Legal / regulatory |  |  |  |
| Environmental |  |  |  |
| Market / competitive |  |  |  |
| Internal (strategy, culture, capability) |  |  |  |

# 7 Mission, goals and objectives

> ***Guidance:** Connect the initiative to the organization's mission and strategy, then state the goals it must achieve and the measurable objectives that show each goal has been met.*
>
> *Make objectives SMART (specific, measurable, achievable, relevant, time-bound). Every business requirement in Appendix A should trace to at least one goal or objective here.*

## 7.1 Mission and strategic alignment

\[State the organization's or business unit's mission and the strategic objectives this initiative supports.\]

## 7.2 Goals and objectives

| **ID** | **Goal** | **Objective** | **KPI / measure** | **Baseline** | **Target** | **By** |
|----|----|----|----|----|----|----|
| *G-01 / O-01* | *Improve the onboarding experience* | *Reduce elapsed time from complete application to account opening* | *Median working days* | *10 days* | *1 day* | *\[Q4 YYYY\]* |
| *G-01 / O-02* | *Improve the onboarding experience* | *Reduce applications abandoned before completion* | *% abandoned* | *30%* | *≤ 10%* | *\[Q4 YYYY\]* |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## 7.3 Success criteria and benefits

\[Describe how the sponsor will judge overall success and when benefits are expected to be realized and measured.\]

# 8 Business model

> ***Guidance:** Describe how the business area creates, delivers and captures value, and how the initiative changes that.*
>
> *Where the model is changing, show the current and future state side by side. Leave unchanged elements as "No change".*

| **Element**            | **Current state** | **Future state** |
|------------------------|-------------------|------------------|
| Customer segments      |                   |                  |
| Value proposition      |                   |                  |
| Channels               |                   |                  |
| Customer relationships |                   |                  |
| Revenue streams        |                   |                  |
| Key activities         |                   |                  |
| Key resources          |                   |                  |
| Key partners           |                   |                  |
| Cost structure         |                   |                  |

# 9 Information environment

> ***Guidance:** Describe the information the business relies on and produces: what it is, where it comes from, who owns it, who uses it, how sensitive it is and how long it must be kept.*
>
> *List the existing systems and data stores that hold this information, since they constrain or will be affected by the change. Stay at the level of business information, not database design.*

## 9.1 Information items

| **ID** | **Information item** | **Source** | **Owner** | **Used by** | **Sensitivity** | **Retention** |
|----|----|----|----|----|----|----|
| *INF-01* | *Customer identity documents* | *Customer upload; branch scan* | *Operations* | *KYC team; audit* | *Confidential (personal data)* | *\[N\] years after account closure* |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## 9.2 Existing systems and data stores

| **System / data store** | **Purpose** | **Business owner** | **Information held** | **Expected change** |
|----|----|----|----|----|
| *\[Core banking system\]* | *Account records* | *\[Owner\]* | *INF-02, INF-03* | *Modify* |
|  |  |  |  |  |
|  |  |  |  |  |

Expected change: Retain / Modify / Replace / Retire.

# 10 Business processes

> ***Guidance:** Identify the business processes in scope and describe how each will work after the change: trigger, main steps, roles, inputs, outputs and outcome. Make clear what differs from today.*
>
> *Use process diagrams (for example BPMN) for complex processes, and keep detailed step-level models in an appendix or a linked document.*

## 10.1 Process inventory

| **ID** | **Process name** | **Process owner** | **Trigger** | **Outcome** | **Change** |
|----|----|----|----|----|----|
| *P-01* | *Open retail account* | *\[Head of retail operations\]* | *Customer submits application* | *Account opened and customer notified* | *Changed* |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

Change: New / Changed / Unchanged / Retired.

## 10.2 Process descriptions

Repeat the table below for each process marked New or Changed.

### \[P-01\] \[Process name\]

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<tbody>
<tr>
<td><strong>Purpose</strong></td>
<td>[Why this process exists]</td>
</tr>
<tr>
<td><strong>Trigger</strong></td>
<td>[Event that starts the process]</td>
</tr>
<tr>
<td><strong>Roles / actors</strong></td>
<td>[Who performs or takes part in the process]</td>
</tr>
<tr>
<td><strong>Inputs</strong></td>
<td>[Information or materials consumed]</td>
</tr>
<tr>
<td><strong>Main steps (future state)</strong></td>
<td><p>1. [Step]</p>
<p>2. [Step]</p>
<p>3. [Step]</p></td>
</tr>
<tr>
<td><strong>Outputs</strong></td>
<td>[Information or products produced]</td>
</tr>
<tr>
<td><strong>Outcome / end state</strong></td>
<td>[What is true when the process completes successfully]</td>
</tr>
<tr>
<td><strong>Volumes and frequency</strong></td>
<td>[e.g. 12,000 per month; peaks in March]</td>
</tr>
<tr>
<td><strong>Pain points today</strong></td>
<td>[Problems with the current process]</td>
</tr>
<tr>
<td><strong>Changes from current state</strong></td>
<td>[What is different and why]</td>
</tr>
<tr>
<td><strong>Related rules / goals</strong></td>
<td>[RULE-xx; G-xx / O-xx]</td>
</tr>
<tr>
<td><strong>Process diagram</strong></td>
<td>[Insert or link diagram]</td>
</tr>
</tbody>
</table>

# 11 Business operational policies and rules

> ***Guidance:** List the policies, business rules and decisions that govern how the business operates within scope, whether they come from internal policy, contracts or law.*
>
> *Write each rule as one testable statement and cite its source, so it can be rechecked when the source changes. Write down rules that are only implied today ("everyone knows").*

| **ID** | **Rule statement** | **Type** | **Source** | **Applies to** | **Owner** |
|----|----|----|----|----|----|
| *RULE-01* | *An account shall not be opened until the customer's identity has been verified against an approved document.* | *Rule* | *\[KYC policy v3, §4.2\]* | *P-01* | *Compliance* |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

Type: Policy / Rule / Decision / Calculation.

# 12 Business operational constraints

> ***Guidance:** Record limits the business must work within that this initiative cannot change: budget, deadlines, regulatory dates, staffing, approved technology, contracts, locations and agreements with employee representatives.*
>
> *A constraint restricts the options; it is not something the solution delivers. State its source and the consequence of breaching it.*

| **ID** | **Constraint** | **Category** | **Source** | **Consequence if breached** |
|----|----|----|----|----|
| *C-01* | *The new process shall be live before \[DD-MMM-YYYY\]* | *Schedule* | *\[Regulatory deadline ref.\]* | *Regulatory penalties; licence conditions* |
| *C-02* | *Total capital spend shall not exceed \[amount\]* | *Budget* | *\[Investment committee decision\]* | *Re-approval required* |
|  |  |  |  |  |
|  |  |  |  |  |

# 13 Business operational modes

> ***Guidance:** Describe the different ways the business must be able to operate and what is expected in each, for example normal operation, peak periods, degraded operation when a system or site is unavailable, business-continuity mode, and migration or parallel running.*
>
> *For each mode, state how the business enters and leaves it and what must keep working.*

| **Mode** | **Description** | **Entry condition** | **Exit condition** | **Business expectations in this mode** |
|----|----|----|----|----|
| Normal |  |  |  |  |
| Peak |  |  |  |  |
| Degraded |  |  |  |  |
| Business continuity |  |  |  |  |
| Transition / parallel run |  |  |  |  |

# 14 Business operational quality

> ***Guidance:** State the quality the business needs from its operations, in business terms and with a measure: service levels to customers, availability during business hours, accuracy, timeliness, security and privacy, compliance, accessibility and customer satisfaction.*
>
> *These expectations later become non-functional stakeholder and system requirements, so give each one a measure and a target.*

| **ID** | **Quality attribute** | **Business expectation** | **Measure** | **Target** |
|----|----|----|----|----|
| *Q-01* | *Timeliness* | *Customers receive a decision on a complete application on the same working day* | *% of decisions issued the same working day* | *≥ 95%* |
| *Q-02* | *Accuracy* | *Accounts are opened with correct customer details* | *% of accounts needing correction in first 30 days* | *≤ 1%* |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

# 15 Business structure

> ***Guidance:** Describe the organizational units, roles and locations involved, their responsibilities, and how they will change: new roles, changed responsibilities, reporting lines, headcount, sourcing and locations.*

## 15.1 Organizational units and roles

| **Unit / role** | **Responsibilities** | **Location(s)** | **People affected** | **Change** |
|----|----|----|----|----|
| *Branch onboarding officer* | *Verify identity documents; open accounts* | *All branches* | *\[~250\]* | *Changed: identity checks move to central team* |
|  |  |  |  |  |
|  |  |  |  |  |

## 15.2 Organization chart

\[Insert organization chart for the affected area, current and future\]

# 16 High-level operational concept

> ***Guidance:** Describe in narrative form how the business will operate once the change is in place, from the point of view of the people doing the work and the customers they serve. Explain how processes, people, information and any supporting systems work together, without specifying a solution design.*
>
> *If a separate operational concept (OpsCon / ConOps) document exists, summarize it here and reference it.*

\[Describe the future-state operation.\]

\[Insert high-level future-state diagram\]

# 17 High-level operational scenarios

> ***Guidance:** Give a small number of end-to-end stories showing the business operating in the future state. Cover the typical case, high-volume periods, important exceptions and failure situations.*
>
> *Scenarios help stakeholders validate the BRS, and they are reused later to derive stakeholder requirements and acceptance tests.*

## 17.1 Scenario summary

| **ID** | **Scenario** | **Operational mode** | **Related goals / processes** |
|----|----|----|----|
| *SC-01* | *Customer opens an account online with valid documents* | *Normal* | *G-01; P-01* |
| *SC-02* | *Identity verification service is unavailable during peak period* | *Degraded* | *G-01; P-01; Q-01* |
|  |  |  |  |
|  |  |  |  |

## 17.2 Scenario descriptions

Repeat the table below for each scenario.

### \[SC-01\] \[Scenario title\]

<table>
<colgroup>
<col style="width: 27%" />
<col style="width: 72%" />
</colgroup>
<tbody>
<tr>
<td><strong>Related goals / objectives</strong></td>
<td>[G-xx / O-xx]</td>
</tr>
<tr>
<td><strong>Actors</strong></td>
<td>[People, organizations or systems involved]</td>
</tr>
<tr>
<td><strong>Operational mode</strong></td>
<td>[Normal / Peak / Degraded / ...]</td>
</tr>
<tr>
<td><strong>Preconditions</strong></td>
<td>[What must be true before the scenario starts]</td>
</tr>
<tr>
<td><strong>Trigger</strong></td>
<td>[Event that starts the scenario]</td>
</tr>
<tr>
<td><strong>Main sequence</strong></td>
<td><p>1. [Step]</p>
<p>2. [Step]</p>
<p>3. [Step]</p></td>
</tr>
<tr>
<td><strong>Alternative and exception paths</strong></td>
<td>[What happens when things differ from the main sequence]</td>
</tr>
<tr>
<td><strong>Outcome</strong></td>
<td>[End state and the business result]</td>
</tr>
</tbody>
</table>

# Appendix A — Business requirements register

> ***Guidance:** List the individual business requirements this BRS establishes. Each should state one need of the business, be independent of any solution, trace to a goal or objective, and have an objective way to tell whether it has been met.*
>
> *Suggested pattern: "The \[organization / business unit\] shall be able to \[capability or outcome\] \[condition\] \[measure\]." Priority uses MoSCoW: Must / Should / Could / Won't (this time). Status: Proposed / Agreed / Deferred / Rejected / Withdrawn.*

| **ID** | **Business requirement** | **Rationale** | **Priority** | **Source** | **Goal / objective** | **Acceptance criterion** | **Status** |
|----|----|----|----|----|----|----|----|
| *BR-01* | *The organization shall be able to open a retail account for a verified customer within one working day of receiving a complete application.* | *The current 10-day cycle drives 30% abandonment.* | *Must* | *SH-01; sponsor workshop \[date\]* | *G-01 / O-01* | *95% of complete applications opened within one working day over three consecutive months* | *Proposed* |
| *BR-02* | *The organization shall be able to show, for every account, evidence of identity verification that satisfies RULE-01.* | *Regulatory obligation.* | *Must* | *RULE-01; \[regulation ref.\]* | *G-02* | *Audit sample of 100 accounts shows 100% with retrievable evidence* | *Proposed* |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |

# Appendix B — Requirement quality checklist

> ***Guidance:** Run this checklist before submitting the BRS for review and approval. It reflects the characteristics of well-formed requirements and requirement sets described in ISO/IEC/IEEE 29148, phrased here as practical checks.*

### B.1 Each individual requirement

| **Characteristic** | **What to check** | **Pass** | **Notes / IDs failing** |
|----|----|----|----|
| Necessary | Removing it would leave a business need unmet or a goal unsupported. | ☐ |  |
| Appropriate | It is stated at the business level and does not prescribe a solution or design. | ☐ |  |
| Unambiguous | It can be read only one way; no vague terms such as "fast", "user-friendly", "and/or" or "etc." | ☐ |  |
| Complete | It can be understood without further information; conditions and measures are stated. | ☐ |  |
| Singular | It expresses one need, not several bundled together. | ☐ |  |
| Feasible | It can be achieved within known constraints of cost, time, technology and regulation. | ☐ |  |
| Verifiable | There is an objective way to show it has been met (an acceptance criterion is defined). | ☐ |  |
| Correct | It accurately reflects the business or stakeholder need it came from. | ☐ |  |
| Conforming | It follows the agreed template, language conventions and ID scheme. | ☐ |  |

### B.2 The set of requirements as a whole

| **Characteristic** | **What to check** | **Pass** | **Notes** |
|----|----|----|----|
| Complete | Together, the requirements cover every goal, objective and in-scope item. | ☐ |  |
| Consistent | No requirements conflict with or duplicate one another; terms are used consistently. | ☐ |  |
| Feasible | The set as a whole can be achieved within the constraints in section 12. | ☐ |  |
| Comprehensible | The intended readers can understand what the business needs and why. | ☐ |  |
| Able to be validated | It can be shown that meeting the set will achieve the business goals in section 7. | ☐ |  |

# Appendix C — Traceability matrix

> ***Guidance:** Show how each business requirement traces back to goals and stakeholders and forward to stakeholder and system requirements, and how it will be verified. Keep this matrix up to date as downstream specifications are written.*

| **BR ID** | **Goal / objective** | **Stakeholders** | **Process / scenario** | **StRS requirement IDs** | **SyRS / SRS requirement IDs** | **Verification method** | **Status** |
|----|----|----|----|----|----|----|----|
| *BR-01* | *G-01 / O-01* | *SH-01, SH-02* | *P-01; SC-01, SC-02* | *\[StRS-014, StRS-015\]* | *\[SyRS-102\]* | *Analysis of 3 months of operational data* | *Open* |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |

Verification method: Inspection / Analysis / Demonstration / Test.

# Appendix D — Open issues and decisions log

> ***Guidance:** Track open questions, unresolved conflicts between stakeholders, and decisions taken while the BRS is being prepared. Close every open item, or explicitly accept it, before approval.*

| **ID** | **Issue / decision** | **Raised by** | **Date raised** | **Owner** | **Due** | **Resolution / decision** | **Status** |
|----|----|----|----|----|----|----|----|
| *I-01* | *Is online onboarding in scope for joint accounts?* | *\[Name\]* | *\[DD-MMM-YYYY\]* | *\[Sponsor\]* | *\[DD-MMM-YYYY\]* | *\[Decision and rationale\]* | *Open* |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |

— End of document —
