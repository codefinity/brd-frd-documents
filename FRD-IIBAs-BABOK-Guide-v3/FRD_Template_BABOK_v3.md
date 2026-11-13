# Functional Requirements Document (FRD)

**\[Initiative name\] · \[Solution name\]**

Template based only on the BABOK® Guide v3 (IIBA) · Version \[0.1\] · \[YYYY-MM-DD\]

**Contents**

- [How to use this template](#how-to-use-this-template)
- [Document control](#document-control)
- [1. Introduction](#1-introduction)
- [2. Stakeholders](#2-stakeholders)
- [3. Requirements architecture](#3-requirements-architecture)
- [4. Requirements models](#4-requirements-models)
- [5. Functional requirements](#5-functional-requirements)
- [6. Non-functional requirements](#6-non-functional-requirements)
- [7. Interface requirements](#7-interface-requirements)
- [8. Transition requirements](#8-transition-requirements)
- [9. Assumptions and constraints](#9-assumptions-and-constraints)
- [10. Verification](#10-verification)
- [11. Validation](#11-validation)
- [12. Traceability](#12-traceability)
- [13. Prioritization](#13-prioritization)
- [14. Change control](#14-change-control)
- [15. Open items](#15-open-items)
- [16. Glossary](#16-glossary)
- [17. Approval](#17-approval)

# How to use this template

Make one copy per solution or release. Replace every \[bracketed placeholder\], then delete this section, the *Guidance* notes and the example rows before the first review.

- **Basis:** this template uses only A Guide to the Business Analysis Body of Knowledge (BABOK Guide) v3. BABOK does not prescribe a document format, so the sections follow its concepts: the requirements classification schema (section 2.3 of BABOK), the five model categories of Specify and Model Requirements (task 7.1), and the Requirements Life Cycle Management tasks (chapter 5). The table at the end of this section maps every section to its BABOK task and techniques.

- **What an FRD holds in BABOK terms:** solution requirements, which BABOK divides into functional requirements (the capabilities the solution must have) and non-functional requirements (the conditions or qualities under which it must work). Transition requirements can be included in section 8. Business and stakeholder requirements stay in the BRD; this document traces to them.

- **Requirements versus designs:** BABOK separates requirements (the need) from designs (a usable representation of a solution). Keep screen layouts and technical choices in design documents and link them through traceability (section 12).

- **Example rows** continue the running example from the BRD template, automating accounts-payable invoice processing, and trace to its IDs (BR-01 to BR-03, SR-01 to SR-03).

## Requirement attributes

BABOK (task 3.4) lists the attributes commonly recorded for each requirement. The tables in this template show the most-used ones; record the others in your requirements repository.

| **Attribute** | **What to record** | **Shown in tables** |
|----|----|----|
| Absolute reference | A unique ID that never changes or gets reused | Yes (ID) |
| Author | Who wrote the requirement | No |
| Complexity | How hard it is expected to be to implement | No |
| Ownership | The person or group who needs it and will own it after implementation | No |
| Priority | Relative importance (section 13) | Yes |
| Risks | Uncertain events that could affect the requirement | No |
| Source | Where it came from: the BRD, a stakeholder, a regulation | Yes (Traces to) |
| Stability | How mature the requirement is, and how likely to change | No |
| Status | Proposed, Verified, Validated, Approved, Deferred or Rejected | Yes |
| Urgency | How soon it is needed | No |

## Requirement status

| **Status** | **Meaning** |
|----|----|
| Proposed | Written but not yet reviewed |
| Verified | Meets the quality characteristics in section 10 |
| Validated | Shown to deliver value toward a business objective (section 11) |
| Approved | Agreed by the approvers in section 17 |
| Deferred | Postponed to a later release |
| Rejected | Not to be implemented |

## Writing a requirement

State one requirement per row, in the form "The solution shall \[capability\]", and give it acceptance criteria (BABOK technique 10.1, Acceptance and Evaluation Criteria) that show when it is met. Use models (section 4) wherever a picture or matrix states the requirement more clearly than text.

## Mapping to BABOK v3

| **FRD section** | **BABOK task** | **BABOK techniques** |
|----|----|----|
| 1\. Introduction | 6.4 Define Change Strategy (solution scope) | 10.41 Scope Modelling |
| 2\. Stakeholders | 2.4 Stakeholders | 10.43 Stakeholder List, Map, or Personas |
| 3\. Requirements architecture | 7.4 Define Requirements Architecture | 10.22 Functional Decomposition; 10.41 Scope Modelling |
| 4\. Requirements models | 7.1 Specify and Model Requirements | See section 4 for each model category |
| 5\. Functional requirements | 7.1 Specify and Model Requirements | 10.1 Acceptance and Evaluation Criteria; 10.22 Functional Decomposition |
| 6\. Non-functional requirements | 7.1 Specify and Model Requirements | 10.30 Non-Functional Requirements Analysis |
| 7\. Interface requirements | 7.1 Specify and Model Requirements | 10.24 Interface Analysis |
| 8\. Transition requirements | 6.4 Define Change Strategy | 10.1 Acceptance and Evaluation Criteria |
| 9\. Assumptions and constraints | 7.1 Specify and Model Requirements; 6.3 Assess Risks | 10.38 Risk Analysis and Management |
| 10\. Verification | 7.2 Verify Requirements | 10.37 Reviews; 10.26 Item Tracking |
| 11\. Validation | 7.3 Validate Requirements | 10.1 Acceptance and Evaluation Criteria; 10.28 Metrics and KPIs |
| 12\. Traceability | 5.1 Trace Requirements | — |
| 13\. Prioritization | 5.3 Prioritize Requirements | 10.33 Prioritization |
| 14\. Change control | 5.2 Maintain Requirements; 5.4 Assess Requirements Changes | 10.26 Item Tracking |
| 15\. Open items | 5.2 Maintain Requirements | 10.26 Item Tracking |
| 16\. Glossary | 7.1 Specify and Model Requirements | 10.23 Glossary |
| 17\. Approval | 5.5 Approve Requirements | 10.37 Reviews |

# Document control

| **Field** | **Value** |
|----|----|
| **Document title** | Functional Requirements Document for \[Solution name\] |
| **Document ID** | \[FRD-2026-001\] |
| **Initiative** | \[Project or change initiative name\] |
| **Release** | \[Release 1\] |
| **Related BRD** | \[BRD title, ID and version, e.g. BRD-2026-014 v1.0\] |
| **Business analyst** | \[Name\] |
| **Sponsor** | \[Name, title\] |
| **Current version** | \[0.1\] |
| **Status** | \[Draft / Under review / Approved\] |
| **Last updated** | \[YYYY-MM-DD\] |

## Version history

| **Version** | **Date**       | **Author** | **Summary of changes**                |
|-------------|----------------|------------|---------------------------------------|
| 0.1         | \[YYYY-MM-DD\] | \[Name\]   | Initial draft                         |
| \[0.2\]     | \[YYYY-MM-DD\] | \[Name\]   | \[Changes after verification review\] |

# 1. Introduction

## 1.1 Purpose

\[State what this FRD specifies and who uses it. Example: This FRD specifies the solution requirements for Release 1 of the \[Invoice Automation Solution\]. Developers, testers and solution architects use it to design, build and test the solution; business owners use it to confirm the solution will meet their needs.\]

## 1.2 Business need and objectives

> *Guidance: summarise the need and the business requirements this solution addresses, and point to the BRD for detail. Do not restate the BRD.*

| **Business requirement (BRD)** | **Summary** | **Measure** |
|----|----|----|
| \[BR-01\] | \[Reduce invoice approval time\] | \[9 days → 3 days by \[date\]\] |
| \[BR-02\] | \[Capture early-payment discounts\] | \[35% → 80% of eligible invoices\] |
| \[BR-03\] | \[Reduce supplier status queries\] | \[400 → 200 a month\] |

## 1.3 Solution scope

> *Guidance: state what the solution includes and excludes in this release, consistent with the change strategy in the BRD. A scope model (a context diagram showing the solution boundary) is recommended.*

- **In scope:** \[invoice capture from email, data extraction, PO matching, approval workflow, supplier status portal, ERP integration\]

- **Out of scope:** \[payment execution (stays in the ERP); non-PO invoices; expense claims\]

Scope model: \[link or attachment\]

## 1.4 Audience

| **Reader**                         | **Sections to read**  |
|------------------------------------|-----------------------|
| Developers and solution architects | 3 to 9                |
| Testers                            | 4, 5, 6, 7, 8, 11, 12 |
| Business owners and approvers      | 1, 2, 5, 6, 11, 17    |

## 1.5 References

| **Document**                                     | **Version** | **Location** |
|--------------------------------------------------|-------------|--------------|
| \[Business Requirements Document, BRD-2026-014\] | \[1.0\]     | \[Link\]     |
| \[Delegation of authority policy\]               | \[2025\]    | \[Link\]     |
| \[Design documents and prototypes\]              | \[0.3\]     | \[Link\]     |

# 2. Stakeholders

> *Guidance: list the stakeholders for these requirements, using the BABOK stakeholder roles: business analyst, customer, domain subject matter expert, end user, implementation subject matter expert, operational support, project manager, regulator, sponsor, supplier and tester. Show each one's involvement with this document.*

| **Stakeholder** | **BABOK role** | **Interest in these requirements** | **Involvement (RACI)** |
|----|----|----|----|
| \[Name\], \[title\] | Sponsor | \[Approves scope and funding\] | A |
| \[Name\] | Business analyst | \[Elicits, specifies and maintains requirements\] | R |
| \[AP manager\] | Domain subject matter expert | \[Correct invoice handling\] | C |
| \[AP clerks\] | End user | \[Daily use of the work queue\] | C |
| \[Approvers\] | End user | \[Fast mobile approval\] | C |
| \[Solution architect\] | Implementation subject matter expert | \[Feasibility and design\] | C |
| \[IT service desk\] | Operational support | \[Support after go-live\] | I |
| \[Internal audit\] | Regulator | \[Controls and audit trail\] | C |
| \[QA lead\] | Tester | \[Testable requirements\] | C |
| \[Suppliers\] | Customer | \[Visibility of invoice status\] | I |

# 3. Requirements architecture

> *Guidance: show how the requirements fit together, so readers can see that the set is complete and consistent (BABOK task 7.4). Describe how the requirements are organized, which views are used, and how they relate to the BRD and to designs.*

## 3.1 Organization of the requirements

Functional requirements are grouped by capability, taken from a functional decomposition of the solution:

| **Capability code** | **Capability** | **Description** | **Stakeholder requirements served (BRD)** |
|----|----|----|----|
| \[CAP\] | \[Invoice capture\] | \[Receive invoices, extract data, match to PO and goods receipt\] | \[SR-01\] |
| \[APR\] | \[Approval workflow\] | \[Route, approve, reject, remind and escalate\] | \[SR-02\] |
| \[SUP\] | \[Supplier status\] | \[Let suppliers see their invoices' status\] | \[SR-03\] |

Functional decomposition diagram: \[link or attachment\]

## 3.2 Views used

| **View** | **Model category (section 4)** | **Purpose** |
|----|----|----|
| \[Roles and permissions view\] | People and roles | \[Who can do what\] |
| \[Business rules view\] | Rationale | \[Rules the solution enforces\] |
| \[Process view\] | Activity flow | \[How work moves through the solution\] |
| \[Capability view\] | Capability | \[What the solution does\] |
| \[Data view\] | Data and information | \[What information the solution holds and how it changes\] |

## 3.3 Related designs

| **Design** | **Version** | **Location** | **Requirements it satisfies** |
|----|----|----|----|
| \[Wireframes\] | \[0.8\] | \[Link\] | \[FR-APR-01 to FR-APR-03\] |
| \[Integration design\] | \[0.3\] | \[Link\] | \[IF-01, IF-02\] |

# 4. Requirements models

> *Guidance: BABOK groups models into five categories (task 7.1). Use the ones that help; delete the rest. Each subsection names typical BABOK techniques for that category.*

## 4.1 People and roles

*Techniques: 10.39 Roles and Permissions Matrix; 10.32 Organizational Modelling; 10.43 Stakeholder List, Map, or Personas.*

| **Function** | **AP clerk** | **Approver** | **Finance controller** | **Supplier user** | **Administrator** |
|----|----|----|----|----|----|
| View invoices | All | Assigned to them | All | Own company only | All |
| Correct extracted data | Yes | — | Yes | — | — |
| Approve or reject | — | Assigned to them | Above threshold (BRL-01) | — | — |
| Maintain routing rules | — | — | Yes | — | Yes |
| Manage users | — | — | — | Own company's users | Yes |

## 4.2 Rationale

*Techniques: 10.9 Business Rules Analysis; 10.17 Decision Modelling; 10.41 Scope Modelling; 10.40 Root Cause Analysis.*

**Business rules.** BABOK separates definitional rules (what something is) from behavioural rules (what people or the solution must or must not do).

| **ID** | **Rule** | **Type** | **Source** | **Enforced by** |
|----|----|----|----|----|
| BRL-01 | \[Invoices above \[threshold amount\] need approval from the finance controller as well as the cost-centre owner.\] | Behavioural | \[Delegation of authority policy\] | \[FR-APR-01\] |
| BRL-04 | \[An invoice "matches" when its amount is within \[±2%\] of the PO and goods-receipt value.\] | Definitional | \[Finance policy\] | \[FR-CAP-03\] |

**Decision model (example).**

| **Invoice amount** | **Cost centre has owner** | **Approvers** |
|----|----|----|
| \[Up to threshold\] | Yes | Cost-centre owner |
| \[Above threshold\] | Yes | Cost-centre owner, then finance controller |
| \[Any\] | No | Finance controller |

## 4.3 Activity flow

*Techniques: 10.35 Process Modelling; 10.47 Use Cases and Scenarios; 10.48 User Stories.*

**Process model:** \[link to the future-state process model\]

**Use case (example).**

| **Element** | **Description** |
|----|----|
| Name | \[UC-01 Approve or reject an invoice\] |
| Goal | \[The approver decides on an invoice\] |
| Actors | \[Approver (primary); ERP; notification service\] |
| Trigger | \[An invoice is routed to the approver\] |
| Preconditions | \[The approver is signed in; the invoice is "Awaiting approval"\] |
| Basic flow | \[1. The solution notifies the approver. 2. The approver opens the invoice. 3. The solution shows the invoice, match result and history. 4. The approver approves. 5. The solution records the decision and routes onward or marks the invoice Approved.\] |
| Alternative flows | \[4a. The approver rejects and enters a reason.\] |
| Exception flows | \[5a. The ERP is unavailable: the solution queues the update and retries.\] |
| Postconditions | \[The decision is recorded with user, time and reason\] |
| Related requirements | \[FR-APR-01 to FR-APR-03\] |

**User story (example).** As an \[approver\], I want \[to approve invoices from my phone\], so that \[suppliers are not kept waiting while I am away from my desk\].

> Given an invoice is awaiting my approval
>
> When I select "Approve" on my phone
>
> Then the invoice status changes to "Approved"
>
> And the ERP shows the approval within 5 minutes

## 4.4 Capability

*Techniques: 10.22 Functional Decomposition; 10.6 Business Capability Analysis; 10.36 Prototyping.*

\[Attach the functional decomposition (section 3.1) and link prototypes or wireframes. Each leaf of the decomposition should map to one or more functional requirements in section 5.\]

## 4.5 Data and information

*Techniques: 10.15 Data Modelling; 10.12 Data Dictionary; 10.13 Data Flow Diagrams; 10.44 State Modelling; 10.23 Glossary.*

**Data model:** \[link to the logical data model\]

**Data dictionary (example).**

| **Element** | **Description** | **Type and format** | **Allowed values or rule** | **Required** |
|----|----|----|----|----|
| \[Invoice number\] | \[Supplier's reference for the invoice\] | \[Text, up to 30 characters\] | \[Unique per supplier\] | Yes |
| \[Invoice amount\] | \[Total payable, including tax\] | \[Decimal (13,2)\] | \[Greater than 0\] | Yes |
| \[Invoice status\] | \[Where the invoice is in its life cycle\] | \[List\] | \[Received, Matched, Awaiting approval, Approved, Rejected, Paid\] | Yes |

**State model:** \[link to the invoice state diagram showing allowed status changes\]

# 5. Functional requirements

> *Guidance: functional requirements describe the capabilities the solution must have. Group them by the capabilities in section 3.1. Each needs acceptance criteria, a trace to the BRD, a priority and a status. Include what happens with invalid input and failures, not only the normal path.*

## 5.1 \[CAP: Invoice capture\]

| **ID** | **Requirement** | **Acceptance criteria** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| FR-CAP-01 | \[The solution shall create an invoice record within 60 seconds of an invoice email arriving in the AP mailbox.\] | \[50 sample invoices each create a record within 60 seconds.\] | \[SR-01, BR-01\] | High | \[Proposed\] |
| FR-CAP-02 | \[The solution shall extract the supplier name, invoice number, date, amount, tax and PO number from each invoice.\] | \[At least 95% of fields correct on 200 sample invoices.\] | \[SR-01\] | High | \[Proposed\] |
| FR-CAP-03 | \[The solution shall match each invoice to its PO and goods receipt under BRL-04.\] | \[All 20 matching scenarios give the expected result.\] | \[SR-01\] | High | \[Proposed\] |
| FR-CAP-04 | \[The solution shall reply to the sender with the reason when an attachment cannot be read.\] | \[A password-protected PDF triggers a reply within 5 minutes.\] | \[SR-01\] | Medium | \[Proposed\] |

## 5.2 \[APR: Approval workflow\]

| **ID** | **Requirement** | **Acceptance criteria** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| FR-APR-01 | \[The solution shall route each matched invoice to the approvers set by BRL-01 and the decision model in section 4.2.\] | \[All 20 routing scenarios reach the right approvers.\] | \[SR-02, BR-01\] | High | \[Proposed\] |
| FR-APR-02 | \[The solution shall let approvers approve or reject from a mobile browser, with a mandatory reason for rejection.\] | \[User story in section 4.3 passes; rejection without a reason is blocked.\] | \[SR-02\] | High | \[Proposed\] |
| FR-APR-03 | \[The solution shall send a reminder after 48 hours and escalate to the approver's manager after 96 hours.\] | \[Reminder and escalation sent at the right times in a time-shifted test.\] | \[SR-02, BR-02\] | Medium | \[Proposed\] |

> *Guidance: repeat for every capability in section 3.1.*

# 6. Non-functional requirements

> *Guidance: non-functional requirements describe the conditions under which the solution must remain effective, or the qualities it must have (BABOK technique 10.30). Use the BABOK categories below as a checklist; write "Not applicable" with a reason rather than skipping a category. Give each requirement a measure.*

| **Category** | **Code** | **What it covers** |
|----|----|----|
| Availability | AVL | When the solution can be used, and how much downtime is acceptable |
| Compatibility | CMP | Working with other solutions in the same environment |
| Functionality | FUN | How well the functions meet users' needs, including accuracy |
| Maintainability | MNT | How easily the solution can be changed, corrected or extended |
| Performance efficiency | PRF | Response times, throughput and use of resources |
| Portability | PRT | Moving the solution to other environments or devices |
| Reliability | REL | Working correctly over time; recovery after failure |
| Scalability | SCL | Handling growth in users, data or transactions |
| Security | SEC | Protection against unauthorized access, and accountability |
| Usability | USB | How easily users can learn and use the solution |
| Certification | CRT | Constraints for meeting external certifications or standards |
| Compliance | CPL | Regulatory, financial or legal constraints |
| Localization | LOC | Local languages, formats, laws and customs |
| Service level agreements | SLA | Commitments made to users about service levels |
| Extensibility | EXT | Adding new capabilities without major change |

| **ID** | **Category** | **Requirement** | **Acceptance criteria** | **Traces to** | **Priority** |
|----|----|----|----|----|----|
| NFR-PRF-01 | Performance efficiency | \[95% of screens shall respond within 2 seconds with 200 concurrent users.\] | \[Load test result.\] | \[SR-02\] | High |
| NFR-AVL-01 | Availability | \[The approval function shall be available 99.5% of business hours each month.\] | \[Monitoring report for the first month.\] | \[SR-02\] | High |
| NFR-SEC-01 | Security | \[Internal users shall sign in through single sign-on with multi-factor authentication.\] | \[Security test.\] | \[SR-01, SR-02\] | High |
| NFR-SEC-02 | Security | \[Every change and decision shall be logged with user, time, and old and new values.\] | \[Audit trail review.\] | \[Internal audit\] | High |
| NFR-USB-01 | Usability | \[A first-time approver shall complete an approval on a phone in under 60 seconds without training.\] | \[Observed test with 5 approvers.\] | \[SR-02\] | Medium |
| NFR-SCL-01 | Scalability | \[The solution shall handle 3 times the current invoice volume without redesign.\] | \[Load test at 15,000 invoices a month.\] | \[SR-01\] | Medium |
| NFR-CPL-01 | Compliance | \[Invoice and approval records shall be kept for \[n\] years.\] | \[Retention settings reviewed.\] | \[Tax law\] | High |
| NFR-LOC-01 | Localization | \[Amounts shall use the \[local currency format\] and dates \[YYYY-MM-DD\].\] | \[Screen review.\] | \[Company standard\] | Medium |
| NFR-CRT-01 | Certification | \[Not applicable: no external certification is required for this solution.\] | — | — | — |

# 7. Interface requirements

> *Guidance: identify every interface the solution has with people, processes and other systems, and what is exchanged (BABOK technique 10.24). For each, state what happens when the other side is unavailable.*

| **ID** | **Interface** | **Type** | **Exchanged** | **Frequency** | **If unavailable** | **Traces to** | **Priority** |
|----|----|----|----|----|----|----|----|
| IF-01 | \[ERP: purchase orders and goods receipts\] | \[System to system\] | \[PO and receipt data, in\] | \[Every 15 minutes\] | \[Retry every 5 minutes; alert after 3 failures\] | \[FR-CAP-03\] | High |
| IF-02 | \[ERP: approved invoices\] | \[System to system\] | \[Approved invoices, out\] | \[Within 5 minutes\] | \[Queue and retry\] | \[FR-APR-02\] | High |
| IF-03 | \[Approver screens\] | \[User interface\] | \[Invoice details and decisions\] | \[On demand\] | \[—\] | \[FR-APR-02\] | High |
| IF-04 | \[Supplier email\] | \[People outside the solution\] | \[Rejection notices, out\] | \[On event\] | \[Retry for 1 hour\] | \[SR-03\] | Medium |

# 8. Transition requirements

> *Guidance: transition requirements describe what is needed only to move from the current state to the future state, such as data conversion, training and running old and new processes in parallel. They stop applying once the transition is complete.*

| **ID** | **Category** | **Requirement** | **Acceptance criteria** | **Traces to** | **Priority** |
|----|----|----|----|----|----|
| TR-01 | Data conversion | \[Invoices open on the cut-over date shall be loaded with their approval history.\] | \[Reconciliation of counts and values before go-live.\] | \[BR-01\] | High |
| TR-02 | Training | \[All AP clerks and approvers shall complete training before go-live.\] | \[Training records show 100% completion.\] | \[SR-01, SR-02\] | High |
| TR-03 | Parallel running | \[Old and new processes shall run side by side for \[2\] payment cycles.\] | \[Daily reconciliation shows no differences.\] | \[BR-01\] | Medium |

# 9. Assumptions and constraints

> *Guidance: an assumption is believed to be true but not confirmed; a constraint limits the options for the solution. BABOK distinguishes business constraints (such as budget, time and policy) from technical constraints (such as platforms and standards).*

| **ID** | **Type** | **Description** | **Owner** | **Impact if wrong or binding** |
|----|----|----|----|----|
| A-01 | Assumption | \[At least 85% of invoices arrive as machine-readable PDFs.\] | \[AP manager\] | \[More manual exceptions\] |
| C-01 | Business constraint | \[Go-live by \[date\] within a budget of \[amount\].\] | \[Sponsor\] | \[Scope may need to be reduced\] |
| C-02 | Technical constraint | \[The ERP's core code cannot be changed; integration only through its APIs.\] | \[IT\] | \[Some functions must sit outside the ERP\] |

# 10. Verification

> *Guidance: verification checks that requirements are of good enough quality to be used (BABOK task 7.2). Check each requirement against the nine characteristics, and record the reviews held.*

## 10.1 Quality characteristics

☐ **Atomic:** self-contained and understandable on its own.

☐ **Complete:** enough detail to move forward.

☐ **Consistent:** aligned with the stakeholders' needs and with the other requirements.

☐ **Concise:** no extraneous content.

☐ **Feasible:** reasonable and possible within the agreed risk, schedule and budget.

☐ **Unambiguous:** understood the same way by everyone.

☐ **Testable:** it can be verified that the requirement has been met.

☐ **Prioritized:** ranked, grouped or negotiated in relation to the other requirements.

☐ **Understandable:** uses terms the audience understands, with the glossary.

## 10.2 Verification activities

☐ Models use their notation correctly and are complete within themselves.

☐ Related models agree with each other (for example, the data model and the data dictionary).

☐ Terms are used consistently and are in the glossary.

☐ Examples are added where they make a requirement clearer.

## 10.3 Review record

| **Review** | **Date** | **Participants** | **Findings** | **Status** |
|----|----|----|----|----|
| \[Peer review of sections 4 and 5\] | \[YYYY-MM-DD\] | \[BA, QA lead, solution architect\] | \[8 findings; 6 fixed, 2 open as ITM-01 and ITM-02\] | \[Closed\] |

# 11. Validation

> *Guidance: validation confirms that the requirements deliver value toward the business objectives (BABOK task 7.3). For each group of requirements, state the benefit it supports, how that benefit will be measured, and any assumptions behind it.*

| **Requirements** | **Business requirement (BRD)** | **Expected benefit** | **Evaluation criteria and measure** | **Assumption** | **Validated by** |
|----|----|----|----|----|----|
| \[FR-CAP-01 to FR-CAP-04\] | \[BR-01\] | \[Less manual keying; faster matching\] | \[Average days from receipt to approval: 9 → 3\] | \[A-01\] | \[Finance controller, YYYY-MM-DD\] |
| \[FR-APR-01 to FR-APR-03\] | \[BR-01, BR-02\] | \[Faster approvals; more discounts captured\] | \[Discount capture rate: 35% → 80%\] | \[—\] | \[Finance controller, YYYY-MM-DD\] |
| \[IF-04\] | \[BR-03\] | \[Fewer supplier queries\] | \[Queries a month: 400 → 200\] | \[—\] | \[AP manager, YYYY-MM-DD\] |

# 12. Traceability

> *Guidance: BABOK (task 5.1) recognizes four kinds of relationship. Derive: a requirement is derived from another. Depends: one requirement depends on another, either by necessity or because implementing one first makes the other easier. Satisfy: a design or solution component satisfies a requirement. Validate: a test case or other check validates that a requirement is met.*

| **Business requirement** | **Stakeholder requirement (derive)** | **Solution requirements (derive)** | **Depends on** | **Designs (satisfy)** | **Test cases (validate)** |
|----|----|----|----|----|----|
| \[BR-01\] | \[SR-01\] | \[FR-CAP-01 to FR-CAP-04, NFR-SCL-01\] | \[IF-01\] | \[Capture service design\] | \[TC-CAP-01 to TC-CAP-12\] |
| \[BR-01, BR-02\] | \[SR-02\] | \[FR-APR-01 to FR-APR-03, NFR-PRF-01, NFR-USB-01\] | \[FR-CAP-03\] | \[Wireframes; workflow design\] | \[TC-APR-01 to TC-APR-15\] |
| \[BR-03\] | \[SR-03\] | \[IF-04\] | \[FR-APR-02\] | \[Notification design\] | \[TC-SUP-01 to TC-SUP-05\] |

# 13. Prioritization

> *Guidance: record how priorities were set (BABOK task 5.3). State the approach, the factors considered, and who agreed the result.*

- **Approach:** \[Grouping into High, Medium and Low\]

- **Meaning:** \[High: the solution cannot go live without it. Medium: needed in this release but can follow shortly after go-live if necessary. Low: desirable; first to be deferred.\]

- **Basis considered:** \[benefit, penalty for not implementing, cost, risk, dependencies, time sensitivity, stability, regulatory or policy compliance\]

- **Agreed by:** \[Sponsor and product owner, YYYY-MM-DD\]

| **Priority** | **Number of requirements** | **Share** |
|--------------|----------------------------|-----------|
| High         | \[n\]                      | \[n%\]    |
| Medium       | \[n\]                      | \[n%\]    |
| Low          | \[n\]                      | \[n%\]    |

# 14. Change control

> *Guidance: after approval, assess every proposed change for its impact before deciding (BABOK tasks 5.2 and 5.4), and record the outcome here.*

| **Change ID** | **Date** | **Requirements affected** | **Change requested** | **Impact (benefit, cost, time, risk)** | **Decision** | **Decided by** |
|----|----|----|----|----|----|----|
| \[CR-01\] | \[YYYY-MM-DD\] | \[FR-APR-03\] | \[Escalate after 72 hours instead of 96\] | \[Low cost; faster approvals\] | \[Approved\] | \[Sponsor\] |

# 15. Open items

> *Guidance: track issues, questions, risks and decisions until they are resolved (BABOK technique 10.26).*

| **ID** | **Type** | **Description** | **Owner** | **Due** | **Status** |
|----|----|----|----|----|----|
| ITM-01 | \[Question\] | \[Will internal audit accept a ±2% matching tolerance (BRL-04)?\] | \[Finance controller\] | \[YYYY-MM-DD\] | \[Open\] |
| ITM-02 | \[Risk\] | \[Scanned invoices may extract poorly (FR-CAP-02).\] | \[AP manager\] | \[YYYY-MM-DD\] | \[Open\] |

# 16. Glossary

| **Term** | **Definition** |
|----|----|
| **Acceptance criteria** | Conditions a requirement must meet to be accepted |
| **Business requirement** | A goal, objective or outcome of the organization; the reason for the change |
| **Design** | A usable representation of a solution, such as a wireframe or data structure |
| **Functional requirement** | A capability the solution must have |
| **Non-functional requirement** | A condition or quality under which the solution must remain effective |
| **Solution requirement** | A capability or quality of the solution; either functional or non-functional |
| **Stakeholder requirement** | A need of a stakeholder or group of stakeholders |
| **Transition requirement** | A capability or condition needed only to move from the current state to the future state |
| **\[Three-way match\]** | \[Checking an invoice against its PO and goods receipt\] |
| **\[Term\]** | \[Definition\] |

# 17. Approval

> *Guidance: record who approved the requirements and when (BABOK task 5.5). Approval confirms the requirements are agreed and can be used for design, build and test.*

By approving, stakeholders agree that version \[x.y\] of this FRD states the solution requirements correctly and completely enough to proceed. Changes after approval follow section 14.

| **Name** | **Role** | **Decision** | **Signature** | **Date** |
|----|----|----|----|----|
| \[Name\] | Sponsor | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Domain subject matter expert | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Implementation subject matter expert | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Tester | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |

References: [A Guide to the Business Analysis Body of Knowledge (BABOK Guide) v3, IIBA](https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/) · [IIBA task cards: Requirements Analysis and Design Definition](https://www.iiba.org/contentassets/134acd0f148b4c51a7225c72bd17db0a/all-task-cards-req-analysis-and-design-def.pdf)
