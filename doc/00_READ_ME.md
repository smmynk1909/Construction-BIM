# Construction lifecycle platform blueprint
Version 0.2 | 27 October 2026 | For business and technical architecture review

## Recommended direction
Build a governed construction lifecycle platform with BIM as the engineering information backbone. Connect opportunity to contract, design to delivery, procurement to payment, and commissioning to reliable operation. Marketing, Sales, Planning, Finance, Accounting, Operations and Maintenance are first-class domains with their own records, approvals and measures.

This is an overall requirements baseline for discussion, not a signed construction method, legal opinion, accounting policy or implementation estimate. All roles, SLAs, phases and targets are proposed until company owners approve them. The country, contractual delivery model, software estate, project scale and statutory obligations have not yet been established.

## Read in this order
Start with [Solution map and technical scope](08_SOLUTION_MAP.md) for a concise technical review. [Marketing and service lifecycle requirements](09_MARKETING_AND_SERVICE_LIFECYCLE.md) adds explicit Marketing ownership and specialised Sales/Operations/Maintenance acceptance.

1. **01_BRD.md** — business outcomes, operating model, lifecycle gates, measures and boundaries.
2. **02_PRD.md** — product scope, users, releases, measurable acceptance and architecture constraints.
3. **03_FUNCTIONAL_SPECIFICATION.md** — shared data, workflow states, detailed process rules, controls, integrations and test scenarios.
4. **04_MODULE_AND_GOVERNANCE_CATALOG.md** — teams → capabilities → processes → implementation steps, with explicit dependency, RACI, SLA and governance inheritance.
5. **05_RESEARCH_AND_DESIGN_RATIONALE.md** — consulting research, research methods, limits and resulting design choices.
6. **06_VISUAL_MAPS.html** — snowflake capability map, fishbone risk map and cross-functional workflow diagrams. Open in a browser; select a diagram to view or print it.

The identifiers BR, PR, FR, M and WF connect these documents. The catalog is the authoritative initial module breakdown. The functional specification supplies the reusable workflow patterns used by its processes.

## What BIM means in this application
BIM joins structured information about a built asset to models and documents over its lifecycle. A model viewer alone does not manage contracts, payments or maintenance. The proposed platform links BIM objects and controlled model revisions to work packages, BOQ lines, activities, inspections, cost accounts and maintained assets. Many records, including land rights, commercial opportunities and overhead costs, legitimately have no model object.

Authoring tools remain responsible for design production; the application coordinates information requirements, reviews, approvals, changes and evidence. Model ingestion must be tested on representative road, factory and infrastructure files before a supported schema/version promise is made.

## Two connected journeys
**Commercial journey:** campaign/source → lead/account → opportunity → qualification → bid/no-bid → estimate → tender → negotiation → contract → delivery commitments → client billing → collections → renewal and service revenue.

**Asset journey:** land/site due diligence → concept → schematic → detailed design → tender packages → construction → commissioning → handover → operation → maintenance → refurbishment or retirement.

They overlap. Tendering can happen before detailed design under design-and-build arrangements. Land acquisition may be client-owned. Packages can be at different stages; a project-level gate must not falsely imply every package has the same maturity. Contract requirements determine which activities and gates are mandatory.

## Working example
A factory pump moves from a design requirement to a tagged BIM object, an approved specification and a BOQ allocation. Planning sets its required-on-site date. Procurement orders it against an approved budget. Stores records delivery and serial number; QHSE inspects it. Construction records installation; commissioning proves performance. Finance matches the invoice to the order and accepted receipt. Operations accepts the asset, and Maintenance receives its warranty, spares and service plan. Sales can subsequently manage the maintenance renewal. Every link references the relevant revision and evidence.

For a road, the corresponding chain uses alignment, chainage and section, earthworks or pavement quantities, approved measurements, road-opening acceptance and condition inspections. A road section is an asset/location context; it need not be treated as a factory equipment tag.

## Initial delivery strategy
Start with a thin but complete pilot: opportunity/contract intake → shared project and location codes → approved design/BOQ/budget/schedule → PR/PO → receipt or service acceptance → verified progress → client certification and vendor billing → ERP reconciliation. In parallel, define asset and handover requirements and pilot one maintenance work order so operational needs shape design from the beginning.

Extend the same foundations into commissioning, operations, maintenance and portfolio services. Early AI should extract and retrieve reviewed information, flag missing records and draft summaries. Predictive AI follows reliable history and evaluated performance. Approval decisions stay with authorised people.

## Decisions needed for the next iteration
- Business model: EPC contractor, developer, owner-operator, concessionaire, or a combination? Separate templates should serve each.
- Pilot asset: road section, factory package, bridge or another defined project?
- Sales model: B2B bids and service contracts, property/unit sales, leasing, or several? This version prioritises B2B project and service sales; property sales is an optional extension.
- Countries, currencies, entities, tax regimes, client reporting and contract forms?
- Existing ERP/accounting, CRM, BIM authoring/CDE, scheduling and maintenance systems?
- User/concurrency scale, file sizes, field connectivity, hosting and security requirements?
- Named process owners, approval authority limits and emergency operating procedures?

## Next workshop outputs
Confirm those decisions, map five real transactions from source evidence, agree the coding structure, set baseline measures and approve one pilot scope. Then elaborate one module at a time using the detailed process contract in the functional specification. Do not procure an entire technology stack before the workflows and integrations have been tested on actual project data.
