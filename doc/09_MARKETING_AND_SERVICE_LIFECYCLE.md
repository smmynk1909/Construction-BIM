# Marketing and service lifecycle requirements

Version 0.2 | 27 October 2026

## 1 Scope and traceability

This addendum explicitly includes Marketing alongside Sales, Operations and Maintenance. It extends the original BRD/PRD/functionality without replacing their controls. M01 owns sales/customer relationships; new M17 owns marketing processes; M14 owns operation/service delivery; M15 owns maintenance. M11 owns contractual obligations and M05/M06 own financial control and accounting.

- **BR13 Marketing accountability:** trace approved campaigns and references to leads, opportunities and outcomes with cost, attribution and applicable contact preferences.
- **PR16 Marketing core:** campaign/source, lead handoff, duplicate review, contact preference and content/reference approval.
- **PR17 Sales continuity:** qualification, bid decision, approved contract handoff, client actions, collection coordination and renewal opportunities.
- **PR18 Operating service:** custody, shift/service records, incidents, shutdown coordination, downtime and contractual service evidence.
- **PR19 Maintainability and reliability:** design-stage maintenance requirements, preventive/corrective work, spares, tests, warranty and return-to-service decisions.

PR17–PR19 elaborate existing PR03/09/10/11; they do not add duplicate system masters. PR16 core and a thin sample of each journey belong in Pilot A; campaign automation, advanced attribution and service analytics follow in Release B. All targets and roles remain proposed.

## 2 Marketing workflow WF11

**Capture:** campaign ID, sector/geography, target account, channel/source, approved content version, budget/actual cost, contact provenance/preferences, lead, qualification result and attribution links. Separate sourced and influenced opportunity value to prevent double counting.

**Flow:** Draft campaign → approval → launch through authorised channels → capture and deduplicate lead → review qualification → Sales accepts or returns with reason → track outcome. Publication and outbound communications require the configured marketing authority and applicable contact permissions.

**Governance:** R Marketing executive; A Marketing head; C Sales, Finance, Legal/Compliance; I management. Complete lead handoff proposed within 1 business day; escalation to Marketing head, then Sales head for stalled acceptance. Finance owns spending authority. Lead contact data follows the approved privacy/retention policy.

**Metrics:** accepted leads, cost per accepted lead, sourced conversion and approved-reference turnaround. Contract value and recognised revenue remain Finance/Accounting-controlled measures.

## 3 Sales and customer workflow WF12

**Capture:** account/contact, opportunity, qualification, bid decision, cost/price assumptions, scope/exclusions, technical and service commitments, contract, customer actions, dispute, renewal and loss reason.

**Flow:** Qualified lead → Sales acceptance → bid/no-bid → approved proposal → negotiation → executed award → delivery handoff → customer review → renewal or close.

**Governance:** R Sales executive; A Sales head; C Engineering, Planning, Commercial, Finance, Operations, Maintenance; I Project Director. Proposed complete internal qualification decision within 2 business days. Delivery commitments require the responsible technical/operating reviews; contract authority remains separate from sales ownership.

**Metrics:** bid conversion, margin movement at award, aged customer actions and service-renewal rate. Pipeline probability is not booked revenue.

## 4 Operations workflow WF13

**Capture:** accepted system/asset, operating custodian, operating limits, shift log, output/service evidence, incident, downtime intervals, shutdown plan, SLA result and corrective action.

**Flow:** Readiness review → accepted custody → operate and inspect → record service/event → triage → coordinate maintenance/shutdown → verify recovery → authorised restoration → review service performance.

**Governance:** R Operations supervisor; A Operations head; C Maintenance, QHSE, Engineering, Planning, Commercial, Finance; I Sales and asset owner. Critical-event triage proposed within 15 elapsed minutes; site emergency procedures take precedence. Software alerts do not substitute for emergency response. Return to service requires explicit operating authority.

**Metrics:** service availability with defined exclusions, downtime by cause, operating cost, aged operating risks and contract SLA compliance. Service deductions require contractual review.

## 5 Maintenance workflow WF14

**Capture:** asset criticality, approved task plan, interval/meter trigger, work request/order, failure code, labour, spares, isolation/permit references, test results, warranty and repair/replacement recommendation.

**Flow:** Approved preventive trigger or fault → triage → plan labour/spares/window → verify prerequisites → execute → inspect/test → Operations authorises return → close and reconcile cost → reliability review.

**Governance:** R Maintenance planner/supervisor; A Maintenance head; C Operations, QHSE, Stores, Procurement, Engineering, Finance; I asset owner and Commercial. Critical-work triage proposed within 30 elapsed minutes; statutory/site requirements override. Deferrals need designated risk authority. Failure of a required test prevents restoration and closure.

**Metrics:** preventive completion by due date, repair duration with explicit start/stop basis, repeat failures, spare availability and warranty recoveries. No sensor feed is interpreted as healthy condition.

## 6 Shared record boundaries and agent opportunities

A campaign links to lead/account/opportunity; the opportunity links to executed contract and owned obligations. The project creates accepted systems/assets; service contracts link those assets to commercial obligations, operating events, maintenance costs and renewal opportunities. Customer complaints link to a delivery defect, incident or work order.

Agents may suggest duplicate leads, draft reviewed content, assemble bid evidence, extract proposed obligations, summarise shift events, prepare work orders, check spares and flag renewals. They must not invent performance claims, launch unapproved outreach, commit delivery promises, override maintenance/safety holds or publish client information without the required authorisation.

## 7 Acceptance scenarios

- **AT14 [BR13/PR16/WF11]:** repeated lead imports preserve one identity plus reviewable source links; an opted-out contact is excluded from applicable outbound campaigns.
- **AT15 [BR08/PR17/WF12]:** an unsupported promised service response is flagged for Operations/Maintenance review before proposal approval.
- **AT16 [BR09/PR18/WF13]:** missing mandatory commissioning evidence blocks custody transfer; availability starts only on the agreed operating basis.
- **AT17 [BR10/PR19/WF14]:** failed functional test keeps the asset unavailable and work open; labour/spares and failure history survive rework.
- **AT18 [BR08/PR17]:** service expiry generates a renewal task; no signed contract means no new backlog or revenue.
- **AT19 [BR13/PR16]:** a completed project becomes a marketing-reference candidate; publication remains blocked until required client consent and content approval exist.
- **AT20 [BR03/PR18/19]:** operating and maintenance costs reconcile to ledger references without counting stores issues and ERP actuals twice.

## 8 Supporting documents

Use the [solution map](08_SOLUTION_MAP.md) for module placement, the [functional specification](03_FUNCTIONAL_SPECIFICATION.md) for shared state/control rules, and the [catalog](04_MODULE_AND_GOVERNANCE_CATALOG.md) for process ownership. WF11–WF14 specialise WF00/01/07/08/09; they do not relax inherited controls.
