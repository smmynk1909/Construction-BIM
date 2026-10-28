# Product requirements document
Construction lifecycle web application | Version 0.1 | 26 October 2026

## 1 Product definition
A browser-based work platform with mobile-friendly field capture, configurable approval workflows, controlled engineering information, shared project/asset identifiers and role-specific work queues. Users should see what needs action, why it is blocked and what other teams are affected.

The product joins existing specialist systems wherever practical. It is not initially a replacement for BIM authoring, a statutory accounting ledger, a full scheduling solver or industrial control systems.

## 2 Product users and experiences
- Executives: portfolio exposure, gate decisions, liquidity and outcomes with drill-down to evidence.
- Sales and CRM: accounts, contacts, opportunities, bid decisions, commitments, milestones, complaints and renewals; marketing manages consent-aware campaigns and approved case studies.
- Land and business development: parcel map, opportunity/site linkage, rights and clearance conditions.
- Engineering and BIM: requirements, documents/models, revisions, review issues and intended-use releases.
- Planning: work breakdown, activity dependencies, baselines, short-term constraints and forecast updates.
- Finance and Accounting: budgets, commitments, cash and variance; certification, invoices, reconciliation and controlled close.
- Procurement and stores: demand, sourcing, orders, quality acceptance and stock movements.
- Construction and QHSE: released work packages, daily evidence, measurement, inspections, permits and safety holds.
- Operations: readiness, service performance, shift log, alarms/incidents, planned shutdowns and operating obligations.
- Maintenance: equipment/linear-asset history, service tasks, spares, work permits, work orders and warranty.
- Legal, compliance and commercial: obligations, notices, variations, approvals, claims and expiry calendars.
- Clients, consultants, suppliers and subcontractors: narrowly scoped submissions, clarifications, acceptance and status.

## 3 Product hierarchy and navigation
Portfolio → project → site/location or alignment/chainage → package → activity or asset → related transactions and evidence. Offer both a model/map view and a list view. Users must work without loading a large model. Search supports project, asset tag, document, BOQ line, order and obligation IDs.

Shared screens are My Work, Project Workspace, Commercial Workspace, Planning and Cost, Engineering Information, Supply and Stores, Field Delivery, Operations, Maintenance, Governance and Reports. Every detail screen shows state, revision, owner, dependencies, due date, approvals and linked records.

## 4 Prioritised requirements and acceptance
- **PR01 Shared identity and access [Must; BR01/12]:** an external supplier assigned to one order cannot discover another supplier's price, project files or search results. Permission checks cover exports and AI retrieval too.
- **PR02 Workflow engine [Must; BR01/06]:** configurable states, authority routes, parallel reviews, rejection, resubmission, escalation and delegation; no user can approve their own controlled financial request.
- **PR03 Commercial intake [Must; BR08]:** an awarded opportunity creates or links one project and an approved obligation register without duplicating award value during retries.
- **PR04 Design and BIM control [Must; BR01/09]:** publish immutable model/document revisions, intended-use status, review issues and object/quantity mappings. Users can identify the revision authorising site work.
- **PR05 Plan and cost baseline [Must; BR03/04]:** show original baseline, approved revisions, current forecast and actual status side by side; reject missing package/activity/cost coding.
- **PR06 BOQ and supply [Must; BR05/07]:** demonstrate a partial order, partial accepted receipt, rejection, return and invoice exception without overstating stock or commitments.
- **PR07 Verified progress and client billing [Must; BR03/05]:** submit measurements with evidence, prevent cumulative overclaim, track client certification disputes and collections independently of vendor invoices.
- **PR08 Accounting integration [Must; BR03]:** an accepted invoice receives a unique ERP reference or a visible failure; a retry cannot post twice. Reconcile status and amounts by entity/currency/period.
- **PR09 Asset readiness [Must; BR09/10]:** required asset fields and commissioning tests are known during design; block acceptance when mandatory evidence is absent.
- **PR10 Operations and maintenance core [Must; BR09/10]:** demonstrate a breakdown → approved work → spares issue → test → authorised return to service → closed costed job.
- **PR11 Sales and service continuity [Must; BR08]:** link delivery commitments to contract obligations and create renewal actions from service expiry without counting a renewal as booked revenue.
- **PR12 QHSE and compliance [Must; BR11]:** a critical open hold blocks the affected work/release, and reopening a defect restores the appropriate hold.
- **PR13 Assisted information [Should; BR12]:** extracted values and answers cite source revision/page where available, show confidence and require review before controlled records change.
- **PR14 Forecasting and condition intelligence [Later; BR04/10/12]:** predictions must beat an agreed baseline on time-separated evaluation and meet alert precision/recall thresholds before live decision support.
- **PR15 Portfolio optimisation and specialised extensions [Later]:** service profitability, resource scenarios, concession revenue or property sales enabled only where the business model needs them.

## 5 Releases and dependencies
**Foundation and discovery:** approve role/authority matrix, coding, source-system ownership, contract templates, data migration and integration proof. Profile real model files, cost codes and asset data. Exit: a usable data dictionary and agreed pilot tests.

**Pilot release A:** one project/package with commercial intake, basic land/clearance tracking, CDE/revision control, BOQ, baseline plan/budget, PR/PO/receipt, verified progress, vendor/client billing status and ERP integration. Include commissioning requirements and one asset's basic operations/maintenance lifecycle. This is the minimum end-to-end slice, not a whole-enterprise rollout.

**Release B:** richer CRM and bid pricing, procurement competition, subcontract billing, commissioning, bulk asset handover, shift/service operations, preventive/corrective maintenance, warranty, spares and service billing/renewals. Build on the asset and finance foundations already tested in A.

**Release C:** multi-project roll-up, advanced planning/4D visualisation, condition data, evaluated risk forecasts, portfolio commercial analytics and governed agent execution. Do not gate basic O&M on AI or sensors.

Timelines, staffing and costs follow discovery; these are dependency-based releases, not a delivery promise.

## 6 Proposed nonfunctional targets
These are sizing hypotheses to validate before architecture approval.
- For an agreed pilot load of 100 concurrent transactional users, p95 standard list/detail response ≤2 seconds excluding network, model processing and large exports. Define dataset sizes in the performance test plan.
- Background model import/export shows queued/running/failed/completed status and preserves partial failure diagnostics; test large representative files separately.
- Proposed monthly availability 99.5%, recovery point ≤1 hour and recovery time ≤4 hours for the business workflow service. Safety-critical field procedures and emergency response cannot depend on this service availability. Validate targets with Operations and IT.
- SSO/MFA, project-scoped roles, entity and supplier separation, encryption, auditable privilege changes and tested backups.
- Mobile capture tolerates disconnection; offline approvals, payments, work permits and return-to-service authorisations are disabled. Sync conflict resolution retains original evidence and author timestamps.
- Accessibility target WCAG 2.2 AA subject to formal verification; keyboard navigation, readable status text and alternatives to model-only actions.
- Currency, units, time zones, business calendars and language support are configurable. Store source values and explicit conversions.

## 7 Out of initial scope
Autonomous engineering sign-off, title certification, autonomous bank payments, automatic safety clearance, plant/road control, unrestricted generative design and universal ERP replacement. Detailed property sales, payroll and full manufacturing production management require separate scope decisions.

## 8 Product readiness and measurement
Track active users by role, required data completion, approval cycle time, exception age, reconciliation accuracy and repeated offline conflicts. Require process-owner UAT, permission and segregation testing, restore testing, integration retry tests and a complete asset/work-order rehearsal. Release B cannot weaken controls proven in A.

## 9 Architecture handoff
The architect should produce context/container diagrams, bounded domain model, integration contracts, permissions model, deployment/security plan, sizing evidence, migration approach and a decision log. Prototype model-to-BOQ-to-cost mappings and ERP idempotency before committing to implementation estimates. The functional specification and catalog provide the initial backlog decomposition.


## Product scope extension

[Marketing and service lifecycle requirements](09_MARKETING_AND_SERVICE_LIFECYCLE.md) extends this baseline with BR13, PR16–PR19, workflows WF11–WF14 and acceptance AT14–AT20. Marketing is a first-class domain M17; Sales, Operations and Maintenance retain distinct ownership. Use [Solution map and technical scope](08_SOLUTION_MAP.md) for the current module/data overview.
