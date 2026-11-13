# Business Requirements Document (BRD)

**\[Project name\]**

Template aligned to the BABOK® Guide v3 · Version \[0.1\] · \[YYYY-MM-DD\]

# How to use this template

Make one copy per initiative. Replace every \[bracketed placeholder\], then delete the *Guidance* notes and example rows before the first review.

- **Example rows** follow one running example, automating accounts-payable invoice processing, so you can see how a requirement traces from section 6 through section 14.

- **One requirement per row.** Use "shall" for mandatory and "should" for desirable.

- **Priority** uses MoSCoW: Must, Should, Could, Won't (this release).

- **Status** moves Draft → Under review → Approved. Use Deferred or Rejected for items taken out of scope.

- **Agile projects:** keep every section, but hold the detailed functional requirements (section 8) as epics and user stories in the backlog, and list the story IDs in the traceability matrix.

Requirement types follow the BABOK v3 requirements classification schema (section 2.3):

| **Type** | **Question it answers** | **ID prefix** | **Section** |
|----|----|----|----|
| Business | Why is the organization making this change? | BR- | 6 |
| Stakeholder | What does each stakeholder group need? | SR- | 7 |
| Solution: functional | What must the solution do? | FR- | 8 |
| Solution: non-functional | How well, and under what conditions, must it work? | NFR- | 9 |
| Transition | What is needed only to move from the current to the future state? | TR- | 10 |

Other IDs: BRL- for business rules; A-, C- and D- for assumptions, constraints and dependencies; RSK- for risks; PP- for pain points.

Reference: [A Guide to the Business Analysis Body of Knowledge (BABOK Guide) v3, IIBA](https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/).

# Document control

| **Field**                             | **Value**                           |
|---------------------------------------|-------------------------------------|
| **Project name**                      | \[Project name\]                    |
| **Project ID**                        | \[ID\]                              |
| **Business sponsor**                  | \[Name, title\]                     |
| **Document owner (business analyst)** | \[Name\]                            |
| **Current version**                   | \[0.1\]                             |
| **Document status**                   | \[Draft / Under review / Approved\] |
| **Last updated**                      | \[YYYY-MM-DD\]                      |

## Version history

| **Version** | **Date**       | **Author** | **Summary of changes**               |
|-------------|----------------|------------|--------------------------------------|
| 0.1         | \[YYYY-MM-DD\] | \[Name\]   | Initial draft                        |
| \[0.2\]     | \[YYYY-MM-DD\] | \[Name\]   | \[Changes after stakeholder review\] |

## Reviewers and approvers

| **Name** | **Role**           | **Review or approve** | **Date reviewed** |
|----------|--------------------|-----------------------|-------------------|
| \[Name\] | Business sponsor   | Approve               | \[YYYY-MM-DD\]    |
| \[Name\] | Process owner      | Approve               | \[YYYY-MM-DD\]    |
| \[Name\] | IT / solution lead | Review                | \[YYYY-MM-DD\]    |
| \[Name\] | QA / test lead     | Review                | \[YYYY-MM-DD\]    |

# 1. Executive summary

> *Guidance: write this last, in 150–250 words, for a sponsor who reads nothing else. Cover the problem, the change proposed, the expected benefit with a number, what is in scope, the top risk and the decision you need.*

\[Organization\] takes \[9\] days on average to approve a supplier invoice, which costs \[amount\] a year in late-payment penalties and missed early-payment discounts. This BRD sets out the requirements for \[an automated invoice capture and approval process\] covering \[all PO-backed supplier invoices\]. The change targets \[a 3-day approval cycle and 80% discount capture\] by \[date\]. The main risk is \[extraction accuracy on scanned invoices\], mitigated by \[a vendor accuracy test before contract\]. **Decision requested:** approve these requirements so that \[solution selection\] can begin by \[date\].

# 2. Business need

> *Guidance: BABOK task 6.1 (Analyze Current State) starts here. State the need in business terms, never as a solution.*

## 2.1 Problem or opportunity statement

|  |  |
|----|----|
| **The problem of** | \[Slow, manual invoice approval\] |
| **affects** | \[AP clerks, approving managers and suppliers\] |
| **the impact of which is** | \[Average approval time of 9 days, \[amount\]/year in late fees, 35% of early-payment discounts captured\] |
| **a successful solution would** | \[Approve invoices in 3 days and capture most available discounts\] |

## 2.2 Strategic alignment

\[Which corporate goal, OKR or strategic theme this supports, with a link to it.\]

## 2.3 Cost of doing nothing

\[What happens over the next 12–24 months if no change is made, in money, risk or customer impact.\]

## 2.4 Business case

\[Link to the approved business case or investment request, if separate.\]

# 3. Current state (as-is)

> *Guidance: describe how the work is done today, with evidence. Attach the as-is process map (BPMN 2.0 recommended).*

## 3.1 Process overview

1.  \[Supplier emails a PDF invoice to the AP mailbox.\]

2.  \[AP clerk keys invoice data into the ERP by hand.\]

3.  \[Clerk emails the invoice to the cost-centre owner for approval.\]

4.  \[Approver replies by email; clerk updates the ERP.\]

5.  \[Payment run picks up approved invoices weekly.\]

As-is process map: \[link or attachment\]

## 3.2 Pain points

| **ID** | **Pain point** | **Who is affected** | **Evidence** |
|----|----|----|----|
| PP-01 | \[Manual keying causes data-entry errors\] | AP clerks | \[4% of invoices corrected after entry, Q2 audit\] |
| PP-02 | \[Approval requests get lost in email\] | Approvers, suppliers | \[Average 6 of the 9 days spent waiting for approval\] |
| PP-03 | \[Suppliers cannot see payment status\] | Suppliers, AP team | \[About 400 status calls and emails a month\] |

## 3.3 Systems and data in use

| **System** | **Purpose** | **Owner** | **Notes** |
|----|----|----|----|
| \[ERP name\] | Ledger, POs, payments | \[Finance IT\] | \[Version, integration options\] |
| \[Shared mailbox\] | Invoice intake | \[AP team\] | \[Volume per month\] |

# 4. Scope

> *Guidance: an explicit out-of-scope list prevents more disputes than any other section.*

## 4.1 In scope

- \[Capture of PO-backed supplier invoices received by email or supplier portal\]

- \[Approval routing and approval on mobile and desktop\]

- \[Supplier view of invoice and payment status\]

## 4.2 Out of scope

- \[Non-PO invoices and employee expense claims — planned for phase 2\]

- \[Replacement of the ERP\]

- \[Changes to payment-run frequency\]

## 4.3 Affected areas

| **Area** | **Included** |
|----|----|
| **Business units** | \[Finance shared services, all cost centres that approve invoices\] |
| **Locations** | \[All entities in country X\] |
| **Systems** | \[ERP, AP mailbox, new capture tool\] |
| **External parties** | \[Suppliers\] |

# 5. Stakeholders

> *Guidance: BABOK lists common stakeholder roles: customer, domain subject matter expert, end user, implementation subject matter expert, operational support, project manager, regulator, sponsor, supplier and tester. Mark who is Responsible, Accountable, Consulted or Informed for this BRD.*

| **Stakeholder or group** | **BABOK role** | **Main interest** | **Influence** | **RACI** |
|----|----|----|----|----|
| \[CFO\] | Sponsor | Lower cost, fewer late fees | High | A |
| \[AP manager\] | Domain SME | Workload, accuracy | High | R |
| \[AP clerks\] | End user | Less manual keying | Medium | C |
| \[Cost-centre managers\] | End user | Fast, simple approval | Medium | C |
| \[Suppliers\] | Customer | Paid on time, visible status | Low | I |
| \[Finance IT\] | Implementation SME | ERP integration, support | Medium | C |
| \[Internal audit\] | Regulator | Controls, audit trail | Medium | C |
| \[QA lead\] | Tester | Testable requirements | Low | C |

# 6. Business requirements

Business requirements state the goals, objectives and outcomes that justify the change. Each one needs a measure, a baseline and a target.

| **ID** | **Requirement** | **Measure: baseline → target** | **Source** | **Priority** | **Status** |
|----|----|----|----|----|----|
| BR-01 | The organization shall reduce average invoice approval time by \[date\]. | Days from receipt to approval: \[9 → 3\] | \[CFO\] | Must | Draft |
| BR-02 | The organization shall capture early-payment discounts on eligible invoices. | Discount capture rate: \[35% → 80%\] | \[Finance director\] | Should | Draft |
| BR-03 | The organization shall reduce supplier payment-status queries to AP. | Queries a month: \[400 → 200\] | \[AP manager\] | Could | Draft |

# 7. Stakeholder requirements

Stakeholder requirements state what a particular group needs from the solution. Each one traces back to a business requirement.

| **ID** | **Stakeholder group** | **Requirement** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| SR-01 | AP clerks | AP clerks need to see every invoice awaiting their action in a single work queue. | BR-01 | Must | Draft |
| SR-02 | Approving managers | Approvers need to approve or reject invoices from a phone without logging into the ERP. | BR-01, BR-02 | Must | Draft |
| SR-03 | Suppliers | Suppliers need to check the status of their invoices without contacting AP. | BR-03 | Could | Draft |

# 8. Functional requirements

Functional requirements describe what the solution must do. Write acceptance criteria that a tester could run without asking you what you meant.

| **ID** | **Requirement** | **Acceptance criteria** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| FR-01 | The system shall extract supplier name, invoice number, invoice date, amount and PO number from PDF invoices received in the AP mailbox. | On the agreed test set of \[200\] invoices, at least \[95%\] of fields are extracted correctly. | SR-01 | Must | Draft |
| FR-02 | The system shall route each invoice to the approver set for its cost centre and amount band (see BRL-01). | Given an invoice for cost centre X above \[threshold\], it reaches both the cost-centre owner and the finance controller. | SR-02 | Must | Draft |
| FR-03 | The system shall let approvers approve or reject an invoice from a mobile browser, with a mandatory reason on rejection. | Rejection cannot be submitted without a reason; the decision appears in the ERP within \[5\] minutes. | SR-02 | Must | Draft |
| FR-04 | The system shall show suppliers the status and expected payment date of each invoice they submitted. | A supplier sees only their own invoices; status matches the ERP. | SR-03 | Could | Draft |

# 9. Non-functional requirements

Non-functional requirements set the qualities and conditions the solution must meet. Give each one a number someone can test.

| **ID** | **Category** | **Requirement** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| NFR-01 | Performance | Data extraction shall finish within \[60\] seconds of an invoice's arrival for \[95%\] of invoices. | FR-01 | Must | Draft |
| NFR-02 | Availability | The approval function shall be available \[99.5%\] of the time during \[business hours, time zone\]. | FR-03 | Should | Draft |
| NFR-03 | Security | Users shall sign in through \[single sign-on\], and suppliers shall see only their own data. | FR-03, FR-04 | Must | Draft |
| NFR-04 | Audit and compliance | Every approval, rejection and data change shall be logged with user, time and old and new values, and kept for \[n\] years as required by \[applicable law\]. | FR-02, FR-03 | Must | Draft |
| NFR-05 | Usability | A new approver shall be able to approve an invoice without training, measured in \[5\] observed sessions. | FR-03 | Should | Draft |

# 10. Transition requirements

Transition requirements cover what is needed only to move from the current state to the future state. They stop applying once the change is complete.

| **ID** | **Category** | **Requirement** | **Traces to** | **Priority** | **Status** |
|----|----|----|----|----|----|
| TR-01 | Data migration | Invoices open in the old process on the cut-over date shall be loaded into the new system with their approval history. | BR-01 | Must | Draft |
| TR-02 | Training | All AP clerks and approvers shall complete \[30-minute\] training before go-live. | SR-01, SR-02 | Must | Draft |
| TR-03 | Parallel run | The old and new processes shall run side by side for \[2\] payment cycles, with a daily reconciliation. | BR-01 | Should | Draft |
| TR-04 | Supplier communication | Suppliers shall be told the new invoice address and portal link \[4\] weeks before go-live. | SR-03 | Should | Draft |

# 11. Future state (to-be) and business rules

> *Guidance: BABOK task 6.2 (Define Future State). Attach the to-be process map and reference requirement IDs at each step.*

## 11.1 Future-state process

1.  Supplier emails the invoice or uploads it through the portal.

2.  The system extracts the invoice data and matches it to the PO (FR-01).

3.  Invoices that fail the match go to the AP clerk's work queue (SR-01).

4.  The system routes matched invoices to the right approvers (FR-02, BRL-01).

5.  The approver approves or rejects from any device (FR-03).

6.  Approved invoices are scheduled for payment, discount-eligible ones first (BR-02, BRL-02).

To-be process map: \[link or attachment\]

## 11.2 Business rules

> *Guidance: BABOK separates definitional rules (what something is) from behavioural rules (what people or systems must or must not do).*

| **ID** | **Rule** | **Type** | **Source** | **Owner** |
|----|----|----|----|----|
| BRL-01 | Invoices above \[threshold amount\] need approval from the finance controller as well as the cost-centre owner. | Behavioural | \[Delegation of authority policy\] | \[Finance controller\] |
| BRL-02 | An invoice is discount-eligible when the supplier's terms offer a discount for payment within a stated number of days. | Definitional | \[Supplier contract terms\] | \[Procurement\] |
| BRL-03 | A rejected invoice shall be returned to the supplier with the reason within \[2\] business days. | Behavioural | \[AP policy\] | \[AP manager\] |

# 12. Assumptions, constraints and dependencies

> *Guidance: an assumption is believed true but not confirmed; a constraint limits the options; a dependency is something outside the project that must happen first.*

| **ID** | **Type** | **Description** | **Owner** | **Impact if wrong or unmet** |
|----|----|----|----|----|
| A-01 | Assumption | \[Suppliers will accept sending invoices to a single AP address.\] | \[AP manager\] | \[Intake volume through old channels stays high.\] |
| A-02 | Assumption | \[At least 85% of invoices arrive as machine-readable PDFs.\] | \[AP manager\] | \[More manual exceptions; BR-01 at risk.\] |
| C-01 | Constraint | \[The solution must integrate with the existing ERP; no ERP replacement in this phase.\] | \[Finance IT\] | — |
| C-02 | Constraint | \[Budget capped at \[amount\]; go-live by \[date\].\] | \[Sponsor\] | — |
| D-01 | Dependency | \[IT security review must be complete before the supplier portal goes live.\] | \[IT security\] | \[Portal launch slips; FR-04 delayed.\] |

# 13. Risks

> *Guidance: BABOK task 6.3 (Assess Risks). Rate likelihood and impact High, Medium or Low, and name one owner per risk.*

| **ID** | **Risk** | **Likelihood** | **Impact** | **Mitigation** | **Owner** |
|----|----|----|----|----|----|
| RSK-01 | \[Extraction accuracy falls below target on scanned or handwritten invoices.\] | Medium | High | \[Test vendors on 200 sample invoices before contract; keep a manual exception queue.\] | \[AP manager\] |
| RSK-02 | \[Approvers keep using email instead of the new tool.\] | Medium | High | \[Mobile approval, automatic reminders, escalation after 48 hours.\] | \[Sponsor\] |
| RSK-03 | \[Errors in migrated open invoices.\] | Low | Medium | \[Two trial migrations with reconciliation before cut-over.\] | \[Finance IT\] |

# 14. Requirements traceability matrix

> *Guidance: BABOK task 5.1 (Trace Requirements). Every business requirement should trace forward to stakeholder, solution and test items. A solution requirement that traces to no business requirement is a scope question.*

| **Business req.** | **Stakeholder req.** | **Functional / non-functional** | **Transition** | **Design ref.** | **Test cases** | **Status** |
|----|----|----|----|----|----|----|
| BR-01 | SR-01, SR-02 | FR-01, FR-02, FR-03, NFR-01, NFR-02, NFR-04 | TR-01, TR-02, TR-03 | \[Design doc §\] | \[TC-01 to TC-12\] | Draft |
| BR-02 | SR-02 | FR-02, FR-03 | TR-02 | \[Design doc §\] | \[TC-13 to TC-16\] | Draft |
| BR-03 | SR-03 | FR-04, NFR-03 | TR-04 | \[Design doc §\] | \[TC-17 to TC-20\] | Draft |

# 15. Requirements quality checklist

Before review, check every requirement against BABOK's nine characteristics of quality requirements (task 7.2, Verify Requirements).

☐ **Atomic:** it states one thing and cannot be split further.

☐ **Complete:** nothing a reader needs to act on it is missing.

☐ **Consistent:** it does not conflict with any other requirement.

☐ **Concise:** it contains no extra words or explanation.

☐ **Feasible:** it can be met within known budget, time and technology.

☐ **Unambiguous:** two readers would interpret it the same way.

☐ **Testable:** a tester can prove it has been met.

☐ **Prioritized:** it has a MoSCoW priority.

☐ **Understandable:** its intended readers understand every term.

Document-level checks:

☐ Every requirement has an ID, a source, a priority and a status.

☐ Every business requirement traces forward in section 14.

☐ Every term a non-specialist might not know is in the glossary.

☐ Open questions are closed or assigned an owner and a date.

# 16. Glossary

| **Term** | **Definition** |
|----|----|
| **BRD** | Business Requirements Document: this document. |
| **Business requirement** | A goal, objective or outcome the organization needs, stating why the change is made. |
| **Stakeholder requirement** | A need of a particular stakeholder group, linking business and solution requirements. |
| **Solution requirement** | A capability (functional) or quality (non-functional) the solution must have. |
| **Transition requirement** | A temporary need for moving from the current to the future state, such as data migration or training. |
| **MoSCoW** | Prioritization scheme: Must have, Should have, Could have, Won't have this time. |
| **Traceability** | The links from each requirement back to its source and forward to design and tests. |
| **\[PO\]** | \[Purchase order: the buyer's approved order that an invoice is matched against.\] |

# 17. Sign-off

By signing, approvers confirm that version \[x.y\] of this BRD states the business requirements accurately and authorize \[the next phase\]. Changes after sign-off go through \[the change control process, with link\].

| **Name** | **Role** | **Decision** | **Signature** | **Date** |
|----|----|----|----|----|
| \[Name\] | Business sponsor | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | Process owner | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
| \[Name\] | IT / solution lead | \[Approved / Approved with conditions / Rejected\] |  | \[YYYY-MM-DD\] |
