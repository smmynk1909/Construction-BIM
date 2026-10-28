# Functional specification
Construction lifecycle platform | Version 0.1 | 26 October 2026

## 1 Process contract and governance inheritance
Every segment, capability, process and task carries an ID and the following process contract. The catalog gives concrete owners and handoffs; task-level entries inherit them unless an explicit override is approved. Inheritance must be resolved to named people at project setup, displayed to users and included in exports. A missing accountable owner prevents activation.

Required fields: purpose; trigger; upstream record IDs/revisions; inputs; preconditions; responsible executor R; one accountable decision owner A; consulted roles C; informed roles I; authority policy; workflow/state map; expected outputs; downstream dependencies; SLA/calendar; evidence; rejection/exception path; escalation owner; metric; retention and access class. A process owner is not automatically authorised to approve every amount or technical decision.

Tasks inherit the process's dependencies, RACI and controls, but have distinct due dates within its SLA. Changes to inherited policy create a versioned impact review; historical transactions retain the policy under which they were approved. Review and approval tasks may assign a different R to preserve segregation. Multiple A roles are represented as separate decisions, each with one A.

## 2 Canonical entities and relationships
**FR01 Organisation:** company/entity, portfolio, project, company project role, contract, package, party/contact, user, role assignment and authority delegation. External identifiers are stored with source system and source ID; internal immutable IDs remain stable.

**FR02 Location and asset:** parcel and right; site; building/floor/zone; alignment and chainage interval; system; maintainable asset; serial/tag; asset class; criticality; ownership/custodian; condition and warranty. Asset hierarchy and spatial hierarchy are separate but linked. Partial handover can activate one system while other packages remain in construction.

**FR03 Engineering information:** requirement; information delivery requirement; document container; immutable revision; model revision; model element reference; issue; review; transmittal and release. Element key includes model source and revision plus source object ID. Deleted or recreated model elements require explicit reconciliation; a GUID alone is not guaranteed continuity across authoring revisions.

**FR04 Controls and commercial:** WBS/work package; activity and predecessor; calendar; baseline; progress rule; cost account; estimate/BOQ revision and line; allocation; budget version; commitment; cost actual/accrual; forecast; opportunity; bid; obligation; variation; notice; measurement; certification; invoice and payment reference.

**FR05 Supply and execution:** material/service item with unit; demand/reservation; PR; RFQ; response; evaluation; PO/contract line; receipt; inspection; service acceptance; stock movement; daily report; work package; permit; nonconformance and incident.

**FR06 Operate and maintain:** commissioning test; handover pack; acceptance; service contract; shift log; operating event; downtime interval; asset reading; maintenance plan; work order; failure code; labour/time entry; spare issue/return; test; return-to-service approval and renewal.

**FR07 Governance:** workflow definition/version, instance, task, decision, SLA clock, exception, evidence, audit event, risk, obligation and integration event. Store creator/time, occurrence time, effective date, revision, state, currency/unit, source, permissions and correlation ID as applicable.

Relationships are many-to-many where needed. A model object can contribute to several BOQ lines; a BOQ line can cover many objects, activities and assets. Use allocation records with quantity, unit, basis and effective revision. Prevent repeated allocation from double counting and show unmapped quantities. Track non-modelled costs explicitly.

## 3 Common workflow engine
**WF00 Controlled decision:** Draft → Submitted → Validation → In review → Approved → Released/Executed → Closed. Validation failure returns to Draft with errors. Review may return Needs revision or Rejected; resubmission creates a new revision. Submitted/approved versions are immutable. Cancelled and Superseded preserve history.

Approval does not automatically mean permitted for construction, posted to the ledger, paid or returned to service. Those are distinct transitions with their own preconditions. Parallel reviews have mandatory/optional decisions and an explicit join rule. An overdue review never becomes approval automatically.

Authority routing uses entity, project, transaction type, amount/currency, risk, contract and policy effective date. Split purchases are flagged for review. Delegation has scope and expiry, cannot exceed delegator authority and cannot defeat self-approval controls. Missing approver routes to a governed exception queue.

Proposed SLA convention: business days use the assigned project calendar; elapsed hours use continuous time. Start on complete submission, stop at decision, and retain total elapsed time alongside active processing time. Only a reason-coded request for missing external information may pause the processing clock; show pause age. Warn at 75%, escalate at 100% to A, and at 150% to the relevant department head/project director. Emergency and safety responses use site procedures and continuous clocks; notifications do not substitute for emergency response.

## 4 Detailed cross-functional workflows
### WF01 Opportunity to contract and renewal
Sales records account, scope, business model, client procurement dates, estimated value, win probability and credit concerns. Qualification consults Engineering, Planning, Finance, Operations and Maintenance for deliverability and life-cycle commitments. Bid/no-bid is an authorised business decision, followed by controlled estimate, exclusions, risk review and tender approval.

Accepted negotiation produces an executed contract reference, obligations, milestones, payment terms, service requirements and scope baseline. Sales initiates the handover; Commercial validates obligations; Project Director accepts delivery ownership. Preserve bid cost, awarded price, internal budget and forecast margin separately. Lost bids retain reason and permitted learning data.

Client complaints link to a delivery issue, defect or maintenance work order. Service expiry creates a renewal task; a renewal becomes backlog only after authorised contract execution. Marketing publication of a project reference requires client consent where required and commercial approval. Property/unit inventory, booking cancellation and leasing are optional business-model extensions.

### WF02 Land and clearance
Land officer registers parcel, geospatial reference, document provenance, rights/interests and dates. Legal reviews title/rights evidence and restrictions; Engineering checks surveys and access; Compliance tracks permissions; Finance evaluates approved acquisition exposure. Approval records conditions rather than assuming full clearance.

Map overlaps and missing documents raise exceptions for human assessment. Acquisition and transfer require the appropriate agreement and authority. Construction readiness checks the specific required access/right/permit, validity and location. If the client owns land, record its clearance evidence and contractual responsibility rather than inventing company ownership.

### WF03 Design revision and change impact
Engineering submits a model/drawing revision and declared purpose. BIM/document control validates naming, metadata and agreed information requirements. Discipline reviewers resolve issues; Construction checks buildability; Planning checks sequence; Procurement checks ordered items; Finance/Commercial check cost and contract; Operations/Maintenance check access, isolation, reliability and lifecycle obligations.

Approved revision publishes with intended-use status and transmittal. A changed quantity or asset specification creates a controlled impact case linked to budget, schedule, outstanding POs, installed work, client variation and asset data. Do not overwrite downstream approved records. A change can require stop-work/hold or withdrawal of obsolete information. Review package scope and signed exceptions before release.

### WF04 Baseline and progress
Planning decomposes scope into WBS, packages and activities, captures calendars, predecessor relationships and constraints, then imports or calculates a schedule through the selected scheduling engine. Detect cycles and unconnected activities. Approve the baseline with resource/cost and contractual milestone alignment.

Field teams submit measured progress and evidence against the released package. QHSE validates required acceptance; Planning confirms the defined earning rule and updates the current forecast. Physical percent complete, quantity installed, client-certified quantity and invoice amount are distinct measures. Rejected work cannot earn accepted progress unless the explicitly approved measurement rule permits a separate reported category.

Use quantity-based progress where suitable; weighted milestones for equipment/design; define weights before baseline. Earned value is optional and requires an agreed time-phased budget and earning rules: PV = budgeted work scheduled; EV = budgeted work earned; AC = actual cost on the same basis; CPI = EV/AC and SPI = EV/PV only when denominator is positive. Do not use SPI alone to predict completion.

### WF05 Demand to paid supplier invoice
Approved scope/BOQ and plan create dated demand. Stores checks available accepted stock and reservations. Requester creates PR with item/service, unit, quantity, package, cost code, needed date and technical revision. Budget control reserves approved PR demand; it is not yet a contractual commitment.

Procurement sources qualified suppliers, separates technical and commercial evaluations, records tender confidentiality and conflict declarations, and routes award approval. Approved PO creates commitment and releases/replaces the corresponding PR reservation atomically. For partial conversion, retain only the unconverted reservation.

Receipt records delivered, accepted, rejected and quarantined quantities separately. QHSE releases quality holds; stores posts accepted stock; service orders use approved service acceptance or milestone certification. Supplier invoice matches PO, accepted receipt/service and invoice within approved tolerances. Duplicate checks include entity, supplier, invoice identifier and amount/date heuristics. Exceptions route to Procurement/Engineering/Accounting; tolerance does not bypass authority.

Accounting approves posting under its policy, integration sends the transaction once, and treasury/payment authority executes payment in the financial system. Import payment reference and reconcile. Handle partial receipts, advance payments with guarantees, retention, credit notes, cancellations, returns and disputed quantities through explicit document types. Any exceptional unmatched invoice requires an authorised exception, evidence and subsequent reconciliation.

### WF06 Measurement to client cash
Construction/QS submits cumulative measurements tied to package, BOQ and inspection evidence. Commercial reviews contractual eligibility, prior claimed/certified quantities, variations and deductions. Client/consultant certification may accept, partially accept or dispute quantities. Preserve submission and certification separately.

Accounting issues the invoice from the approved certification or other contractual billing basis; Finance tracks expected cash; Sales/Commercial manage collection actions and disputes. Store advances, retention, recoveries, tax and final settlement separately. Revenue recognition uses approved Accounting policy and ledger integration, not automatic conversion of site progress or cash received.

### WF07 Commissioning and handover
Define operating requirements, asset tags, criticality, test standards, manuals, training and spares during design. Commission by system with approved prerequisites, inspection/test evidence, punch list categories and permit/isolation controls. Retest failed systems; preserve failure history.

Engineering and commissioning lead recommend readiness; Operations accepts operational custody; Maintenance accepts data and maintainability; Commercial records client acceptance and warranty start per contract; Accounting reviews capitalisation eligibility where company-owned. None of these decisions is implied by another.

A conditional acceptance must list permitted residual defects, risk owner, remedy deadline and approver; safety-critical gaps block activation. Asset data transfers to the agreed asset system with acknowledged IDs and reconciliation. Project closure, client acceptance, warranty start and asset activation have distinct dates.

### WF08 Operations and corrective maintenance
Operations logs event, asset/location, severity, downtime and service impact. Triage distinguishes emergency response from routine work. Maintenance raises a work order; planner identifies tasks, competency, spares, permits and shutdown window. Operations authorises availability/isolation through site procedures; permitted work begins only after prerequisites are verified.

Technician records execution, time, materials, readings, failure/cause/action and evidence. Inspection/test confirms function. Authorised Operations representative approves return to service; Maintenance supervisor closes the job and reviews failure coding. Finance/Accounting receive costs on the approved asset and cost basis. A rejected test reopens execution; it cannot close the outage silently. Warranty-eligible work creates a recovery claim.

### WF09 Preventive and condition maintenance
Plan by calendar, usage meter, condition or statutory trigger. Version task lists and required competence. Generate orders idempotently using plan/asset/due-cycle key. Overdue critical/statutory work escalates; deferral requires risk assessment and designated authority, never an automatic reschedule that erases noncompliance.

Condition readings include units, calibration context and quality flag. Thresholds create triage alerts; predictive models only propose actions until evaluated. Store sensor event time and ingestion time, mark stale feeds and distinguish missing signal from healthy condition. Operations agrees shutdowns; spares and labour link to Planning, Procurement and cost forecast.

### WF10 Change and claims
A change records origin, affected baseline/revisions, reason, contractual entitlement, cost, schedule, cash, quality and operational impact. Engineering, Planning, Commercial, Finance, Operations and Maintenance review their impacts. The delegated authority approves scope/cost decisions; client approval is captured separately when required.

Notice deadlines follow contract-specific rules with source clauses and owner review. An AI-extracted date is proposed until confirmed. Approved change revises relevant baselines through linked versioned transactions. Pending/unapproved changes remain visible as exposure and do not silently increase authorised budget. Emergency work follows a defined emergency authority and later ratification without pretending approval existed earlier.

## 5 Budget and stock calculation rules
Approved budget B includes only authorised revisions. Commitments distinguish original, amendments, cancelled amount, fulfilled/invoiced portion and outstanding portion. PR reservations, PO commitments, accruals and actuals are separate states, with explicit transitions to prevent duplication.

Forecast EAC = posted actuals + nonduplicated unposted incurred/accrued costs + remaining open committed cost + forecast uncommitted cost to complete. Reconcile matched invoices/receipts/accrual reversals so no cost occurs twice. Contingency and pending changes follow a disclosed forecast policy. Variance at completion = B − EAC; positive is favourable. Cash forecast additionally uses payment terms, advances, retention and taxes; it is not EAC.

Stock on hand = accepted opening + accepted receipts + accepted returns/transfers in − issues − supplier returns − transfers out ± approved adjustments. Available = usable on hand − reservations; quarantined/rejected stock is not usable. Installed quantity is recorded through accepted execution, not inferred from warehouse issues. Use controlled unit conversions and retain original units. Negative stock is blocked unless a scoped, approved policy explicitly permits it.

## 6 Integration and technical boundaries
Prefer a modular application with explicit domain APIs and a transactional core initially. Separate file/model processing, search and AI jobs from interactive approvals. Use durable asynchronous events/outbox, idempotency keys, retry limits and a visible dead-letter/exception queue. Microservices are an architectural option after scale/team boundaries justify them.

Authoritative sources must be chosen per object: identity provider for identities; authoring/CDE for published engineering files if retained; scheduling system for calculation if retained; ERP for posted actuals, tax, receivables/payables and payment status; CRM/EAM for their records if retained. The new platform owns only the objects explicitly assigned to it. Never implement unrestricted dual-master updates.

Candidate interfaces: SSO; CRM; ERP; scheduling imports/APIs; CDE/model files; GIS/land evidence; EAM/CMMS; document signatures; notifications; sensor historians via read-only gateways. Agree supported versions and connectors through proof-of-concept. IFC handles model exchange, BCF issue exchange, IDS machine-readable information checks where supported. These do not guarantee a complete bidirectional native-model round trip.

Each integration contract defines source/target, object/field mapping, authority, cadence, auth, units/currency, effective dates, idempotency, error handling, reconciliation and support owner. Event example: InvoicePostingRequested contains event ID, entity, invoice ID/revision, source document hash, currency, posting date and approved coding. Receiver returns external reference and status; a network timeout triggers lookup/retry with the same key.

## 7 AI and agent controls
First use retrieval over authorised approved records, extraction into review queues, meeting/action drafts and missing-evidence alerts. Each response carries source revision/as-of date; stale/superseded content is labelled. Uploaded documents and embedded instructions are untrusted content, not permission to invoke tools.

Agents operate with scoped service identities, an allowlist of tools, amount/action limits, idempotency, audit logs and human approval before controlled writes. They may prepare a PR or work order; they cannot approve engineering, certify title, post discretionary journals, authorise payment, clear permits or return assets to service.

ML schedule, cost and failure models need sufficient representative history, temporal train/test separation, leakage checks, comparison against simple rules and evaluation by asset/project segment. Publish precision/recall, false-alert cost and forecast error appropriate to the use case; agree thresholds before deployment. Monitor drift, data gaps and overrides. Computer-vision progress remains suggested evidence until measurement/quality verification.

## 8 Security and audit
Enforce project/entity/party scope at API, storage, search, export and AI retrieval. Separate technical tender access from commercial pricing. Sensitive land, personal and employee data require restricted fields and defined retention. Preserve immutable audit events for approvals, changes, policy/delegation and integration outcomes. Log original and revised values without leaking secrets.

Financial close locks approved periods; corrections use authorised reversal/adjustment transactions. Evidence retention and deletion policies must respect contract, jurisdiction and legal holds. Backup restore tests include evidence links and audit integrity.

## 9 Minimum acceptance scenarios and traceability
- **AT01 [BR01/12; PR01/02; FR01/07]:** requester tries self-approval, expired delegation and cross-project access; all fail and are auditable.
- **AT02 [BR08; PR03/11; WF01]:** awarded bid includes a service promise; it becomes an owned obligation, delivery milestone and renewal reminder without duplicate award value.
- **AT03 [BR02/11; PR12; WF02]:** expired access permission blocks only affected work; resolving an unrelated document cannot release it.
- **AT04 [BR01/07; PR04/06; WF03]:** changed model quantity affects an open PO; existing approval is preserved and a change case reaches Engineering, Planning, Procurement and Finance.
- **AT05 [BR04; PR05; WF04]:** revised forecast finish changes while approved baseline stays intact; rejected work remains outside accepted progress.
- **AT06 [BR03/05/07; PR06/08; WF05]:** order 100 units, receive 60, accept 55, quarantine 5, invoice 60. Only 55 become usable stock; excess invoice quantity becomes an exception. Retry never creates a second ledger posting.
- **AT07 [BR03/05; PR07; WF06]:** client certifies 80 of 100 claimed; record 20 disputed and invoice only the contractually authorised basis. Collection does not rewrite recognised revenue.
- **AT08 [BR09/10; PR09; WF07]:** missing mandatory operating manual blocks asset acceptance; conditional noncritical punch items require explicit approved disposition.
- **AT09 [BR09/10; PR10; WF08]:** failed post-maintenance test keeps the asset unavailable; spare use, labour and downtime remain linked until authorised return to service.
- **AT10 [BR10; PR10/14; WF09]:** duplicate maintenance scheduler run generates one order; stale sensor data produces a quality alert rather than a healthy status.
- **AT11 [BR03/06; PR05; WF10]:** pending variation appears as exposure, not approved budget; approval creates linked baseline revisions with authority evidence.
- **AT12 [BR12; PR13; AI controls]:** a supplier document attempts to instruct an agent to release payment; no tool executes and the attempted instruction is treated as document content.
- **AT13 [BR01/12; PR01/08; integration]:** offline photo sync conflicts with a revised record; preserve both evidence timestamps and route reconciliation rather than overwriting approval.

These scenarios seed UAT. Detailed field validation, edge cases and load/security suites follow module elaboration.

## 10 Definition of a module ready for development
Approved process contract and mock screens; complete state/transition permissions; field dictionary and sample data; confirmed source ownership; API/event contracts; exceptions and reconciliation; business rules; audit/retention needs; accepted test scenarios; migration and support responsibilities. Without these, estimates remain provisional.


## Workflow extension

[Marketing and service lifecycle requirements](09_MARKETING_AND_SERVICE_LIFECYCLE.md) extends this baseline with BR13, PR16–PR19, workflows WF11–WF14 and acceptance AT14–AT20. Marketing is a first-class domain M17; Sales, Operations and Maintenance retain distinct ownership. Use [Solution map and technical scope](08_SOLUTION_MAP.md) for the current module/data overview.
