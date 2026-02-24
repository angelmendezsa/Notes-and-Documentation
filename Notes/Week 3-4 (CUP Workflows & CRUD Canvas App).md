# 02/23/2026 - Meeting Notes

---

## Andrew

- Ironing out the tables
- Working on tables planning page
- Queries are currently not working
- Need to map out what has happened so far

---

## Angel

- Angel asks for a foundation of databases/lists/tools needed to automate Richard's headaches that he does manually
- Angel to get Richard's advice about Richard's manual inefficiences so Angel can get scope of work for automation
- Other possible work:
- **Wireframe/ Design dashboard for Jose in Power BI or whatever tool**
- **Maybe do the 'Change Device' or 'Discard' button on the PowerApps catalog for faculty (in case they choose wrong - rare)**

---

## Chris

- Working on his app
- Wants devs assigned to tasks

---

## Richard

- Works with IT-SA site list
- Uses **CHHSS Technology Procurement**
- Environment: **TQR - DEV**
- Site contents include:
  - Parent request
  - Line items

---

## Scope of Work / Questions

- Currently guessing what Jose wants / what Richard needs
- Does updating status cascade everywhere else?
- Line items belong to a parent request
- How can two objects within a parent request be combined into one?
- Andrew to spin up a sandbox environment to work with data
- CUP Frontend:
  - Design set so devs should not see certain elements?
- Legitimately impersonate other users (similar to Canvas student view for professors)
- Ability to impersonate a specific user to check permissions or for testing

---

## Jose Requests

- Dashboard to see tasks requiring approval/disapproval for CUP users
- Expanded data analytics capabilities (See 13 imacs versus 12 windows laptops)

---

# 02/20/2026 (3PM CUP Meeting)

### TL;DR

- Dataverse likely confirmed for data housing.
- Move email-heavy workflow visibility into dashboards/widgets.
- Wireframing + Planner organization in progress.
- Invoice roll-up automation needed for Richard.
- Data quality + eligibility tracking are major concerns.
- Angel needs Dataverse license.

---

### Data + System Direction

- Data housing: Dataverse.
- Share all CUP data in CHHS IT SharePoint → Projects → CUP.
- Dashboards to start as wireframes.
- Workflows moving into wireframing phase.
- Create second Planner board for TQR.
- Everything tracked in Planner.
- Roadmap defined after planning (target items).

---

### CUP Direction + Ownership

- Invoice automation for Richard.
- Andrew will decide overall build direction for CUP.
- Convert CUP email system → dashboard widget (target item).
- Use system to identify next eligible people.
  - Currently faculty ask Jose about future eligibility.

---

### Data Considerations

- June 30 → final data release for CUP update.
- Data sources: Stacey, Michael, Chairs.
- Data quality issue:
  - People leave.
  - People join.
  - Eligibility data becomes outdated.

- March 6 → tasks assigned.

---

### Automation + Workflow Issues

- Richard needs automation to roll up quotes into one invoice.
- Reduce reliance on email automation → move tasks into dashboards/widgets.
  - Previously 1 email.
  - Now ~8 emails.
  - Goal: central task visibility, not just fewer emails.

---

### Access + Governance

- Use admin accounts (not personal accounts).
- Angel needs Dataverse license.
- Ensure Richard and Jose have all required data.
- Challenge Andrew/Jose with alternative ideas when appropriate.

---

# 02/20/2026 (4PM Angel Progress Meeting)

### TL;DR

- Demoed CRUD PowerApp.
- Presented CUP workflow (Visio).
- Discussed future automation + Dataverse migration.
- Reminder to watch for PowerApps scalability warnings.

---

### Discussion

- Showed CRUD PowerApp.
- Displayed CUP workflow in Visio.

Future work discussed:
- Richard’s “Invoice Roll-Up” automation.
- Possible migration of SharePoint list to Dataverse.
- Monitor yellow warning indicators in PowerApps:
  - Filter functions not scalable past 2000 records.
  - Delegation warnings.
  - Future performance issues.


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












