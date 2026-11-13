# brd-frd-documents

Templates and worked examples for writing **Business Requirements Documents (BRDs)** and **Functional Requirements Documents (FRDs)**. Each one follows a recognized standard: the IIBA's **BABOK® Guide v3** or **ISO/IEC/IEEE 29148:2018**, the successor to IEEE 830.

Each template has a complete worked example. All the examples describe the same fictional project, *Tarang Direct*, so you can see what a finished document looks like and follow a requirement from the business need down to a functional requirement that can be tested.

## BRDs and FRDs

- **Business Requirements Document (BRD):** why the organization is making a change and what business outcomes it needs. It is written from the business point of view and does not depend on any particular solution. ISO/IEC/IEEE 29148 calls this document a *Business Requirements Specification (BRS)*.
- **Functional Requirements Document (FRD):** what the solution must do and how well it must work. It is detailed enough for a delivery team to design and build the solution and for testers to verify it. In ISO/IEC/IEEE 29148 terms, this is a *Software Requirements Specification (SRS)*.

The BRD is written first. The FRD is derived from it, and each requirement in the FRD traces back to the BRD.

## Contents of this repository

| Folder | Document | Standard | Template | Worked example |
|---|---|---|---|---|
| [BRD-IIBAs-BABOK-Guide-v3](BRD-IIBAs-BABOK-Guide-v3/) | BRD | BABOK Guide v3 | [BRD_Template_BABOK_v3.docx](BRD-IIBAs-BABOK-Guide-v3/BRD_Template_BABOK_v3.docx) | [BRD_Example_Ecommerce_Portal_Tarang_Direct.docx](BRD-IIBAs-BABOK-Guide-v3/BRD_Example_Ecommerce_Portal_Tarang_Direct.docx) |
| [BRD-ISO-IEC-IEEE-29148](BRD-ISO-IEC-IEEE-29148/) | BRS | ISO/IEC/IEEE 29148:2018 | [BRS_Template_ISO-IEC-IEEE_29148.docx](BRD-ISO-IEC-IEEE-29148/BRS_Template_ISO-IEC-IEEE_29148.docx) | [BRS_Example_ISO29148_Ecommerce_Tarang_Direct.docx](BRD-ISO-IEC-IEEE-29148/BRS_Example_ISO29148_Ecommerce_Tarang_Direct.docx) |
| [FRD-IIBAs-BABOK-Guide-v3](FRD-IIBAs-BABOK-Guide-v3/) | FRD | BABOK Guide v3 | [FRD_Template_BABOK_v3.docx](FRD-IIBAs-BABOK-Guide-v3/FRD_Template_BABOK_v3.docx) | [FRD_Example_BABOK_Ecommerce_Tarang_Direct.docx](FRD-IIBAs-BABOK-Guide-v3/FRD_Example_BABOK_Ecommerce_Tarang_Direct.docx) |
| [FRD-IEEE830-ISO29148](FRD-IEEE830-ISO29148/) | FRD (SRS) | ISO/IEC/IEEE 29148:2018 / IEEE 830 | [FRD_Template_IEEE830_ISO29148_Structure.docx](FRD-IEEE830-ISO29148/FRD_Template_IEEE830_ISO29148_Structure.docx) | [FRD_Example_SRS_Structure_Ecommerce_Tarang_Direct.docx](FRD-IEEE830-ISO29148/FRD_Example_SRS_Structure_Ecommerce_Tarang_Direct.docx) |

### BRD: BABOK Guide v3

This template is organized around the BABOK requirements classification schema. It has five requirement types, each with its own ID prefix: business (`BR-`), stakeholder (`SR-`), functional (`FR-`), non-functional (`NFR-`) and transition (`TR-`). It also covers:

- the business need and business case
- the current state (as-is) and future state (to-be)
- scope and stakeholders
- business rules
- assumptions, constraints, dependencies and risks
- a requirements traceability matrix and a requirements quality checklist

Requirements are prioritized with MoSCoW. The template also explains how agile teams can keep the detailed requirements in their backlog.

### BRS: ISO/IEC/IEEE 29148

This template follows the BRS content items in clause 9.3 of ISO/IEC/IEEE 29148:2018, and a table maps each section to its clause. It covers:

- the business purpose, scope and overview
- stakeholders and the business environment
- goals and objectives
- the business model and the information environment
- business processes, policies and rules
- the operational concept and scenarios

The appendices hold a business requirements register, a quality checklist, a traceability matrix and an issues and decisions log.

### FRD: BABOK Guide v3

This template uses only the BABOK Guide v3. BABOK does not prescribe a document format, so the sections follow its concepts:

- the requirements architecture
- the five model categories: people and roles, rationale, activity flow, capability, and data and information
- functional, non-functional, interface and transition requirements
- the requirements life-cycle tasks: verification, validation, traceability, prioritization and change control

### FRD: IEEE 830 / ISO/IEC/IEEE 29148 SRS structure

This template follows the example SRS outline in ISO/IEC/IEEE 29148:2018 and maps each section back to IEEE 830-1998. It covers:

- functions
- performance and usability
- interfaces
- logical database requirements
- design constraints
- software system attributes: reliability, availability, security, maintainability and portability

Each requirement is ranked Essential, Conditional or Optional. A verification matrix assigns each one a verification method: inspection, analysis, demonstration or test.

## The worked example: Tarang Direct

Tarang Home & Kitchen Pvt. Ltd. is a fictional Indian retailer of home décor, kitchenware and furnishings. It has 38 stores in 11 cities and sells online only through third-party marketplaces. *Tarang Direct* is its own direct-to-consumer e-commerce portal, built as a responsive website and progressive web app. The portal shows stock across 2 warehouses and 12 pilot stores, offers home delivery or collection from a store, and brings the company's loyalty programme online.

The four example documents describe the same project at different levels, and their IDs trace from one to another:

| Document ID | Document | Role |
|---|---|---|
| BRD-DIG-014 | BRD (BABOK) | The source document. It records the business need, the scope and all five BABOK requirement types. |
| BRS-DIG-014 | BRS (ISO 29148) | Describes the same need at the business level only. The BRD's business requirements become its goals and objectives. |
| FRD-DIG-014-B | FRD (BABOK) | The Release 1 solution requirements, derived from the BRD. |
| FRD-DIG-014-S | FRD (SRS structure) | The same Release 1 requirements in the ISO 29148 SRS structure. |

To see how the two standards present the same requirements, compare the two FRD examples side by side.

The BRD and FRD templates also have sample rows from a smaller example of their own, an accounts-payable invoice-processing system.

## How to use the templates

1. Make one copy of the template for each initiative, product or release.
2. Replace every `[bracketed placeholder]`.
3. Delete the *Guidance* notes and the sample rows before the first review.
4. Give every requirement a unique ID that is never reused, and keep the traceability matrix up to date as requirements change.

If you are new to requirements documents, read the BRD example first and then one of the FRD examples.

## Notes

- All organizations, people, figures, systems and dates in the examples are fictional.
- The regulatory content in the examples reflects Indian law as of November 2026, including the Consumer Protection (E-Commerce) Rules 2020 and the Digital Personal Data Protection (DPDP) Act. Confirm it with legal counsel before you use it on a real project.
- The guidance text in the templates is original and does not reproduce the standards. For the normative wording, refer to the BABOK Guide and ISO/IEC/IEEE 29148. ISO/IEC/IEEE 29148 clause numbers refer to the 2018 edition.
- This repository is not affiliated with or endorsed by IIBA, ISO, IEC or IEEE. BABOK® is a registered trademark of the International Institute of Business Analysis.

## License

[MIT](LICENSE)
