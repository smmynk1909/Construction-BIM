# Module and governance catalog
Construction lifecycle platform | Version 0.1 | 26 October 2026

## How to implement the hierarchy
Level 1 is a team segment Mxx; level 2 is its capability Mxx.1; level 3 is a process Mxx.1.n; level 4 is a sequence of implementation tasks Mxx.1.n.t. Additional capabilities can be introduced during detailed workshops. This is an initial decomposition, not an exhaustive construction work method.

Every node has dependencies, RACI, SLA, workflow and governance through the explicitly stated inheritance below. At activation, materialise the resolved values for each node and replace roles with named assignments. No child can weaken a parent control. Task due dates sum within the process SLA; longer contractual timelines must be modelled separately. SLAs below govern complete internal reviews or triage, not external approvals, physical completion or emergency response.

R performs work; A owns the process outcome; C gives required input; I receives the outcome. Actual approval steps use the authority register and separate decision owners. RACI strings below are compact matrix rows; they must become a role-by-task matrix when a module is elaborated. Technical, safety, financial and client decisions remain separately authorised even when a process has one A.

Common inherited controls at every node: scoped access; immutable submitted revisions; evidence; authority checks; segregation; audit trail; reason-coded exceptions; expiry checks; escalation at SLA breach. Common workflow definitions WF00–WF10 are in the functional specification.


## M01 Sales and CRM
**Level 1 contract:** R Sales executive; A Sales head; C Commercial, Finance, Planning, Operations, Maintenance; I Project Director. Upstream: account, client requirements. Downstream: contract obligations, bid scope, renewals. SLA: 2 business days for qualification decision. Workflow: WF01. Governance: No unsupported delivery promises; signed award before backlog. Escalation: Sales head, then Project Director/sponsor for unresolved cross-functional issues.

### M01.1 Opportunity and customer lifecycle
**Level 2 contract:** inherits the full M01 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M01.1.1 Opportunity qualification
**Level 3 contract:** inherits M01.1 RACI and SLA; explicit input/output handoff: client brief → qualify capacity and credit → bid decision → approved pursuit. Cross-functional links: Commercial, Finance, Planning, Operations, Maintenance; notify Project Director. Workflow WF01; controls: No unsupported delivery promises; signed award before backlog. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M01.1.1.1** Client brief. Task contract inherits M01.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.1.2** Qualify capacity and credit. Task contract inherits M01.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.1.3** Bid decision. Task contract inherits M01.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.1.4** Approved pursuit. Task contract inherits M01.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M01.1.2 Bid and contract handover
**Level 3 contract:** inherits M01.1 RACI and SLA; explicit input/output handoff: approved pursuit → compile priced scope and exclusions → negotiate and approve → accepted obligations. Cross-functional links: Commercial, Finance, Planning, Operations, Maintenance; notify Project Director. Workflow WF01; controls: No unsupported delivery promises; signed award before backlog. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M01.1.2.1** Approved pursuit. Task contract inherits M01.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.2.2** Compile priced scope and exclusions. Task contract inherits M01.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.2.3** Negotiate and approve. Task contract inherits M01.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.2.4** Accepted obligations. Task contract inherits M01.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M01.1.3 Customer service and renewals
**Level 3 contract:** inherits M01.1 RACI and SLA; explicit input/output handoff: complaint or expiry → route delivery/service action → verify client resolution → renewal or closure. Cross-functional links: Commercial, Finance, Planning, Operations, Maintenance; notify Project Director. Workflow WF01; controls: No unsupported delivery promises; signed award before backlog. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M01.1.3.1** Complaint or expiry. Task contract inherits M01.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.3.2** Route delivery/service action. Task contract inherits M01.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.3.3** Verify client resolution. Task contract inherits M01.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M01.1.3.4** Renewal or closure. Task contract inherits M01.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M02 Land and business development
**Level 1 contract:** R Land officer; A Land head; C Legal, Engineering, Compliance, Finance; I Planning, Sales. Upstream: parcel evidence, site opportunity. Downstream: clearance conditions, project feasibility. SLA: 5 business days for complete internal due-diligence review. Workflow: WF02. Governance: Legal clearance records conditions; no automatic title certification. Escalation: Land head, then Project Director/sponsor for unresolved cross-functional issues.

### M02.1 Site rights and feasibility
**Level 2 contract:** inherits the full M02 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M02.1.1 Parcel register
**Level 3 contract:** inherits M02.1 RACI and SLA; explicit input/output handoff: site lead → map parcel and rights → check provenance/overlaps → publish controlled register. Cross-functional links: Legal, Engineering, Compliance, Finance; notify Planning, Sales. Workflow WF02; controls: Legal clearance records conditions; no automatic title certification. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M02.1.1.1** Site lead. Task contract inherits M02.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.1.2** Map parcel and rights. Task contract inherits M02.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.1.3** Check provenance/overlaps. Task contract inherits M02.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.1.4** Publish controlled register. Task contract inherits M02.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M02.1.2 Due diligence and acquisition
**Level 3 contract:** inherits M02.1 RACI and SLA; explicit input/output handoff: registered parcel → review legal/technical restrictions → approve transaction authority → execute and record rights. Cross-functional links: Legal, Engineering, Compliance, Finance; notify Planning, Sales. Workflow WF02; controls: Legal clearance records conditions; no automatic title certification. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M02.1.2.1** Registered parcel. Task contract inherits M02.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.2.2** Review legal/technical restrictions. Task contract inherits M02.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.2.3** Approve transaction authority. Task contract inherits M02.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.2.4** Execute and record rights. Task contract inherits M02.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M02.1.3 Access and obligation monitoring
**Level 3 contract:** inherits M02.1 RACI and SLA; explicit input/output handoff: required work location → verify access and permit validity → escalate conditions → release eligible readiness checks. Cross-functional links: Legal, Engineering, Compliance, Finance; notify Planning, Sales. Workflow WF02; controls: Legal clearance records conditions; no automatic title certification. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M02.1.3.1** Required work location. Task contract inherits M02.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.3.2** Verify access and permit validity. Task contract inherits M02.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.3.3** Escalate conditions. Task contract inherits M02.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M02.1.3.4** Release eligible readiness checks. Task contract inherits M02.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M03 Engineering and BIM
**Level 1 contract:** R Discipline engineer; A Engineering head; C BIM lead, Construction, Planning, Procurement, Operations, Maintenance; I Commercial, Finance. Upstream: client/asset requirements, surveys. Downstream: released design, BOQ impact, asset specifications. SLA: 3 business days for complete package review. Workflow: WF03. Governance: Release by revision and intended use; engineering authority sign-off. Escalation: Engineering head, then Project Director/sponsor for unresolved cross-functional issues.

### M03.1 Controlled design information
**Level 2 contract:** inherits the full M03 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M03.1.1 Design requirements and options
**Level 3 contract:** inherits M03.1 RACI and SLA; explicit input/output handoff: approved concept brief → compare design options → review operability and cost → approve design basis. Cross-functional links: BIM lead, Construction, Planning, Procurement, Operations, Maintenance; notify Commercial, Finance. Workflow WF03; controls: Release by revision and intended use; engineering authority sign-off. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M03.1.1.1** Approved concept brief. Task contract inherits M03.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.1.2** Compare design options. Task contract inherits M03.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.1.3** Review operability and cost. Task contract inherits M03.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.1.4** Approve design basis. Task contract inherits M03.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M03.1.2 Model and document coordination
**Level 3 contract:** inherits M03.1 RACI and SLA; explicit input/output handoff: discipline submission → validate metadata/model information → resolve review issues → publish intended-use revision. Cross-functional links: BIM lead, Construction, Planning, Procurement, Operations, Maintenance; notify Commercial, Finance. Workflow WF03; controls: Release by revision and intended use; engineering authority sign-off. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M03.1.2.1** Discipline submission. Task contract inherits M03.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.2.2** Validate metadata/model information. Task contract inherits M03.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.2.3** Resolve review issues. Task contract inherits M03.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.2.4** Publish intended-use revision. Task contract inherits M03.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M03.1.3 Engineering change
**Level 3 contract:** inherits M03.1 RACI and SLA; explicit input/output handoff: changed specification → map affected objects/quantities → assess supply/plan/cost/asset impact → route approved change. Cross-functional links: BIM lead, Construction, Planning, Procurement, Operations, Maintenance; notify Commercial, Finance. Workflow WF03; controls: Release by revision and intended use; engineering authority sign-off. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M03.1.3.1** Changed specification. Task contract inherits M03.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.3.2** Map affected objects/quantities. Task contract inherits M03.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.3.3** Assess supply/plan/cost/asset impact. Task contract inherits M03.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M03.1.3.4** Route approved change. Task contract inherits M03.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M04 Planning and project controls
**Level 1 contract:** R Planning engineer; A Planning head; C Engineering, Construction, Procurement, Finance, Operations; I Project Director, Sales. Upstream: scope, quantities, constraints, contract dates. Downstream: baseline, lookahead, forecast, material dates. SLA: 2 business days for weekly update validation. Workflow: WF04. Governance: Keep baseline and forecast separate; evidence-based earning rules. Escalation: Planning head, then Project Director/sponsor for unresolved cross-functional issues.

### M04.1 Schedule and performance
**Level 2 contract:** inherits the full M04 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M04.1.1 Baseline planning
**Level 3 contract:** inherits M04.1 RACI and SLA; explicit input/output handoff: approved scope → create WBS and activity logic → review resources and interfaces → approve baseline. Cross-functional links: Engineering, Construction, Procurement, Finance, Operations; notify Project Director, Sales. Workflow WF04; controls: Keep baseline and forecast separate; evidence-based earning rules. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M04.1.1.1** Approved scope. Task contract inherits M04.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.1.2** Create wbs and activity logic. Task contract inherits M04.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.1.3** Review resources and interfaces. Task contract inherits M04.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.1.4** Approve baseline. Task contract inherits M04.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M04.1.2 Lookahead and constraints
**Level 3 contract:** inherits M04.1 RACI and SLA; explicit input/output handoff: current plan → identify design/material/access constraints → assign owners and dates → release ready packages. Cross-functional links: Engineering, Construction, Procurement, Finance, Operations; notify Project Director, Sales. Workflow WF04; controls: Keep baseline and forecast separate; evidence-based earning rules. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M04.1.2.1** Current plan. Task contract inherits M04.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.2.2** Identify design/material/access constraints. Task contract inherits M04.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.2.3** Assign owners and dates. Task contract inherits M04.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.2.4** Release ready packages. Task contract inherits M04.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M04.1.3 Progress and recovery
**Level 3 contract:** inherits M04.1 RACI and SLA; explicit input/output handoff: field evidence → validate earned quantities → update forecast and critical path → approve recovery actions. Cross-functional links: Engineering, Construction, Procurement, Finance, Operations; notify Project Director, Sales. Workflow WF04; controls: Keep baseline and forecast separate; evidence-based earning rules. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M04.1.3.1** Field evidence. Task contract inherits M04.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.3.2** Validate earned quantities. Task contract inherits M04.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.3.3** Update forecast and critical path. Task contract inherits M04.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M04.1.3.4** Approve recovery actions. Task contract inherits M04.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M05 Finance and treasury
**Level 1 contract:** R Finance analyst; A Finance head; C Planning, Commercial, Accounting, Sales, Operations; I Project Director. Upstream: budget basis, contract, plan, ledger actuals. Downstream: funding decisions, forecast, cash plan. SLA: 3 business days for complete budget/change review. Workflow: WF10. Governance: Authorised budget distinct from forecast and pending exposure. Escalation: Finance head, then Project Director/sponsor for unresolved cross-functional issues.

### M05.1 Funding and commercial outlook
**Level 2 contract:** inherits the full M05 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M05.1.1 Budget and funding
**Level 3 contract:** inherits M05.1 RACI and SLA; explicit input/output handoff: estimate and cash need → allocate cost codes/contingency → approve budget/funding → publish version. Cross-functional links: Planning, Commercial, Accounting, Sales, Operations; notify Project Director. Workflow WF10; controls: Authorised budget distinct from forecast and pending exposure. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M05.1.1.1** Estimate and cash need. Task contract inherits M05.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.1.2** Allocate cost codes/contingency. Task contract inherits M05.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.1.3** Approve budget/funding. Task contract inherits M05.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.1.4** Publish version. Task contract inherits M05.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M05.1.2 Forecast and variance
**Level 3 contract:** inherits M05.1 RACI and SLA; explicit input/output handoff: actual/accrual/commitment data → reconcile remaining cost → evaluate EAC and risks → approve forecast actions. Cross-functional links: Planning, Commercial, Accounting, Sales, Operations; notify Project Director. Workflow WF10; controls: Authorised budget distinct from forecast and pending exposure. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M05.1.2.1** Actual/accrual/commitment data. Task contract inherits M05.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.2.2** Reconcile remaining cost. Task contract inherits M05.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.2.3** Evaluate eac and risks. Task contract inherits M05.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.2.4** Approve forecast actions. Task contract inherits M05.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M05.1.3 Cash and collections planning
**Level 3 contract:** inherits M05.1 RACI and SLA; explicit input/output handoff: payment terms and milestones → forecast receipts/payments → review funding gaps → authorise treasury actions. Cross-functional links: Planning, Commercial, Accounting, Sales, Operations; notify Project Director. Workflow WF10; controls: Authorised budget distinct from forecast and pending exposure. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M05.1.3.1** Payment terms and milestones. Task contract inherits M05.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.3.2** Forecast receipts/payments. Task contract inherits M05.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.3.3** Review funding gaps. Task contract inherits M05.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M05.1.3.4** Authorise treasury actions. Task contract inherits M05.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M06 Accounting and financial close
**Level 1 contract:** R Project accountant; A Accounting head; C Finance, Commercial, Procurement, Operations; I Project Director. Upstream: accepted services/receipts, certifications, ERP policy. Downstream: posted books, ageing, close and capital records. SLA: 2 business days for a complete posting review. Workflow: WF05/WF06. Governance: Segregated posting/payment; approved accounting policy and locked periods. Escalation: Accounting head, then Project Director/sponsor for unresolved cross-functional issues.

### M06.1 Books and reconciliation
**Level 2 contract:** inherits the full M06 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M06.1.1 Payables and reconciliation
**Level 3 contract:** inherits M06.1 RACI and SLA; explicit input/output handoff: matched invoice → check coding/tax/period → post once to ERP → reconcile and resolve differences. Cross-functional links: Finance, Commercial, Procurement, Operations; notify Project Director. Workflow WF05/WF06; controls: Segregated posting/payment; approved accounting policy and locked periods. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M06.1.1.1** Matched invoice. Task contract inherits M06.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.1.2** Check coding/tax/period. Task contract inherits M06.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.1.3** Post once to erp. Task contract inherits M06.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.1.4** Reconcile and resolve differences. Task contract inherits M06.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M06.1.2 Receivables and revenue
**Level 3 contract:** inherits M06.1 RACI and SLA; explicit input/output handoff: approved billing basis → issue client invoice → apply policy and ledger entries → reconcile receipts/retention. Cross-functional links: Finance, Commercial, Procurement, Operations; notify Project Director. Workflow WF05/WF06; controls: Segregated posting/payment; approved accounting policy and locked periods. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M06.1.2.1** Approved billing basis. Task contract inherits M06.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.2.2** Issue client invoice. Task contract inherits M06.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.2.3** Apply policy and ledger entries. Task contract inherits M06.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.2.4** Reconcile receipts/retention. Task contract inherits M06.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M06.1.3 Close and asset accounting
**Level 3 contract:** inherits M06.1 RACI and SLA; explicit input/output handoff: period cutoff and asset acceptance → review accruals/capitalisation → approve close/reversals → publish reconciled records. Cross-functional links: Finance, Commercial, Procurement, Operations; notify Project Director. Workflow WF05/WF06; controls: Segregated posting/payment; approved accounting policy and locked periods. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M06.1.3.1** Period cutoff and asset acceptance. Task contract inherits M06.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.3.2** Review accruals/capitalisation. Task contract inherits M06.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.3.3** Approve close/reversals. Task contract inherits M06.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M06.1.3.4** Publish reconciled records. Task contract inherits M06.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M07 BOQ and cost engineering
**Level 1 contract:** R Quantity surveyor; A Cost engineering head; C Engineering, Planning, Procurement, Commercial, Finance; I Construction, Accounting. Upstream: approved drawings/model/specifications. Downstream: quantity baseline, estimates, demand and measurement rules. SLA: 3 business days for complete BOQ revision review. Workflow: WF03/WF10. Governance: Model quantity is not automatically payable or purchased quantity. Escalation: Cost engineering head, then Project Director/sponsor for unresolved cross-functional issues.

### M07.1 Quantities rates and cost allocation
**Level 2 contract:** inherits the full M07 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M07.1.1 Quantity baseline
**Level 3 contract:** inherits M07.1 RACI and SLA; explicit input/output handoff: released design → measure and record basis → review units/allocations → approve BOQ revision. Cross-functional links: Engineering, Planning, Procurement, Commercial, Finance; notify Construction, Accounting. Workflow WF03/WF10; controls: Model quantity is not automatically payable or purchased quantity. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M07.1.1.1** Released design. Task contract inherits M07.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.1.2** Measure and record basis. Task contract inherits M07.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.1.3** Review units/allocations. Task contract inherits M07.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.1.4** Approve boq revision. Task contract inherits M07.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M07.1.2 Rate and estimate library
**Level 3 contract:** inherits M07.1 RACI and SLA; explicit input/output handoff: qualified historical rates → normalise date/location/unit → review assumptions and allowances → publish estimate basis. Cross-functional links: Engineering, Planning, Procurement, Commercial, Finance; notify Construction, Accounting. Workflow WF03/WF10; controls: Model quantity is not automatically payable or purchased quantity. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M07.1.2.1** Qualified historical rates. Task contract inherits M07.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.2.2** Normalise date/location/unit. Task contract inherits M07.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.2.3** Review assumptions and allowances. Task contract inherits M07.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.2.4** Publish estimate basis. Task contract inherits M07.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M07.1.3 Quantity change and reconciliation
**Level 3 contract:** inherits M07.1 RACI and SLA; explicit input/output handoff: revision or field measure → compare original/current/installed quantities → review entitlement and cost → approve controlled adjustment. Cross-functional links: Engineering, Planning, Procurement, Commercial, Finance; notify Construction, Accounting. Workflow WF03/WF10; controls: Model quantity is not automatically payable or purchased quantity. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M07.1.3.1** Revision or field measure. Task contract inherits M07.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.3.2** Compare original/current/installed quantities. Task contract inherits M07.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.3.3** Review entitlement and cost. Task contract inherits M07.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M07.1.3.4** Approve controlled adjustment. Task contract inherits M07.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M08 Procurement and suppliers
**Level 1 contract:** R Procurement buyer; A Procurement head; C Engineering, Stores, Planning, Finance, Legal; I Construction, Accounting. Upstream: approved demand, technical specification, budget. Downstream: awarded order, supply dates, commitment. SLA: 3 business days for complete PR sourcing disposition. Workflow: WF05. Governance: Technical/commercial reviews and authority limits; disclose conflicts. Escalation: Procurement head, then Project Director/sponsor for unresolved cross-functional issues.

### M08.1 Source and contract supply
**Level 2 contract:** inherits the full M08 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M08.1.1 PR and sourcing
**Level 3 contract:** inherits M08.1 RACI and SLA; explicit input/output handoff: dated demand → check stock/budget/specification → approve PR and sourcing route → issue RFQ. Cross-functional links: Engineering, Stores, Planning, Finance, Legal; notify Construction, Accounting. Workflow WF05; controls: Technical/commercial reviews and authority limits; disclose conflicts. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M08.1.1.1** Dated demand. Task contract inherits M08.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.1.2** Check stock/budget/specification. Task contract inherits M08.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.1.3** Approve pr and sourcing route. Task contract inherits M08.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.1.4** Issue rfq. Task contract inherits M08.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M08.1.2 Evaluation and order
**Level 3 contract:** inherits M08.1 RACI and SLA; explicit input/output handoff: supplier responses → evaluate compliance and commercial terms → approve award → issue PO/contract. Cross-functional links: Engineering, Stores, Planning, Finance, Legal; notify Construction, Accounting. Workflow WF05; controls: Technical/commercial reviews and authority limits; disclose conflicts. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M08.1.2.1** Supplier responses. Task contract inherits M08.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.2.2** Evaluate compliance and commercial terms. Task contract inherits M08.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.2.3** Approve award. Task contract inherits M08.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.2.4** Issue po/contract. Task contract inherits M08.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M08.1.3 Expediting and amendments
**Level 3 contract:** inherits M08.1 RACI and SLA; explicit input/output handoff: supplier confirmation/change → assess delivery and cost impacts → approve remedy/amendment → update stakeholders. Cross-functional links: Engineering, Stores, Planning, Finance, Legal; notify Construction, Accounting. Workflow WF05; controls: Technical/commercial reviews and authority limits; disclose conflicts. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M08.1.3.1** Supplier confirmation/change. Task contract inherits M08.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.3.2** Assess delivery and cost impacts. Task contract inherits M08.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.3.3** Approve remedy/amendment. Task contract inherits M08.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M08.1.3.4** Update stakeholders. Task contract inherits M08.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M09 Stores and logistics
**Level 1 contract:** R Stores officer; A Stores manager; C Procurement, QHSE, Construction, Maintenance; I Planning, Accounting. Upstream: order, shipping evidence, stock demand. Downstream: accepted stock, issues, returns and valuation feed. SLA: 1 business day for routine receipt recording. Workflow: WF05. Governance: Quarantine excluded from usable stock; approved adjustments and traceable movements. Escalation: Stores manager, then Project Director/sponsor for unresolved cross-functional issues.

### M09.1 Physical materials control
**Level 2 contract:** inherits the full M09 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M09.1.1 Receipt and inspection routing
**Level 3 contract:** inherits M09.1 RACI and SLA; explicit input/output handoff: delivery → count and record batch/serial → inspect and segregate → accept or reject. Cross-functional links: Procurement, QHSE, Construction, Maintenance; notify Planning, Accounting. Workflow WF05; controls: Quarantine excluded from usable stock; approved adjustments and traceable movements. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M09.1.1.1** Delivery. Task contract inherits M09.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.1.2** Count and record batch/serial. Task contract inherits M09.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.1.3** Inspect and segregate. Task contract inherits M09.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.1.4** Accept or reject. Task contract inherits M09.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M09.1.2 Reservation and issue
**Level 3 contract:** inherits M09.1 RACI and SLA; explicit input/output handoff: work demand → reserve accepted stock → approve and record issue → confirm receiving package/asset. Cross-functional links: Procurement, QHSE, Construction, Maintenance; notify Planning, Accounting. Workflow WF05; controls: Quarantine excluded from usable stock; approved adjustments and traceable movements. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M09.1.2.1** Work demand. Task contract inherits M09.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.2.2** Reserve accepted stock. Task contract inherits M09.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.2.3** Approve and record issue. Task contract inherits M09.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.2.4** Confirm receiving package/asset. Task contract inherits M09.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M09.1.3 Return transfer and count
**Level 3 contract:** inherits M09.1 RACI and SLA; explicit input/output handoff: return/transfer/count event → validate condition and quantities → approve adjustment → reconcile stock and cost. Cross-functional links: Procurement, QHSE, Construction, Maintenance; notify Planning, Accounting. Workflow WF05; controls: Quarantine excluded from usable stock; approved adjustments and traceable movements. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M09.1.3.1** Return/transfer/count event. Task contract inherits M09.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.3.2** Validate condition and quantities. Task contract inherits M09.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.3.3** Approve adjustment. Task contract inherits M09.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M09.1.3.4** Reconcile stock and cost. Task contract inherits M09.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M10 Construction and field delivery
**Level 1 contract:** R Site engineer; A Construction manager; C Planning, Engineering, Procurement, QHSE; I Commercial, Finance, Operations. Upstream: released design, ready package, permits and materials. Downstream: verified progress, measurements, installed asset records. SLA: 1 business day for routine daily-report validation. Workflow: WF04/WF06. Governance: Safety/quality holds and current work revision checked before execution. Escalation: Construction manager, then Project Director/sponsor for unresolved cross-functional issues.

### M10.1 Work packages and measurement
**Level 2 contract:** inherits the full M10 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M10.1.1 Work readiness and execution
**Level 3 contract:** inherits M10.1 RACI and SLA; explicit input/output handoff: lookahead package → verify prerequisites → execute authorised work → capture daily evidence. Cross-functional links: Planning, Engineering, Procurement, QHSE; notify Commercial, Finance, Operations. Workflow WF04/WF06; controls: Safety/quality holds and current work revision checked before execution. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M10.1.1.1** Lookahead package. Task contract inherits M10.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.1.2** Verify prerequisites. Task contract inherits M10.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.1.3** Execute authorised work. Task contract inherits M10.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.1.4** Capture daily evidence. Task contract inherits M10.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M10.1.2 Measurement and installation
**Level 3 contract:** inherits M10.1 RACI and SLA; explicit input/output handoff: completed work → measure and tag installation → obtain inspection acceptance → submit progress/client measure. Cross-functional links: Planning, Engineering, Procurement, QHSE; notify Commercial, Finance, Operations. Workflow WF04/WF06; controls: Safety/quality holds and current work revision checked before execution. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M10.1.2.1** Completed work. Task contract inherits M10.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.2.2** Measure and tag installation. Task contract inherits M10.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.2.3** Obtain inspection acceptance. Task contract inherits M10.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.2.4** Submit progress/client measure. Task contract inherits M10.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M10.1.3 Site issue and rework
**Level 3 contract:** inherits M10.1 RACI and SLA; explicit input/output handoff: site deviation → hold and raise RFI/NCR → receive controlled disposition → execute and verify rectification. Cross-functional links: Planning, Engineering, Procurement, QHSE; notify Commercial, Finance, Operations. Workflow WF04/WF06; controls: Safety/quality holds and current work revision checked before execution. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M10.1.3.1** Site deviation. Task contract inherits M10.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.3.2** Hold and raise rfi/ncr. Task contract inherits M10.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.3.3** Receive controlled disposition. Task contract inherits M10.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M10.1.3.4** Execute and verify rectification. Task contract inherits M10.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M11 Commercial contracts and tendering
**Level 1 contract:** R Contracts manager; A Commercial head; C Sales, Legal, Planning, Engineering, Finance; I Project Director, Accounting. Upstream: client tender/contract, approved measurements, change notices. Downstream: contract obligations, certification, variation and settlement. SLA: 2 business days for complete internal notice assessment; contractual deadlines override. Workflow: WF01/WF06/WF10. Governance: Clause-linked deadlines; client approval distinct from internal approval. Escalation: Commercial head, then Project Director/sponsor for unresolved cross-functional issues.

### M11.1 Entitlement and obligations
**Level 2 contract:** inherits the full M11 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M11.1.1 Contract and tender governance
**Level 3 contract:** inherits M11.1 RACI and SLA; explicit input/output handoff: tender/award draft → assess clauses and risk → approve positions/authority → publish obligation register. Cross-functional links: Sales, Legal, Planning, Engineering, Finance; notify Project Director, Accounting. Workflow WF01/WF06/WF10; controls: Clause-linked deadlines; client approval distinct from internal approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M11.1.1.1** Tender/award draft. Task contract inherits M11.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.1.2** Assess clauses and risk. Task contract inherits M11.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.1.3** Approve positions/authority. Task contract inherits M11.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.1.4** Publish obligation register. Task contract inherits M11.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M11.1.2 Certification and claims
**Level 3 contract:** inherits M11.1 RACI and SLA; explicit input/output handoff: measured eligible work/change → assemble evidence and notices → seek client certification → resolve disputes. Cross-functional links: Sales, Legal, Planning, Engineering, Finance; notify Project Director, Accounting. Workflow WF01/WF06/WF10; controls: Clause-linked deadlines; client approval distinct from internal approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M11.1.2.1** Measured eligible work/change. Task contract inherits M11.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.2.2** Assemble evidence and notices. Task contract inherits M11.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.2.3** Seek client certification. Task contract inherits M11.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.2.4** Resolve disputes. Task contract inherits M11.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M11.1.3 Final account and service terms
**Level 3 contract:** inherits M11.1 RACI and SLA; explicit input/output handoff: accepted deliverables and changes → reconcile retention/claims → approve settlement/service obligations → track closure and renewal. Cross-functional links: Sales, Legal, Planning, Engineering, Finance; notify Project Director, Accounting. Workflow WF01/WF06/WF10; controls: Clause-linked deadlines; client approval distinct from internal approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M11.1.3.1** Accepted deliverables and changes. Task contract inherits M11.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.3.2** Reconcile retention/claims. Task contract inherits M11.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.3.3** Approve settlement/service obligations. Task contract inherits M11.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M11.1.3.4** Track closure and renewal. Task contract inherits M11.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M12 QHSE and regulatory compliance
**Level 1 contract:** R QHSE officer; A QHSE head; C Engineering, Construction, Operations, Maintenance, Legal; I Project Director, Planning. Upstream: inspection plans, hazards, permits, obligations. Downstream: holds, accepted tests, actions and compliance evidence. SLA: Immediate emergency response per site plan; routine review 1 business day. Workflow: WF00. Governance: Critical holds cannot be overridden by commercial or AI approval. Escalation: QHSE head, then Project Director/sponsor for unresolved cross-functional issues.

### M12.1 Quality safety and compliance assurance
**Level 2 contract:** inherits the full M12 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M12.1.1 Inspection and nonconformance
**Level 3 contract:** inherits M12.1 RACI and SLA; explicit input/output handoff: inspection trigger → verify criteria and evidence → accept or raise NCR/hold → verify corrective closure. Cross-functional links: Engineering, Construction, Operations, Maintenance, Legal; notify Project Director, Planning. Workflow WF00; controls: Critical holds cannot be overridden by commercial or AI approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M12.1.1.1** Inspection trigger. Task contract inherits M12.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.1.2** Verify criteria and evidence. Task contract inherits M12.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.1.3** Accept or raise ncr/hold. Task contract inherits M12.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.1.4** Verify corrective closure. Task contract inherits M12.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M12.1.2 Safety and permits
**Level 3 contract:** inherits M12.1 RACI and SLA; explicit input/output handoff: work hazard → assess competence/isolation/permit requirements → authorise under site procedure → monitor and close safely. Cross-functional links: Engineering, Construction, Operations, Maintenance, Legal; notify Project Director, Planning. Workflow WF00; controls: Critical holds cannot be overridden by commercial or AI approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M12.1.2.1** Work hazard. Task contract inherits M12.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.2.2** Assess competence/isolation/permit requirements. Task contract inherits M12.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.2.3** Authorise under site procedure. Task contract inherits M12.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.2.4** Monitor and close safely. Task contract inherits M12.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M12.1.3 Compliance and sustainability
**Level 3 contract:** inherits M12.1 RACI and SLA; explicit input/output handoff: applicable obligation → assign evidence and renewal dates → verify reporting → escalate overdue or noncompliant status. Cross-functional links: Engineering, Construction, Operations, Maintenance, Legal; notify Project Director, Planning. Workflow WF00; controls: Critical holds cannot be overridden by commercial or AI approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M12.1.3.1** Applicable obligation. Task contract inherits M12.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.3.2** Assign evidence and renewal dates. Task contract inherits M12.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.3.3** Verify reporting. Task contract inherits M12.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M12.1.3.4** Escalate overdue or noncompliant status. Task contract inherits M12.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M13 Commissioning and handover
**Level 1 contract:** R Commissioning engineer; A Commissioning manager; C Engineering, QHSE, Operations, Maintenance, Commercial, Accounting; I Sales, Project Director. Upstream: installed system, design requirements, tests and asset data. Downstream: tested system, acceptance package, asset custody. SLA: 3 business days for complete readiness review. Workflow: WF07. Governance: Operations acceptance is a separate decision; failed critical tests block release. Escalation: Commissioning manager, then Project Director/sponsor for unresolved cross-functional issues.

### M13.1 Proof of operational readiness
**Level 2 contract:** inherits the full M13 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M13.1.1 Readiness and testing
**Level 3 contract:** inherits M13.1 RACI and SLA; explicit input/output handoff: system completion → verify prerequisites and permits → execute witnessed tests → resolve failures/punch items. Cross-functional links: Engineering, QHSE, Operations, Maintenance, Commercial, Accounting; notify Sales, Project Director. Workflow WF07; controls: Operations acceptance is a separate decision; failed critical tests block release. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M13.1.1.1** System completion. Task contract inherits M13.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.1.2** Verify prerequisites and permits. Task contract inherits M13.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.1.3** Execute witnessed tests. Task contract inherits M13.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.1.4** Resolve failures/punch items. Task contract inherits M13.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M13.1.2 Asset information and training
**Level 3 contract:** inherits M13.1 RACI and SLA; explicit input/output handoff: approved asset requirements → validate tags/manuals/spares/warranty → deliver operator training → verify complete pack. Cross-functional links: Engineering, QHSE, Operations, Maintenance, Commercial, Accounting; notify Sales, Project Director. Workflow WF07; controls: Operations acceptance is a separate decision; failed critical tests block release. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M13.1.2.1** Approved asset requirements. Task contract inherits M13.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.2.2** Validate tags/manuals/spares/warranty. Task contract inherits M13.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.2.3** Deliver operator training. Task contract inherits M13.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.2.4** Verify complete pack. Task contract inherits M13.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M13.1.3 Custody and acceptance
**Level 3 contract:** inherits M13.1 RACI and SLA; explicit input/output handoff: tested system and pack → obtain distinct operational/client approvals → transfer asset data and custody → track residual duties. Cross-functional links: Engineering, QHSE, Operations, Maintenance, Commercial, Accounting; notify Sales, Project Director. Workflow WF07; controls: Operations acceptance is a separate decision; failed critical tests block release. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M13.1.3.1** Tested system and pack. Task contract inherits M13.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.3.2** Obtain distinct operational/client approvals. Task contract inherits M13.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.3.3** Transfer asset data and custody. Task contract inherits M13.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M13.1.3.4** Track residual duties. Task contract inherits M13.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M14 Operations and service delivery
**Level 1 contract:** R Operations supervisor; A Operations head; C Maintenance, QHSE, Planning, Finance, Commercial; I Sales, Asset owner. Upstream: accepted assets, service contract, operating limits. Downstream: service logs, shutdown needs, downtime and service billing basis. SLA: Critical event triage proposed within 15 elapsed minutes; site emergency plan takes precedence. Workflow: WF08. Governance: Operating authority controls availability and return to service. Escalation: Operations head, then Project Director/sponsor for unresolved cross-functional issues.

### M14.1 Safe service performance
**Level 2 contract:** inherits the full M14 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M14.1.1 Shift and service operations
**Level 3 contract:** inherits M14.1 RACI and SLA; explicit input/output handoff: accepted operating scope → perform checks and handover → record output/service evidence → review performance. Cross-functional links: Maintenance, QHSE, Planning, Finance, Commercial; notify Sales, Asset owner. Workflow WF08; controls: Operating authority controls availability and return to service. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M14.1.1.1** Accepted operating scope. Task contract inherits M14.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.1.2** Perform checks and handover. Task contract inherits M14.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.1.3** Record output/service evidence. Task contract inherits M14.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.1.4** Review performance. Task contract inherits M14.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M14.1.2 Event and shutdown coordination
**Level 3 contract:** inherits M14.1 RACI and SLA; explicit input/output handoff: alarm/incident/request → triage service impact → coordinate safe isolation/shutdown → authorise restoration after proof. Cross-functional links: Maintenance, QHSE, Planning, Finance, Commercial; notify Sales, Asset owner. Workflow WF08; controls: Operating authority controls availability and return to service. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M14.1.2.1** Alarm/incident/request. Task contract inherits M14.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.2.2** Triage service impact. Task contract inherits M14.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.2.3** Coordinate safe isolation/shutdown. Task contract inherits M14.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.2.4** Authorise restoration after proof. Task contract inherits M14.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M14.1.3 Service economics and obligations
**Level 3 contract:** inherits M14.1 RACI and SLA; explicit input/output handoff: operating logs and terms → verify SLA outcomes/costs → assess deductions or billing eligibility → inform Finance/Commercial/Sales. Cross-functional links: Maintenance, QHSE, Planning, Finance, Commercial; notify Sales, Asset owner. Workflow WF08; controls: Operating authority controls availability and return to service. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M14.1.3.1** Operating logs and terms. Task contract inherits M14.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.3.2** Verify sla outcomes/costs. Task contract inherits M14.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.3.3** Assess deductions or billing eligibility. Task contract inherits M14.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M14.1.3.4** Inform finance/commercial/sales. Task contract inherits M14.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M15 Maintenance and asset reliability
**Level 1 contract:** R Maintenance planner; A Maintenance head; C Operations, QHSE, Stores, Procurement, Engineering, Finance; I Asset owner, Commercial. Upstream: asset criticality, manuals, readings, defects. Downstream: work orders, reliable assets, cost/failure history and warranty claims. SLA: Critical work triage proposed within 30 elapsed minutes; statutory/site requirements override. Workflow: WF08/WF09. Governance: No automatic statutory deferral or return-to-service approval. Escalation: Maintenance head, then Project Director/sponsor for unresolved cross-functional issues.

### M15.1 Asset care and reliability
**Level 2 contract:** inherits the full M15 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M15.1.1 Preventive maintenance
**Level 3 contract:** inherits M15.1 RACI and SLA; explicit input/output handoff: asset/manual/obligation → approve task and interval → generate due work once → verify compliance or authorised deferral. Cross-functional links: Operations, QHSE, Stores, Procurement, Engineering, Finance; notify Asset owner, Commercial. Workflow WF08/WF09; controls: No automatic statutory deferral or return-to-service approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M15.1.1.1** Asset/manual/obligation. Task contract inherits M15.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.1.2** Approve task and interval. Task contract inherits M15.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.1.3** Generate due work once. Task contract inherits M15.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.1.4** Verify compliance or authorised deferral. Task contract inherits M15.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M15.1.2 Corrective maintenance
**Level 3 contract:** inherits M15.1 RACI and SLA; explicit input/output handoff: fault and isolation needs → plan labour/spares/permits → execute and test → obtain return-to-service and close costs. Cross-functional links: Operations, QHSE, Stores, Procurement, Engineering, Finance; notify Asset owner, Commercial. Workflow WF08/WF09; controls: No automatic statutory deferral or return-to-service approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M15.1.2.1** Fault and isolation needs. Task contract inherits M15.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.2.2** Plan labour/spares/permits. Task contract inherits M15.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.2.3** Execute and test. Task contract inherits M15.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.2.4** Obtain return-to-service and close costs. Task contract inherits M15.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M15.1.3 Reliability warranty and renewal
**Level 3 contract:** inherits M15.1 RACI and SLA; explicit input/output handoff: failure/condition/cost history → analyse repeat problems and warranty → approve remedial or replacement case → feed design/service renewal. Cross-functional links: Operations, QHSE, Stores, Procurement, Engineering, Finance; notify Asset owner, Commercial. Workflow WF08/WF09; controls: No automatic statutory deferral or return-to-service approval. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M15.1.3.1** Failure/condition/cost history. Task contract inherits M15.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.3.2** Analyse repeat problems and warranty. Task contract inherits M15.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.3.3** Approve remedial or replacement case. Task contract inherits M15.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M15.1.3.4** Feed design/service renewal. Task contract inherits M15.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M16 Enterprise governance and enablement
**Level 1 contract:** R PMO/data steward; A Transformation sponsor; C All domain heads, IT, Legal, Security; I Executive committee. Upstream: business policies, system data, risks and decisions. Downstream: controlled templates, access, audit, reporting and trained users. SLA: 2 business days for routine complete governance request. Workflow: WF00. Governance: Versioned policy and least privilege; named business owners for data. Escalation: Transformation sponsor, then Project Director/sponsor for unresolved cross-functional issues.

### M16.1 Data platform people and assurance
**Level 2 contract:** inherits the full M16 RACI, SLA, upstream/downstream dependencies, workflow and controls. Capability owner validates handoffs across its processes; transaction approval authority remains separately configured.


#### M16.1.1 Process and authority management
**Level 3 contract:** inherits M16.1 RACI and SLA; explicit input/output handoff: policy need → map process/RACI/SLAs → approve authority and version → activate templates and train users. Cross-functional links: All domain heads, IT, Legal, Security; notify Executive committee. Workflow WF00; controls: Versioned policy and least privilege; named business owners for data. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M16.1.1.1** Policy need. Task contract inherits M16.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.1.2** Map process/raci/slas. Task contract inherits M16.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.1.3** Approve authority and version. Task contract inherits M16.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.1.4** Activate templates and train users. Task contract inherits M16.1.1 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M16.1.2 Data integration and intelligence
**Level 3 contract:** inherits M16.1 RACI and SLA; explicit input/output handoff: source event/request → validate ownership/access/quality → sync or generate reviewed insight → reconcile and monitor. Cross-functional links: All domain heads, IT, Legal, Security; notify Executive committee. Workflow WF00; controls: Versioned policy and least privilege; named business owners for data. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M16.1.2.1** Source event/request. Task contract inherits M16.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.2.2** Validate ownership/access/quality. Task contract inherits M16.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.2.3** Sync or generate reviewed insight. Task contract inherits M16.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.2.4** Reconcile and monitor. Task contract inherits M16.1.2 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


#### M16.1.3 Assurance and continuous improvement
**Level 3 contract:** inherits M16.1 RACI and SLA; explicit input/output handoff: audit/metric/feedback → investigate exceptions and root causes → approve corrective change → verify benefits and adoption. Cross-functional links: All domain heads, IT, Legal, Security; notify Executive committee. Workflow WF00; controls: Versioned policy and least privilege; named business owners for data. Rejection returns to the prior responsible step with reason/evidence; blocked work enters the owner's exception queue. Measure active review time, total age and overdue exceptions.

- **M16.1.3.1** Audit/metric/feedback. Task contract inherits M16.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.3.2** Investigate exceptions and root causes. Task contract inherits M16.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.3.3** Approve corrective change. Task contract inherits M16.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.

- **M16.1.3.4** Verify benefits and adoption. Task contract inherits M16.1.3 dependencies, RACI, SLA envelope, workflow, evidence and controls. Assign a named executor and due date; approval actions must use the designated independent authority.


## M17 Marketing

**Level 1 contract:** R Marketing executive; A Marketing head; C Sales, Commercial, Finance, Legal/Compliance; I management and Project Director where project references are involved. Upstream: approved market strategy, campaign budget, contact provenance/preferences, client permissions and verified project/service outcomes. Downstream: qualified leads to M01, approved references, attributed campaign costs to M05/M06. Workflow WF11 and WF00. Proposed SLA: complete internal lead handoff within 1 business day; content/reference review within 3 business days. Governance: spending authority, contact preferences, restricted client information, evidence-backed claims and approval before publication. Escalation: Marketing head, then sponsor for cross-functional disputes. Shared controls and task inheritance at the start of this catalog apply.

### M17.1 Demand generation and approved market communication

**Level 2 contract:** inherits the complete M17 RACI, dependencies, SLAs, workflow and controls. Marketing owns campaigns and content; Sales owns opportunity acceptance; Finance owns spending authority. Task-specific due dates fit within the applicable process SLA.

#### M17.1.1 Campaign planning and lead handoff

**Level 3 contract:** inherits M17.1; upstream strategy, approved audience/contact basis and budget; downstream reviewed lead/source to M01 and campaign costs to M05/M06. Workflow WF11; lead handoff SLA 1 business day after complete qualification. Reject incomplete or duplicate submissions with reason; record source attribution without duplicating opportunity value. Measure accepted leads and source conversion.

- **M17.1.1.1** Define campaign purpose, audience, channel and budget; inherit M17.1.1 RACI, dependencies, controls and SLA envelope; assign named executor/due date.
- **M17.1.1.2** Obtain independent spending/content/contact checks before launch; inherit M17.1.1 contract; approval executor is the designated authority.
- **M17.1.1.3** Capture lead provenance and preferences; deduplicate with review; inherit M17.1.1 contract and evidence requirements.
- **M17.1.1.4** Route to named Sales owner; record acceptance/return and outcome linkage; inherit M17.1.1 contract and escalation.

#### M17.1.2 Project references and content approval

**Level 3 contract:** inherits M17.1; upstream verified project/service evidence from M10/M14/M15 and permission from M11/Legal/client as required; downstream approved versioned content. Workflow WF00/WF11; review SLA 3 business days for complete internal submission, external consent timeline tracked separately. No approval by silence. Measure turnaround and unresolved permission issues.

- **M17.1.2.1** Assemble evidence and proposed content; inherit M17.1.2 contract; record source and revision.
- **M17.1.2.2** Review technical/commercial claims and client permission; inherit M17.1.2 contract; reviewers use designated independent authority.
- **M17.1.2.3** Publish only the approved version/channel after authorisation; inherit M17.1.2 contract; retain publication reference.
- **M17.1.2.4** Track expiry, withdrawal or changed claims; inherit M17.1.2 contract and exception escalation.

#### M17.1.3 Attribution and service campaigns

**Level 3 contract:** inherits M17.1; upstream campaign costs, sales outcomes and approved service-expiry/renewal context; downstream reviewed attribution and proposed service campaign to M01. Workflow WF11/WF12; complete internal campaign proposal review SLA 3 business days. Differentiate sourced/influenced value; Accounting remains revenue authority. Measure accepted renewal leads and campaign cost basis.

- **M17.1.3.1** Link costs and opportunity outcomes with source lineage; inherit M17.1.3 contract and access controls.
- **M17.1.3.2** Reconcile attribution and prevent double counting; inherit M17.1.3 contract; Finance/Accounting validate financial measures.
- **M17.1.3.3** Prepare relevant service/renewal campaign with Operations/Maintenance input; inherit M17.1.3 contract; no unapproved service promises.
- **M17.1.3.4** Approve permitted outreach and return results to Sales; inherit M17.1.3 contract and publication/contact checks.
