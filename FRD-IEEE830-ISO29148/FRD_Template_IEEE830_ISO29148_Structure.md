# Functional Requirements Document (FRD)

**\[Project name\] · \[System name\]**

Template following the ISO/IEC/IEEE 29148:2018 software requirements specification outline (successor to IEEE 830-1998) · Version \[0.1\] · \[YYYY-MM-DD\]

**Contents**

- [How to use this template](#how-to-use-this-template)
- [Document control](#document-control)
- [1. Introduction](#1-introduction)
- [2. References](#2-references)
- [3. Specific requirements](#3-specific-requirements)
- [4. Verification](#4-verification)
- [5. Appendices](#5-appendices)

# How to use this template

Make one copy per software product or release. Replace every \[bracketed placeholder\], then delete this section, the *Guidance* notes and the example rows before the first review.

- **Structure:** sections 1 to 5 follow the example software requirements specification (SRS) outline in ISO/IEC/IEEE 29148:2018, which replaced IEEE 830-1998. Topics that IEEE 830 lists separately, such as the product perspective's interface aspects, apportioning of requirements, standards compliance and the five software system attributes, sit in the matching 29148 sections. The table at the end of this section maps every section to IEEE 830.

- **Front matter:** the document control section below holds the identification, change history and approvals that 29148 expects at the front of every requirements document.

- **Example rows** use one running example, an invoice approval system, so you can see how a requirement is written, ranked and verified. Replace them with your own.

## Requirement attributes

Give every requirement in section 3 these attributes:

| **Attribute** | **What to record** |
|----|----|
| Identifier | A unique ID that never changes or gets reused, such as \[FUN-CAP-01\] |
| Statement | One "shall" sentence (see below) |
| Rationale | Why the requirement exists |
| Source | Where it came from: a stakeholder, a higher-level requirement or a regulation |
| Priority | Essential, Conditional or Optional (see below) |
| Verification method | Inspection, Analysis, Demonstration or Test (section 4) |

Teams can add owner, risk, difficulty, stability and status as further columns if they track them.

## Writing a requirement

Build each requirement from up to five parts: a **condition**, the **subject**, an **action**, an **object**, and a **constraint** on the action. Use "shall" for mandatory requirements and do not combine two requirements in one sentence.

**Example:** When an invoice passes matching *(condition)*, the system *(subject)* shall route *(action)* the invoice to its approvers *(object)* within 2 minutes *(constraint)*.

Avoid language that cannot be verified:

| **Avoid** | **Examples** |
|----|----|
| Superlatives | best, most |
| Subjective words | user-friendly, easy to use, cost-effective |
| Vague pronouns | it, this, that, without a clear noun |
| Imprecise adjectives and adverbs | almost always, significant, minimal |
| Open-ended terms | but not limited to, as a minimum, provide support for |
| Comparisons | better than, higher quality |
| Loopholes | if possible, as appropriate, as applicable |
| Negative capability statements | the system shall not provide X (state what it shall do instead) |

## Priority

Rank each requirement as IEEE 830 recommends:

| **Rank** | **Meaning** |
|----|----|
| Essential | The software is not acceptable without it |
| Conditional | Adds value; its absence does not make the software unacceptable |
| Optional | May be worth having; to be decided during design |

## Quality characteristics

Check every requirement against the ISO/IEC/IEEE 29148 characteristics before review:

| **Applies to** | **Characteristics** |
|----|----|
| Each requirement | Necessary, appropriate, unambiguous, complete, singular, feasible, verifiable, correct, conforming |
| The set of requirements | Complete, consistent, feasible, comprehensible, able to be validated |
| The whole SRS (IEEE 830) | Correct, unambiguous, complete, consistent, ranked for importance or stability, verifiable, modifiable, traceable |

## Mapping to IEEE 830-1998

| **This template (ISO/IEC/IEEE 29148:2018)** | **IEEE 830-1998** |
|----|----|
| 1.1 Purpose | 1.1 Purpose |
| 1.2 Scope | 1.2 Scope |
| 1.3.1 Product perspective (including its interface aspects) | 2.1 Product perspective (2.1.1 to 2.1.8) |
| 1.3.2 Product functions | 2.2 Product functions |
| 1.3.3 User characteristics | 2.3 User characteristics |
| 1.3.4 Limitations | 2.4 Constraints |
| 1.3.5 Apportioning of requirements | 2.6 Apportioning of requirements |
| 1.4 Definitions; 5.2 Acronyms and abbreviations | 1.3 Definitions, acronyms and abbreviations |
| 2 References | 1.4 References |
| 3.1 Functions | 3.2 Functions; 3.7 Organizing the specific requirements |
| 3.2 Performance requirements | 3.3 Performance requirements |
| 3.3 Usability requirements | (no 830 equivalent) |
| 3.4 Interface requirements | 3.1 External interfaces |
| 3.5 Logical database requirements | 3.4 Logical database requirements |
| 3.6 Design constraints, including 3.6.1 Standards compliance | 3.5 Design constraints; 3.5.1 Standards compliance |
| 3.7 Software system attributes | 3.6 Software system attributes |
| 3.8 Supporting information | 3.8 Additional comments; appendixes |
| 4 Verification | (no 830 equivalent) |
| 5.1 Assumptions and dependencies | 2.5 Assumptions and dependencies |

> *Guidance: section names follow the SRS outline in the 2018 edition of ISO/IEC/IEEE 29148. A third edition is in development; check its outline if you need conformance to the newer edition.*

# Document control

| **Field** | **Value** |
|----|----|
| **Document title** | Functional Requirements Document (Software Requirements Specification) for \[System name\] |
| **Document ID** | \[FRD-2026-001\] |
| **Project** | \[Project name\] |
| **Release** | \[Release 1\] |
| **Related documents** | \[BRD or stakeholder requirements specification, ID and version\] |
| **Author** | \[Name, role\] |
| **Current version** | \[0.1\] |
| **Status** | \[Draft / Under review / Approved\] |
| **Date** | \[YYYY-MM-DD\] |

## Change history

| **Version** | **Date**       | **Author** | **Summary of changes**   |
|-------------|----------------|------------|--------------------------|
| 0.1         | \[YYYY-MM-DD\] | \[Name\]   | Initial draft            |
| \[0.2\]     | \[YYYY-MM-DD\] | \[Name\]   | \[Changes after review\] |

## Approvals

| **Name** | **Role** | **Decision** | **Signature** | **Date** |
|----|----|----|----|----|
| \[Name\] | Product owner or customer representative | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Solution architect or development lead | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Test lead | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |

# 1. Introduction

## 1.1 Purpose

> *Guidance: state what this document specifies and who it is for.*

\[This document specifies the software requirements for Release 1 of the \[Invoice Automation System\]. It is written for the development and test teams, the solution architect, and the business owners who approve it.\]

## 1.2 Scope

> *Guidance: name the software product, say what it will and will not do, and state the benefits and objectives it supports. Keep this consistent with higher-level documents such as the BRD.*

- **Software product:** \[Invoice Automation System, Release 1\]

- **What it will do:** \[capture supplier invoices from email, extract and match their data, route them for approval, and send approved invoices to the ERP\]

- **What it will not do:** \[execute payments, which remain in the ERP; handle expense claims\]

- **Objectives supported:** \[reduce invoice approval time from 9 to 3 days; see BRD-2026-014, BR-01\]

## 1.3 Product overview

### 1.3.1 Product perspective

> *Guidance: say whether the product is new, a replacement or part of a larger system, and attach a context diagram that shows the users and the systems it connects to. Then describe each aspect below, or write "None".*

\[The Invoice Automation System is a new product that replaces manual keying and email approvals. It sits between the AP mailbox, the ERP and the approvers.\]

Context diagram: \[link or attachment\]

| **Aspect** | **Description** |
|----|----|
| System interfaces | \[ERP (purchase orders, goods receipts, approved invoices); AP mailbox\] |
| User interfaces | \[Web screens for AP clerks and finance controllers; mobile web for approvers\] |
| Hardware interfaces | \[None\] |
| Software interfaces | \[ERP REST API version \[x\]; corporate identity provider\] |
| Communications interfaces | \[HTTPS; email (SMTP); notification service API\] |
| Memory constraints | \[None beyond the hosting platform's limits\] |
| Operations | \[Unattended invoice capture 24 × 7; approvals during business hours; nightly archive job\] |
| Site adaptation requirements | \[Approval thresholds and cost-centre routing configured for each legal entity\] |

### 1.3.2 Product functions

> *Guidance: summarise the major functions in a few lines each; the detail goes in section 3.1.*

| **Function** | **Summary** |
|----|----|
| \[Invoice capture (CAP)\] | \[Receive invoices, extract data, match to PO and goods receipt\] |
| \[Approval workflow (APR)\] | \[Route, approve, reject, remind and escalate\] |
| \[Supplier status (SUP)\] | \[Let suppliers check invoice status\] |

### 1.3.3 User characteristics

> *Guidance: describe each group of users, including anything that affects usability, such as education, experience, disabilities and technical skill.*

| **User group** | **Number** | **Frequency of use** | **Characteristics** |
|----|----|----|----|
| \[AP clerk\] | \[12\] | \[Daily, full time\] | \[Expert ERP users\] |
| \[Approver\] | \[180\] | \[Weekly, mostly on a phone\] | \[Occasional users; no training\] |
| \[Supplier user\] | \[1,500\] | \[Monthly\] | \[External; varied skills and languages\] |

### 1.3.4 Limitations

> *Guidance: list anything that limits the developers' options: regulations, hardware limits, interfaces to other applications, parallel operation, audit functions, control functions, required languages, handshake protocols, quality requirements such as reliability, criticality of the application, and safety and security considerations.*

| **ID** | **Limitation** | **Source** |
|----|----|----|
| LIM-01 | \[Payments must remain in the ERP; the ERP's core code cannot be changed.\] | \[IT policy\] |
| LIM-02 | \[Invoice and approval records must be kept for \[n\] years.\] | \[Tax law\] |
| LIM-03 | \[Internal users must sign in through the corporate identity provider.\] | \[Security policy\] |

### 1.3.5 Apportioning of requirements

> *Guidance: list requirements that are deferred to a later release, or allocated to another system or a manual process.*

| **Requirement** | **Deferred or allocated to** | **Reason** |
|----|----|----|
| \[Non-PO invoices\] | \[Release 2\] | \[Needs a separate approval matrix\] |

## 1.4 Definitions

> *Guidance: define every term a reader might misunderstand. Put acronyms and abbreviations in section 5.2.*

| **Term** | **Definition** |
|----|----|
| **\[Three-way match\]** | \[Checking an invoice against its purchase order and goods receipt\] |
| **\[Approver\]** | \[A cost-centre owner authorised to approve invoices for that cost centre\] |

# 2. References

> *Guidance: list every document this SRS refers to, with enough detail for a reader to find the right version.*

| **ID** | **Document** | **Version** | **Date** | **Location** |
|----|----|----|----|----|
| \[REF-01\] | \[Business Requirements Document, BRD-2026-014\] | \[1.0\] | \[YYYY-MM-DD\] | \[Link\] |
| \[REF-02\] | \[Delegation of authority policy\] | \[2025\] | \[YYYY-MM-DD\] | \[Link\] |
| \[REF-03\] | \[UI style guide\] | \[2.1\] | \[YYYY-MM-DD\] | \[Link\] |

# 3. Specific requirements

> *Guidance: state every requirement in enough detail for designers to build the software and testers to verify it. Give each the attributes listed at the start of this template. IEEE 830 lets you organize section 3.1 by system mode, user class, object, feature, stimulus, response or functional hierarchy; choose one and use it consistently. This template organizes functions by feature.*

## 3.1 Functions

> *Guidance: for each function, cover input validation, the sequence of operations, responses to abnormal situations (such as overflow, communication failure and errors), and how outputs relate to inputs. Abnormal situations are where specifications are most often incomplete.*

### 3.1.1 \[Feature CAP: Invoice capture\]

\[Brief description of the feature and the stakeholders it serves.\]

| **ID** | **Requirement** | **Rationale** | **Source** | **Priority** | **Verification** |
|----|----|----|----|----|----|
| FUN-CAP-01 | \[When an email with a PDF attachment arrives in the AP mailbox, the system shall create an invoice record within 60 seconds.\] | \[Removes manual keying\] | \[BRD BR-01\] | Essential | Test |
| FUN-CAP-02 | \[The system shall extract the supplier name, invoice number, invoice date, amount, tax amount and PO number from each invoice.\] | \[Data needed for matching and approval\] | \[BRD BR-01\] | Essential | Test |
| FUN-CAP-03 | \[If an attachment cannot be read, the system shall reply to the sender with the reason within 5 minutes.\] | \[Suppliers learn of problems at once\] | \[AP manager\] | Essential | Test |
| FUN-CAP-04 | \[If the same supplier has already submitted an invoice with the same number, the system shall hold the new invoice for review.\] | \[Prevents duplicate payment\] | \[Internal audit\] | Essential | Test |

### 3.1.2 \[Feature APR: Approval workflow\]

\[Brief description of the feature and the stakeholders it serves.\]

| **ID** | **Requirement** | **Rationale** | **Source** | **Priority** | **Verification** |
|----|----|----|----|----|----|
| FUN-APR-01 | \[When an invoice passes matching, the system shall route it to its approvers within 2 minutes.\] | \[Approval speed drives the objective\] | \[BRD BR-01\] | Essential | Test |
| FUN-APR-02 | \[The system shall record each approval or rejection with the user, time and reason.\] | \[Audit trail\] | \[LIM-02\] | Essential | Inspection |
| FUN-APR-03 | \[The system shall let an approver delegate approvals to a named colleague for a date range.\] | \[Covers leave\] | \[Finance controller\] | Optional | Demonstration |

> *Guidance: repeat for every feature listed in section 1.3.2.*

## 3.2 Performance requirements

> *Guidance: state static requirements (such as number of users and volume of data) and dynamic requirements (such as transactions and response times) as measurable numbers, with the conditions under which they apply.*

| **ID** | **Requirement** | **Type** | **Priority** | **Verification** |
|----|----|----|----|----|
| PRF-01 | \[The system shall support 200 concurrent users.\] | Static | Essential | Test |
| PRF-02 | \[The system shall process 5,000 invoices a day.\] | Dynamic | Essential | Test |
| PRF-03 | \[95% of screen responses shall complete within 2 seconds at the load in PRF-01 and PRF-02.\] | Dynamic | Essential | Test |

## 3.3 Usability requirements

> *Guidance: state measurable targets for effectiveness, efficiency and satisfaction for named users and tasks, and any accessibility standard that applies.*

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| USB-01 | \[At least 9 of 10 first-time approvers shall approve an invoice on a phone without help.\] | Essential | Test (usability test) |
| USB-02 | \[A first-time approver shall complete an approval in under 60 seconds.\] | Conditional | Test (usability test) |
| USB-03 | \[All screens shall conform to WCAG 2.2 Level AA.\] | Essential | Inspection |

## 3.4 Interface requirements

> *Guidance: for each interface, give its name, purpose, source or destination, data and format, valid ranges and units, timing, and what happens when it fails.*

### 3.4.1 User interfaces

| **ID** | **Screen** | **Purpose** | **Users** | **Requirements** | **Verification** |
|----|----|----|----|----|----|
| UIF-01 | \[Invoice detail and approval\] | \[View an invoice and decide\] | \[Approver\] | \[Shows the invoice image, extracted data and match result; works on screens 360 px wide and up\] | Demonstration |
| UIF-02 | \[AP work queue\] | \[Resolve exceptions\] | \[AP clerk\] | \[Lists exceptions by due date; allows correction with a reason\] | Demonstration |

### 3.4.2 Hardware interfaces

\[Describe each hardware interface, such as scanners or printers, or write "None".\]

### 3.4.3 Software interfaces

| **ID** | **Interface** | **Data** | **Direction** | **Format and protocol** | **Timing** | **On failure** | **Verification** |
|----|----|----|----|----|----|----|----|
| SWI-01 | \[ERP purchase orders\] | \[PO number, lines, values, requester\] | \[In\] | \[REST API, JSON\] | \[Every 15 minutes\] | \[Retry every 5 minutes; alert after 3 failures\] | Test |
| SWI-02 | \[ERP approved invoices\] | \[Invoice header and lines\] | \[Out\] | \[REST API, JSON\] | \[Within 5 minutes of approval\] | \[Queue and retry; alert after 3 failures\] | Test |

### 3.4.4 Communications interfaces

| **ID** | **Interface** | **Requirements** | **Verification** |
|----|----|----|----|
| COM-01 | \[Email\] | \[Outgoing mail from an authenticated domain (SPF, DKIM, DMARC)\] | Inspection |
| COM-02 | \[Web traffic\] | \[HTTPS with TLS 1.2 or higher only\] | Test |

## 3.5 Logical database requirements

> *Guidance: describe the types of information the software stores, how often each is used, who can access it, the entities and relationships, integrity constraints, and how long data is kept. Attach a data model.*

| **Entity** | **Description** | **Key attributes** | **Frequency of use** | **Retention** |
|----|----|----|----|----|
| \[Invoice\] | \[A supplier's request for payment\] | \[Invoice ID, supplier ID, number, amount, status\] | \[5,000 created a day; read constantly\] | \[\[n\] years (LIM-02)\] |
| \[Approval\] | \[One approver's decision\] | \[Approval ID, invoice ID, approver, decision, reason, time\] | \[8,000 a day\] | \[\[n\] years\] |

| **ID** | **Integrity rule** | **Verification** |
|----|----|----|
| DBR-01 | \[Invoice number shall be unique for each supplier.\] | Test |
| DBR-02 | \[Every rejected approval shall have a reason of at least 10 characters.\] | Test |

Data model: \[link or attachment\]

## 3.6 Design constraints

> *Guidance: state constraints on the design imposed by other standards, regulations, hardware, or the organization's own policies.*

| **ID** | **Constraint** | **Source** | **Verification** |
|----|----|----|----|
| DSC-01 | \[The software shall run on the organization's approved cloud platform in an in-country region.\] | \[IT policy\] | Inspection |
| DSC-02 | \[The software shall integrate with the ERP only through its published APIs.\] | \[LIM-01\] | Inspection |

### 3.6.1 Standards compliance

> *Guidance: state requirements that come from existing standards or regulations, such as report formats, data naming, accounting procedures and audit tracing.*

| **ID** | **Requirement** | **Standard or regulation** | **Verification** |
|----|----|----|----|
| STD-01 | \[Every change to invoice data shall be traceable to a user and time (audit trail).\] | \[Internal control policy\] | Inspection |
| STD-02 | \[Tax amounts shall be shown as required by \[applicable tax law\].\] | \[Tax law\] | Inspection |

## 3.7 Software system attributes

> *Guidance: state each attribute so it can be measured or checked. Write "Not applicable" with a reason rather than leaving an attribute out.*

### 3.7.1 Reliability

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| REL-01 | \[After a failure, no more than 15 minutes of data shall be lost.\] | Essential | Test |

### 3.7.2 Availability

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| AVL-01 | \[The approval function shall be available 99.5% of business hours each month.\] | Essential | Analysis |
| AVL-02 | \[After a failure, service shall be restored within 4 hours.\] | Essential | Test |

### 3.7.3 Security

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| SEC-01 | \[Internal users shall sign in through single sign-on with multi-factor authentication.\] | Essential | Test |
| SEC-02 | \[A supplier user shall see only their own company's invoices.\] | Essential | Test |
| SEC-03 | \[Personal data shall be encrypted at rest.\] | Essential | Inspection |

### 3.7.4 Maintainability

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| MNT-01 | \[Finance controllers shall change approval thresholds without a software release.\] | Conditional | Demonstration |

### 3.7.5 Portability

| **ID** | **Requirement** | **Priority** | **Verification** |
|----|----|----|----|
| PRT-01 | \[The user interface shall work on the latest two versions of Chrome, Edge and Safari.\] | Essential | Test |

## 3.8 Supporting information

> *Guidance: add material that helps readers understand the requirements: sample inputs and outputs, use cases or scenarios, background, and traceability to higher-level requirements.*

### 3.8.1 Traceability to higher-level requirements

| **Higher-level requirement** | **Requirements in this document** |
|----|----|
| \[BRD BR-01 (approval time)\] | \[FUN-CAP-01, FUN-CAP-02, FUN-APR-01, PRF-03\] |
| \[BRD BR-03 (supplier queries)\] | \[FUN-SUP-nn, SEC-02\] |

### 3.8.2 Sample inputs, outputs and scenarios

\[Attach sample invoices, sample ERP messages and key user scenarios, or link to them.\]

# 4. Verification

> *Guidance: this section mirrors section 3. For every requirement, state how it will be verified and what result counts as a pass. Use one of the four methods below.*

## 4.1 Verification methods

| **Method** | **Meaning** |
|----|----|
| Inspection | Examining documents, code, configuration, data or the user interface against the requirement |
| Analysis | Using calculation, models, simulation or sampled data |
| Demonstration | Operating the software to show a capability works, without detailed measurement |
| Test | Running the software with defined inputs and comparing results with expected outputs |

## 4.2 Verification matrix

| **Requirement** | **Method** | **Verification activity and pass criteria** | **Stage** | **Responsible** |
|----|----|----|----|----|
| FUN-CAP-01 | Test | \[Send 50 sample invoices; every record exists within 60 seconds\] | \[System test\] | \[Test lead\] |
| FUN-APR-02 | Inspection | \[Audit trail of 20 test decisions shows user, time and reason for each\] | \[System test\] | \[Test lead\] |
| PRF-03 | Test | \[Load test at PRF-01 and PRF-02 loads; 95th percentile response under 2 seconds\] | \[Performance test\] | \[Performance engineer\] |
| USB-01 | Test | \[Moderated test with 10 first-time approvers; at least 9 succeed unaided\] | \[Acceptance test\] | \[UX lead\] |
| AVL-01 | Analysis | \[Monitoring data for the first month after go-live\] | \[Operation\] | \[Service manager\] |
| \[ID\] | \[Method\] | \[Activity and pass criteria\] | \[Stage\] | \[Name\] |

# 5. Appendices

## 5.1 Assumptions and dependencies

> *Guidance: list factors that are assumed rather than known, and things the project depends on. If an assumption proves false, the requirements may need to change.*

| **ID** | **Type** | **Description** | **Owner** | **Impact if wrong or unmet** |
|----|----|----|----|----|
| ASM-01 | Assumption | \[At least 85% of invoices arrive as machine-readable PDFs.\] | \[AP manager\] | \[More manual exceptions\] |
| DEP-01 | Dependency | \[ERP purchase-order API available in the test environment by \[date\].\] | \[ERP team\] | \[Matching cannot be tested\] |

## 5.2 Acronyms and abbreviations

| **Acronym** | **Meaning**                           |
|-------------|---------------------------------------|
| AP          | Accounts payable                      |
| ERP         | Enterprise resource planning (system) |
| PO          | Purchase order                        |
| SRS         | Software requirements specification   |
| \[Acronym\] | \[Meaning\]                           |
