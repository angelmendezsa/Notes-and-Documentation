## 02/20/2026 (Friday 3PM CUP Meeting)

- Data housing: Dataverse
- Share all CUP data in CHHS IT SharePoint → Projects → CUP
- Dashboards: Wireframes
- Workflows → Wireframing
- Second Planner board for TQR
- Everything tracked in Planner
- Roadmap created after plan (target items)

---

### CUP Direction + Ownership

- Invoice automation for Richard.
- Angel now up to speed on PowerApps.
- Chair approver workflow discussion.
- Andrew will decide how CUP is built.
- CUP email system → convert to dashboard widget (target item).
- Use system to identify next eligible people.
  - Faculty currently ask Jose about future eligibility.

---

### Data Considerations

- June 30 → final data release for CUP update.
- Data sources: Stacey, Michael, Chairs.
- Data quality issues:
  - People leave.
  - People join.
  - Eligibility data becomes outdated.

- March 6 → tasks assigned.

---

### Automation Needs

- Richard needs automation to roll up quotes into one invoice.
- Reduce reliance on email automation → move visibility into dashboards/widgets.
  - Previously 1 email, now ~8 emails.
  - Not necessarily fewer emails, but all tasks should be visible in a dashboard.

---

### Access + Governance

- Use admin accounts (not personal accounts).
- Angel needs Dataverse license.
- Ensure all required data is available for Richard and Jose.
- Challenge Andrew/Jose with alternative ideas where appropriate.

---

## 02/20/2026 (Friday 4PM Angel Progress Meeting)

- Friday Angel Progress Meeting.
- Showed CRUD PowerApp.
- Displayed CUP workflow (Visio).
- Discussion about future projects:

  - Work on Richard’s “Invoice Roll-Up” automation.
  - Possible migration of SharePoint list to Dataverse.
  - Watch for yellow warning indicators in PowerApps:
    - Filter functions not scalable past 2000 records.
    - Delegation warnings.
    - Potential future performance errors.


# 02/16/2026 (Monday)

### TL;DR

- Built out full CUP workflow chart
- - Link to CUP workflow chart: [CUP Workflow Diagram](https://csulb.sharepoint.com/:u:/r/sites/CHHS-IT/Shared%20Documents/CUP/Angel%20Rough%20CUP%20Workflow.vsdx?d=wb7c4269761f14b93b18071ddf96fe378&csf=1&web=1&e=1jF72F)
- Continuing Canvas CRUD app development
- Meeting with Chris and Andrew 2PM 

---

## 2PM CUP Meeting

---

### What do we currently understand?

- I built a full lifecycle workflow chart mapping eligibility through deployment.
- SQL database target: Dataverse.
- Faculty members choose their equipment.
- Goal: push selections into our structured CUP workflow.
- Current system uses SharePoint + Power Automate (Tech Quote Request / TQR).
- Power Automate sends emails when a request enters the list:
  - Department approval
  - Purchasing approval
  - Dean approval
- Heavy email-driven process.
- Concern about tracking status:
  - Quote requested
  - Quote received
  - Quote accepted

---

### What is still needed?

- Define how dashboard will function (requires clean data + workflow states).
- Address licensing:
  - Enough Dataverse licenses for IT.
  - Not enough for front office / finance managers.
- Inventory SharePoint access issue (currently no access).
- Solve manual department-level invoice aggregation (Richard manually totals selections).
- Improve visibility into quote lifecycle.
- Reduce email chains.

---

### What is the plan by end of Design Phase (3wks)?

- A phased implementation plan to reach MVP.
- Confirm dashboard requirements.
- Wireframing for Dashboard.

---

### Additional Notes

- Andrew wants to improve pieces that are not working.
- Jose wants to build from scratch.
- Jose wants dashboards.
- Dashboard requirements:
  - Filter-based views.
  - Not much heavy coding.
  - Needs defined data, workflow, and activities.

- PR Purchase Requisition runs through:
  - “Tech Quote Request” (TQR) system.
- CHHS Tech Quote Requests built on SharePoint solution.
- Contains TQR + Power Automate email flows.

- App idea:
  - People who choose equipment get access to a layer of the CUP app.
  - Add “Change Computer” button in CUP app.

---

### CUP Workflow Build-Out

- Created end-to-end CUP workflow diagram
- Mapped full lifecycle:
  - Eligibility (Microsoft List)
  - Chair Confirmation
  - Quote Process
  - Procurement Review
  - DPR Handling
  - Purchasing (PO creation)
  - Receiving & Inventory
  - Deployment

- Added decision branch:
  - Chair Denial → Status Closed

---

### Architecture Clarification

**Frontend**
- CHHS Storefront entry point

**Backend**
- Dataverse (CUP records)
- Microsoft List (Eligibility)

**Integration**
- Procurement system
- Inventory system

---

### Roles & Responsibilities Defined

- End User – submits / signs DPR
- Chair – confirms eligibility
- Coordinator – requests quotes
- Procurement – reviews quote + funding
- IT – receives + tags device
- System – logs, tracks, stores documents

---

### Automation Triggers Identified

- On eligibility check → notify Chair
- On Chair approval → notify Coordinator
- On Procurement approval → generate DPR
- On PO creation → log tracking
- On delivery → update inventory
- On deployment → close request

Goal: reduce email chains + manual tracking

---

### App Work

- Continuing Canvas CRUD app development
- Refining structure to align with CUP workflow
- Focus still on functionality > polish





