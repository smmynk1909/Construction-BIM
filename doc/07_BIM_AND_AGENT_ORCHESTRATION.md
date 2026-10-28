# BIM components and agent orchestration opportunities

Construction lifecycle platform  
Version 0.1 | 27 October 2026

## Purpose

Explain what Building Information Modelling consists of, how it connects to construction business processes, and where agents can coordinate work and support optimisation. This document complements the BRD, PRD, functional specification and governance catalog already prepared for the platform.

BIM is a way of creating, coordinating and maintaining reliable information about a built asset throughout its life. The 3D model is one part. Drawings, specifications, equipment data, review decisions and operating information are also involved. This broader interpretation is reflected in the [NATSPEC National BIM Guide](https://bim.natspec.org/images/NATSPEC_Documents/NATSPEC_National_BIM_Guide_2022-10_Web.pdf).

For the application, distinguish three connected layers:

1. **BIM information:** models, properties, relationships, documents and information requirements.
2. **Connected business workflows:** planning, procurement, commercial management, finance, accounting, construction, operations and maintenance.
3. **Agent orchestration:** interpreting events, assembling evidence, coordinating tasks, invoking approved tools and tracking decisions.

The agent capabilities below are proposed application features. Their performance and permitted authority must be validated during implementation.

## 1 What BIM consists of

### 1.1 Information requirements

- What information the client, project team and asset operator need.
- Who must produce it, when, in what format, and how it will be accepted.
- Example: every maintainable pump needs a tag, specification, warranty, manual and maintenance requirements before handover.

### 1.2 BIM execution and responsibility planning

- BIM Execution Plan, discipline responsibilities, model coordination rules and information delivery schedules.
- Agreed naming, classification, units, coordinates and required information detail.
- These establish how participating organisations will work together.

Reference: [UK BIM Framework guidance on information management responsibilities](https://ukbimframework.org/wp-content/uploads/2021/02/Guidance-Part-A_The-information-management-function-and-resources_Edition-2.pdf).

### 1.3 Discipline models

- Architectural, structural, mechanical, electrical, plumbing and fire systems.
- Civil works, terrain, roads, drainage, utilities and infrastructure.
- Factory equipment and process systems where included in project scope.

### 1.4 Object properties and relationships

- Object identity, location, dimensions, material, classification and technical properties.
- Relationships such as a pump belonging to a cooling system or a culvert serving a road section.
- Later information can include manufacturer, serial number, installation date and maintenance history.

### 1.5 Drawings and supporting documents

- Plans, sections, details, specifications, calculations and surveys.
- Technical submissions, inspection records, test certificates and operating manuals.
- References to the correct assets, packages and revisions.

### 1.6 Common Data Environment and revision control

- Controlled submission, review, sharing, publication and archiving of information.
- Clear status: work in progress, shared for coordination, approved for an intended use or superseded.
- Visibility of the information that authorises a particular activity.

Reference: [UK BIM Framework guidance on the Common Data Environment](https://ukbimframework.org/wp-content/uploads/2021/02/Guidance-Part-C_Facilitating-the-common-data-environment-workflow-and-technical-solutions_Edition-1.pdf).

### 1.7 Coordination and validation

- Combining discipline models for review.
- Detecting physical clashes, clearance problems, missing properties and inconsistent information.
- Recording issues, assigning owners and verifying corrections.
- Reviewing accessibility, maintainability and construction sequencing alongside geometric clashes.

### 1.8 Quantities time and cost connections

- Quantity take-off from suitable model information.
- Linking model elements to schedule activities for sequencing and visual planning, commonly called **4D**.
- Linking quantities and cost information, commonly called **5D**.

A model quantity still needs measurement rules, scope checks and commercial interpretation before it becomes a BOQ, purchase or payable quantity.

### 1.9 Construction verification and handover

- Comparing intended design with installed conditions.
- Managing approved changes, inspection evidence, commissioning and as-built information.
- Preparing information the operator can use.

### 1.10 Asset information for operations and maintenance

- Accepted asset register, system relationships, service access, warranties, spares and maintenance instructions.
- Connections between maintained assets, work orders, condition records and lifecycle changes.
- Defined update mechanisms and operational uses if a live digital twin is developed.

Labels such as 6D and 7D vary between organisations. Requirements should name the capability, such as sustainability analysis or maintenance information, rather than depend on the number.

## 2 Agent orchestration opportunities

Agents coordinate information and actions. Engineering software, calculation engines and authorised people provide the necessary checks and decisions.

### 2.1 Information requirements agent

**Actions**

- Convert approved requirements into submission checklists.
- Check missing asset properties, documents and delivery milestones.
- Route incomplete submissions to their owners.

**Expected value:** fewer information gaps discovered during handover.

### 2.2 Document and revision agent

**Actions**

- Classify incoming documents and extract proposed metadata.
- Compare revisions, summarise changes and identify affected teams.
- Flag references to superseded drawings.

**Expected value:** faster reviews and fewer mistakes from outdated information.

### 2.3 Design coordination and issue agent

**Actions**

- Collect clash results, design comments, Requests for Information and site issues.
- Group duplicates, suggest discipline ownership and prioritise affected work.
- Retrieve relevant specifications and previous decisions.
- Track corrective submissions and verification.

**Expected value:** less issue-administration effort and faster resolution.

BCF provides an established format for exchanging model-related issues and viewpoints between compatible tools. Reference: [buildingSMART BIM Collaboration Format](https://www.buildingsmart.org/standards/bsi-standards/bim-collaboration-format/).

### 2.4 Planning and constraint agent

**Actions**

- Check whether activities have approved design, access, permits, materials, labour and equipment.
- Identify missing predecessors and unresolved constraints.
- Request updates from responsible teams.
- Use a scheduling engine to compare recovery scenarios.

**Expected value:** more realistic lookahead plans and earlier warning of delay.

### 2.5 Quantity and change impact agent

**Actions**

- Compare quantities and specifications between revisions.
- Identify affected BOQ lines, activities, budgets, orders and installed work.
- Prepare a change-impact dossier for review.

**Expected value:** changes reach affected teams before commitments become expensive.

### 2.6 Procurement and material agent

**Actions**

- Combine approved demand, available stock, supplier lead times and required-on-site dates.
- Draft purchase requisitions and clarification requests.
- Flag late deliveries, excess purchases and technically mismatched submissions.

**Expected value:** fewer material shortages and unnecessary purchases.

### 2.7 Progress and evidence agent

**Actions**

- Organise daily reports, photographs, measurements and inspection records by package.
- Detect missing evidence and inconsistent progress claims.
- Suggest progress updates for verification.

**Expected value:** faster reporting with traceable supporting evidence.

Image-based progress estimates require checks for visibility, measurement and quality acceptance.

### 2.8 Cost finance and accounting agent

**Actions**

- Reconcile budget, commitments, accruals, actuals and forecast inputs.
- Flag duplicate invoices, missing receipts and unexplained variances.
- Draft cash forecasts and exception explanations.

**Expected value:** earlier financial intervention and less reconciliation work.

Approved budget, recognised revenue, invoicing and cash remain separate records.

### 2.9 Sales and contract agent

**Actions**

- Check proposed delivery dates and service promises against operational capacity.
- Transfer awarded commitments into owned contract obligations.
- Track certification, disputes, collection actions and renewal opportunities.

**Expected value:** stronger continuity from what Sales promises to what the company delivers.

### 2.10 Commissioning and handover agent

**Actions**

- Track tests, punch items, manuals, training, warranties and asset data.
- Identify what prevents system acceptance.
- Prepare handover packs and verify receiving-system acknowledgements.

**Expected value:** fewer incomplete assets transferred to Operations.

### 2.11 Operations agent

**Actions**

- Connect shift logs, incidents, asset status and service obligations.
- Highlight service deterioration and coordinate proposed shutdown windows.
- Explain operational effects of outstanding defects.

**Expected value:** clearer service decisions and faster coordination with Maintenance.

### 2.12 Maintenance and reliability agent

**Actions**

- Generate preventive work from approved plans.
- Draft corrective work orders, check spares and retrieve service history.
- Flag recurring failures and warranty recovery opportunities.
- Support repair-versus-replace analysis.

**Expected value:** better maintenance preparation and asset availability.

Predictive maintenance requires suitable condition and failure data. Basic maintenance workflows do not depend on predictive models.

## 3 Example of agent supported issue resolution

### Situation

A factory pipe blocks the maintenance access needed around a pump.

### Workflow

1. **Detect:** a coordination tool or reviewer raises the issue against the relevant model revision.
2. **Assemble context:** the agent collects the viewpoint, pump requirements, piping specification and affected package.
3. **Assign ownership:** propose the piping engineer as responsible, Engineering as accountable, and Maintenance, Construction and Planning as consulted. Resolve roles to named people and approval authorities.
4. **Assess urgency:** check fabrication, procurement and installation dates to establish downstream exposure.
5. **Develop options:** engineers propose alternatives; analysis tools test the relevant constraints.
6. **Assess impacts:** the agent assembles cost, schedule, procurement and maintenance consequences.
7. **Decide:** authorised reviewers select and approve the solution.
8. **Coordinate changes:** the agent tracks revised information and downstream change tasks.
9. **Verify closure:** close only after correction is verified and the required acceptance is recorded.

The agent can manage the resolution process. The engineer remains responsible for the technical solution.

## 4 Foundations required for reliable orchestration

Every orchestrated workflow needs:

- Stable project, package, activity, asset and document identifiers.
- Controlled revisions and authoritative source systems.
- Explicit states, ownership, dependencies and approval rights.
- SLA clocks, escalation rules and exception handling.
- Evidence requirements and an audit trail.
- Tool permissions that prevent duplicate or unauthorised actions.

Use ordinary rules for predictable checks, optimisation engines for constrained calculations, machine learning for evaluated predictions, and generative AI for interpretation and drafting. The agent coordinates these capabilities.

## 5 Authority boundaries

The proposed operating model allows agents to retrieve, compare, draft, route, remind and prepare recommendations within their permissions.

Controlled decisions remain with the designated authority, including:

- Engineering design approval and release.
- Contract award and commercial commitments.
- Budget changes, accounting approval and payment authorisation.
- Safety permits, isolation and work clearance.
- Operational acceptance and return to service.

An agent must not close an issue simply because a revised file was uploaded. Required evidence, verification and acceptance must be completed.

## 6 Recommended starting sequence

1. **Document and revision control plus issue coordination.** Establish reliable information and accountable resolution.
2. **Planning constraints plus change-impact assessment.** Connect engineering changes to delivery consequences.
3. **Asset information completeness plus maintenance work preparation.** Make operating needs visible before handover.
4. **Procurement and financial exception handling.** Improve supply coordination and commercial control.
5. **Predictive optimisation after reliable history exists.** Evaluate predictions against agreed baselines before operational use.

From the first release, Operations and Maintenance should define their information needs, Sales should register contractual promises, and Finance and Accounting should define financial controls. This keeps the platform useful throughout delivery and asset service.

## 7 Related blueprint documents

- [Overall plan](00_READ_ME.md)
- [Business requirements](01_BRD.md)
- [Product requirements](02_PRD.md)
- [Functional specification](03_FUNCTIONAL_SPECIFICATION.md)
- [Module and governance catalog](04_MODULE_AND_GOVERNANCE_CATALOG.md)
- [Consulting research and design rationale](05_RESEARCH_AND_DESIGN_RATIONALE.md)
- [Visual maps](06_VISUAL_MAPS.html)
