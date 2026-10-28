# Business requirements document
Construction lifecycle platform | Version 0.1 | 26 October 2026

## 1 Purpose and business case
Provide controlled, traceable execution of capital projects and subsequent asset services. The business problem is fragmented accountability: a changed drawing may not reach procurement; progress may not support billing; installed assets may reach maintenance without service information. The application must connect these handoffs and show who must decide next.

The sponsor is the Managing Director. Proposed business co-owners are the heads of Sales, Planning, Finance, Accounting, Operations and Maintenance, supported by Engineering, Commercial, Procurement, QHSE and IT. A process council approves enterprise templates; project directors own execution within approved authority.

## 2 Business requirements
- **BR01 Lifecycle accountability:** every controlled transaction has a named owner, current state, next action, due date and evidence. Escalations cannot silently transfer accountability.
- **BR02 Digital land bank:** register parcels, mapped boundaries, owners/rights, restrictions, source documents, due-diligence tasks and renewal obligations. A document upload does not prove legal title; legal clearance and unresolved conditions must remain explicit.
- **BR03 Financial control:** separate approved budget, commitments, actuals, accruals, forecast, client billings, recognised revenue and cash. Control changes and reconcile to the ledger.
- **BR04 Integrated planning:** maintain baselined work breakdown, logic, calendars, resource and material constraints, progress rules and recovery plans. Keep baseline and current forecast independently visible.
- **BR05 Procurement and billing:** link request, sourcing, award, order, receipt/service acceptance, supplier invoice, exceptions and payment status; link client measurements, certification, invoice and collection separately.
- **BR06 Review and communication:** use structured reviews, transmittals, decisions, approval authority and overdue action tracking. Chat comments alone cannot approve a controlled item.
- **BR07 BOQ and inventory:** version quantity/rate assumptions and their allocation to demand, reservations, receipts, issues, returns and installed quantities. BOQ demand is not physical stock.
- **BR08 Commercial continuity:** connect sales promises and exclusions to executable contract obligations, delivery scope and collections. Include service opportunities, renewals, key accounts and client complaints.
- **BR09 Operational readiness:** establish operability, maintainability and acceptance requirements during concept/design, then verify them through commissioning and handover.
- **BR10 Asset reliability:** maintain asset register, criticality, preventive work, corrective work, failure history, warranty and spares, with return-to-service authority.
- **BR11 Quality and safety:** control inspections, test evidence, nonconformances, permits, incidents and corrective actions. Commercial urgency must not bypass a safety hold.
- **BR12 Governed intelligence:** present timely information with source, revision, freshness and permissions; distinguish AI suggestions, estimates and verified facts.

## 3 Business boundaries and company roles
A project template must declare the company role and contracted responsibilities. An EPC contractor may only view the client's land clearance and approved maintenance deliverables. An owner-operator may own land acquisition, capitalisation and ongoing operations. A concessionaire may also manage operating revenue and service-level deductions. External parties see only their approved project, package and transaction scope.

Sales and marketing own demand generation and client relationships. Tendering owns bid assembly; Commercial owns contractual obligations; Planning owns executable logic; Finance owns funding and financial outlook; Accounting owns posted books and policy application. Operations owns safe asset use and service delivery; Maintenance owns asset care and work execution. Ownership may be combined in a smaller company but decision rights and segregation controls must still be explicit.

## 4 Lifecycle gates
For each gate the system records submitted evidence, conditional approvals, named approver, timestamp, policy version, decision reasons and affected packages. The approver is the sponsor or a delegated role recorded in the authority register.

- **G0 Opportunity and site qualification:** Sales and Land/Legal establish client fit, site constraints and permissions to investigate. Finance assesses capacity and credit. Output is pursue, hold or decline.
- **G1 Concept approval:** Engineering proposes options; Planning, Finance, Operations and Maintenance review scope, affordability, delivery strategy and serviceability. Output is an approved concept and explicit assumptions.
- **G2 Schematic approval:** coordinated discipline layouts, preliminary quantities, planning logic, maintainability review and permit strategy. Output is a controlled basis for further design.
- **G3 Detailed design/package release:** approved engineering, constructability, model checks, quantities and cost/schedule impacts. Release is by package and intended use; procurement release does not automatically authorise construction.
- **G4 Tender/award:** approved bid or package award, exclusions, contractual risk, funding, authority and obligations. Outbound client tenders and inbound subcontract/supply tenders have separate permissions and workflows.
- **G5 Construction readiness and control:** site access, released information, permits, labour/equipment, materials and inspection plans; recurring package readiness checks and controlled changes.
- **G6 Handover and operational acceptance:** tested systems, safe isolation arrangements, accepted asset data, manuals, training, spares, warranties and agreed residual defects. Operations can reject incomplete readiness.
- **G7 Service performance and asset care:** ongoing operational review, maintenance compliance, reliability, OPEX, service revenue and renewal. Major modifications return to design/change control. Include retirement/disposal authorisation and data retention at end of life.

## 5 Value measures and ownership
Targets must be set after a pilot baseline; none are guaranteed savings from consulting studies.
- Sales head: bid conversion by value and count, bid margin versus awarded margin, renewal rate and aged client actions. Keep weighted pipeline separate from contracted backlog.
- Planning head: milestone variance, constraints overdue and percent of weekly commitments completed. Compare forecast finish to the approved baseline, with as-of date.
- Finance head: estimate-at-completion variance, cash forecast error and unapproved exposure. Show uncertainty and pending changes separately.
- Accounting head: reconciliation exceptions, unbilled accepted work, receivable ageing and close-cycle time. Revenue follows approved policy, not model progress automatically.
- Procurement head: PR-to-PO elapsed business time, on-time accepted delivery and exception ageing.
- Operations head: availability of serviceable assets, operating incidents, contractual service compliance and operating cost by asset/service.
- Maintenance head: preventive maintenance completed by due date / scheduled due, mean repair duration for qualifying corrective jobs, repeat failures and warranty recoveries.
- QHSE head: defect closure time, overdue safety actions and first-pass inspections. Do not optimise closure counts at the expense of actual risk removal.

The metric register must define numerator, denominator, source, exclusions, time window, owner and freshness. Baseline comparable projects and track adoption and data quality alongside business outcomes.

## 6 Governance and adoption
Weekly package reviews resolve constraints. Monthly project reviews resolve forecast, cash and change exposure. Quarterly portfolio reviews assess investments, sales pipeline and benefits. Daily site and operating reviews use safety and criticality-driven queues. Cadences are configurable to the project and contract.

A data steward in each domain owns completeness, code quality and reconciliation. The design authority approves schema and integration changes. Superusers test workflows with office and field teams. Training must use actual project scenarios, and subcontractor onboarding must specify evidence and data submission duties.

## 7 Risks and assumptions
Key risks are conflicting source systems, inconsistent codes, retrospective approvals, weak field connectivity, overambitious model fidelity, hidden contractual variations and poor asset handover. Mitigate through explicit source ownership, staged migration, offline evidence capture, package-level gates and rehearsed commissioning/maintenance scenarios.

Country-specific land, procurement, safety, privacy, tax, revenue and retention obligations require local review before configuration. No jurisdiction is assumed in this baseline.

## 8 Business acceptance
Business owners accept the pilot only after one real package can be traced from commercial commitment through design, budget, plan, procurement, verified work, billing and accounting reconciliation, and one asset can move through acceptance to a closed maintenance order. Outstanding exceptions must have named owners and agreed disposition; no critical safety or access-control exception may be waived by the product team.


## Business scope extension

[Marketing and service lifecycle requirements](09_MARKETING_AND_SERVICE_LIFECYCLE.md) extends this baseline with BR13, PR16–PR19, workflows WF11–WF14 and acceptance AT14–AT20. Marketing is a first-class domain M17; Sales, Operations and Maintenance retain distinct ownership. Use [Solution map and technical scope](08_SOLUTION_MAP.md) for the current module/data overview.
