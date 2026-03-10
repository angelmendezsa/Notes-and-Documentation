# 03/06/2026

### TL;DR
- Angel Back in Office
- Angel to Get accustomed to [CHHS-IT-SA site](https://csulb.sharepoint.com/sites/CHHS-IT-SA?e=1%3Afa68d22a1c9e426ea715b1f5b94013b5&xsdata=MDV8MDJ8QW5nZWwuTWVuZGV6LVNBQGNzdWxiLmVkdXxjOTE5MTgzOGQ0MGQ0ZTMyYzU1YzA4ZGU3OGI0MDllZHxkMTc1Njc5YmFjZDM0NjQ0YmU4MmFmMDQxOTgyOTc3YXwwfDB8NjM5MDgwOTExODA4NzgzMDcxfFVua25vd258VFdGcGJHWnNiM2Q4ZXlKRmJYQjBlVTFoY0draU9uUnlkV1VzSWxZaU9pSXdMakF1TURBd01DSXNJbEFpT2lKWGFXNHpNaUlzSWtGT0lqb2lUV0ZwYkNJc0lsZFVJam95ZlE9PXwwfHx8&sdata=MlhoRUs4RmJqdGt4VWhaN2pRYy9FRjI5RXNwR1RRS2x3UmZSc2thWGFycz0%3D&CT=1772495917649&OR=OWA-NT-Mail&CID=c06bbafe-ba26-1388-4bb3-a95cb715d4c7&clickParams=eyJYLUFwcE5hbWUiOiJNaWNyb3NvZnQgT3V0bG9vayBXZWIgQXBwIiwiWC1BcHBWZXJzaW9uIjoiMjAyNjAyMTMwMDEuMDYiLCJPUyI6IldpbmRvd3MgMTEifQ%3D%3D&Mode=Edit)
- Angel to make a minor change or update to the site
- Angel wrote documentation about the [CHHS-IT-SA site](https://github.com/angelmendezsa/Notes-and-Documentation/blob/main/Documentation/CHHS-IT-SA%20SharePoint%20Site%20Documentation.md)

# 03/09/2026

### TL;DR
- Angel Out Sick

---

# 03/06/2026

### TL;DR
- Angel Out Sick

---

# 03/03/2026

### TL;DR

- Continuing work on wireframe Dashboard for Chairs. [Chair Dashboard Wireframe](https://csulb.sharepoint.com/:u:/r/sites/CHHS-IT/Shared%20Documents/CUP/Angel%20-%20CUP%20Workflow%20by%20Role.vsdx?d=w169e6ee756b34ea79b53025b194103f0&csf=1&web=1&e=bJHJsT)
- Made minor changes to improperly named parts of my original workflows for Chairs & IT Supervisor
- Researching and defining what Dataverse is.
- Evaluating why Dataverse may be better than SharePoint for CUP.
- Read over Richard's review of Chartfields in OneNote

---

### Work in Progress

- Continuing work on wireframe Dashboard for Chairs.

---

## What is Dataverse?

- Microsoft Dataverse.
- Secure, scalable, intelligent data platform for Power Platform and Microsoft 365.
- A “system of action.”
- Empowers organizations to unlock data’s full potential.
- Enables faster insights.
- Avoids expensive and time-consuming custom data infrastructure.
- Unifies multiple data types in one place.
- Low-code capabilities → non-developers can build useful apps.
- Builds reusable components that can scale across thousands of apps.
- All data connected and accessible when needed.

---

## When is Dataverse Better Than SharePoint?

Dataverse is better when:

- Data relationships matter  
  (Users → Departments → Devices → Approvals)

- Record-level security is required.
- You expect growth.
- You need performance beyond 2,000+ record limits.
- You want to avoid delegation issues.
- You need structured, relational data.

---

## Why Are We Considering Dataverse for CUP?

Because CUP is:

- Multi-role (Users, Chairs, Procurement, IT).
- Multi-step workflow.
- Approval-based.
- Financially sensitive.
- Data-heavy and growing.

Dataverse provides:

- Structured tables.
- Relationships between data.
- Secure role-based access.
- Scalable performance.
- Cleaner automation.

# 03/02/2026 Meeting Notes

### TL;DR

- Deep dive into workflows + wireframes.
- Discussion around Dataverse vs SharePoint data flow.
- Approval visibility + department filtering concerns.
- Need clear end objective for CUP.
- Avoid scope creep into rebuilding TQR.
- Action items assigned to Angel.

---

### Workflow + CUP Discussion

- Combine records in CUP?
  - Combine lists.
  - How to merge 2 records into 1 record?

- Creating records.
- Break down each step before building:
  - What tool is used?
  - What data is required?
  - How does it flow?
  - Who owns it?

Goal: Get to as much detail as possible before full build.

---

### Users + Data Model

- Users (MOD 4)
- Fiscal Year MOD 4
- MOD 4 tied to Employee ID? (Andrew disagrees)
- User database will be core to system.

Data Flow:
- Users in Dataverse → CUP (this cycle in SharePoint)
- SP = SharePoint list
- DV = Dataverse

CUP App should store:
- User
- Department
- Current device
- Asset
- Selected choice
- Cost
- Order #
- (Review fields for necessity)

Fields in Dataverse may be altered by Jose & Richard (subprocess work).

Then send data back to SharePoint list for departments.

Open question:
- Roll-up to Dataverse?
- Or roll-up to SharePoint?

Andrew is dependent on us to help choose tools/databases wisely.

---

### Approval + Department Filtering Issues

- Separate SharePoint lists by department?
  - If school doesn’t want cross-department data visible.
- Possibly Filter users based on department or create completely new lists for each Dep.

Concern (Chris’ notes):
- SharePoint permissions are work (seen in Time-Off app).
- Filtering in Canvas App works visually,
  but does NOT prevent access to full SharePoint list.
- Filtering alone may not be secure.
- Users could potentially access underlying list data.

Question:
- Should departments only see their own data?
- If so, how do we enforce that securely?

Important:
- USERS CANNOT EDIT DATA (unless explicitly allowed).
- Jose may want departments to edit their own CUP entries.
- Adds complexity (may not have time).

---

### Scope + Objective

- What does “complete” mean?
- What is the final objective of CUP?

Andrew:
- Does NOT want scope creep into rebuilding TQR.
- Objective is CUP system.
- Integrate as much data as possible into IT Dataverse side.
- Needs our help deciding integration strategy.

We need to:
- Manage where users funnel through.
- Decide what moves into Dataverse actions for Richard & Jose.

---

### Angel Question

- Why are we using Dataverse? (Answered on 3/3/2026 by Angel)
- Are all the goals just to:
  - Make workflow easier for decision makers?
  - Automate + finalize CUP data flow?
  - Improve efficiency for Richard?

---

### Scheduling

- Next 3 weeks: maybe meet Tuesdays.
- No Friday Team Meetings (Conference CUP meetings).
- Be mindful of Angel’s limited office time.

---

## Angel Action Items

- Update workflows to use role names (not personal names). As they may be sent to other schools. 
- Provide Andrew technical documentation for LOR
  (after slight CHHS website update).
- Get familiar with CHHS-IT-SA site (design privileges granted).
- Use LLM to build a SharePoint Framework feature
  and connect it to CRUD app.
- Focus on leveraging AI for productivity:
  - Understand the problem.
  - Understand output.
  - Understand why something was built.
