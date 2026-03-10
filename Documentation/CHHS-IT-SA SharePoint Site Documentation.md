# CHHS-IT-SA SharePoint Site  
Technical Documentation  

Document Version: 1.0

Author: Angel Mendez  
Department: CHHS IT  
Environment: Microsoft 365 – SharePoint Online  
Site URL: https://csulb.sharepoint.com/sites/CHHS-IT-SA  

Site Type: Team Site  
Group-Connected: Yes (Microsoft 365 Group Connected)  
Privacy Level: Private (Indicated as "Private group" on site header)  
Access Level of Documenter: Member (Edit Permissions)  
Last Updated: 03/10/2026  

---

# 1. Executive Overview

## 1.1 Purpose

The CHHS-IT-SA SharePoint site serves as the centralized onboarding, operational reference, and collaboration portal for CHHS IT Student Assistants.

## 1.2 Audience

- Student Assistants  
- IT Staff  
- Supervisors  

## 1.3 Scope

This documentation reflects the current-state configuration of the site based on Member-level visibility.

This document covers:

- Site configuration (as visible to Member role)
- Permissions structure (observable groups)
- Navigation architecture
- Pages and content structure
- Document libraries and lists
- Integrations
- Governance observations

---

# 2. Site Configuration

## 2.1 General Settings

| Setting                    | Value                               |
|----------------------------|-------------------------------------|
| Site Type                  | Team Site                           |
| Group Connected            | Yes (Microsoft 365 Group Connected) |
| Privacy Level              | Private                             |
| Access Level of Documenter | Member (Edit Permissions)           |

## 2.2 Administrative Visibility Limitations

The document author does not have Owner or SharePoint Admin permissions.

The following configurations are managed at the SharePoint site collection or Microsoft 365 tenant level and are not visible under Member-level access:

- **Storage Quota Allocation** – Defines the maximum storage space allocated to the site collection.
- **Tenant-Level External Sharing Configuration** – Controls whether users outside the organization can access site content.
- **Sensitivity Labels** – Classify site content for security and compliance within Microsoft 365.
- **Advanced Site Collection Settings** – Includes administrative controls such as feature activation and governance configuration.

Administrative-level configurations are assumed to be managed by CHHS IT or Microsoft 365 tenant administrators.

---

# 3. Permissions Model

## 3.1 SharePoint Groups (Visible)

| Group Name | Permission Level | Description                        | Count        |
|------------|------------------|------------------------------------|--------------|
| Owners     | Full Control     | Administrative control of the site | 10           |
| Members    | Edit             | Create and modify site content     | 10           |
| Visitors   | Read             | View-only access                   | Not Observed |

## 3.2 Inheritance

Permission inheritance determines whether libraries and lists follow the root site’s security model or use unique permissions.

Inheritance configuration not verified at Member permission level.

---

# 4. Navigation Architecture

## 4.1 Left Navigation Structure

- Home  
- Calendar  
- Documents  
- Duties and Skills  
- Assessment Form  
- Student-Employee Learning  
- SA General Planner  
- SA Notebook  
- Recycle Bin  

## 4.2 Navigation Type

Vertical (Flat Structure)

## 4.3 Observations

Navigation is flat and not grouped by functional domain (e.g., Onboarding, Operations, Resources).  
Links appear manually organized within the default Team Site structure.

---

# 5. Pages

## 5.1 Home Page

### Web Parts Identified

- People Web Part  
- Text Web Part  
- Image Web Part  
- Files and Media Web Part  
- Hyperlinks  
- Planner Link  

### Content Sections

- Welcome  
- Team Directory  
- Time Management  
- Expectations  
- Ingress / Egress  

Content is primarily static and embedded directly within the page.

---

## 5.2 Calendar

Displays the Microsoft 365 Group calendar associated with the SharePoint Team Site.

---

## 5.3 Documents Page

Displays contents of the default “Documents” document library.

---

## 5.4 Duties and Skills

### Web Parts Identified

- Text Web Part  

### Content Sections

- Duties and Skills Overview  
- Technology Support  
- Designer  
- AVTI  
- Programmer  
- Developer  

Content is static and page-based.

---

## 5.5 Assessment Form

### Platform

Microsoft Lists (List Form)

### Skill Rating Scale

1 (Learner) – 5 (Expert)

### Fields Observed

- Communication  
- Teamwork  
- Leadership  
- Critical Thinking  
- Professionalism  
- Equity and Inclusion  
- Technology  
- Self-Development  

Form is powered by Microsoft Lists and used for skill evaluation tracking.

---

## 5.6 Student-Employee Learning Plan

### Platform

Microsoft Lists

### Columns Observed

- Title  
- Learning Objective  
- Accomplishment  
- Measurement  
- Timeline  
- Accomplished (Boolean)  
- Exceeded (Boolean)  
- Supervisor Notes  

Content is structured and list-driven.

---

# 6. Document Libraries

## 6.1 Documents (Default Library)

### Purpose

General file storage for CHHS-IT-SA site content.

### Versioning

Versioning tracks historical changes to files and enables rollback to previous versions.  
Versioning configuration not verified at Member permission level.

### Folder Structure

Folder structure is visible within the library but not formally standardized or categorized.

---

## 6.2 Additional Libraries

No additional custom document libraries identified at Member-level visibility.

---

# 7. SharePoint Lists

The following custom lists are present:

| List Name                      | Purpose                                      |
|--------------------------------|----------------------------------------------|
| Assessment Form                | Skill evaluation and competency tracking     |
| Student-Employee Learning Plan | Learning objectives and performance tracking |

Additional system-generated lists may exist but are not documented at Member level.

---

# 8. Integrations

## 8.1 Microsoft Teams

Site is Microsoft 365 Group-connected, indicating integration with a corresponding Microsoft Teams workspace.

## 8.2 Microsoft Planner

“SA General Planner” link present in navigation, indicating integration with a Microsoft Planner plan associated with the group.

## 8.3 OneNote Notebook

“SA Notebook” link present in navigation, indicating integration with a Microsoft 365 Group-connected OneNote notebook.

## 8.4 Power Automate

No visible automation flows embedded or surfaced at Member level.

## 8.5 Power Apps

No embedded Power Apps identified on visible site pages.

---

# 9. Metadata & Content Types

No custom metadata columns or site-level content types observed at Member visibility level.

Metadata enables structured classification of documents and list items for improved filtering, organization, and reporting.

Administrative review required for confirmation of site-level content types.

---

# 10. Versioning & Retention

- **Versioning** – Tracks file revisions and preserves previous versions for audit and rollback purposes. Configuration not verified.
- **Retention Policies** – Control how long content is retained or deleted for compliance purposes. Not visible at Member level.

---

# 11. Storage & Usage

## 11.1 Storage Consumption

Storage consumption reflects the amount of space used within the site collection.  
Quota and usage limits are managed at the tenant administration level and not visible under Member permissions.

## 11.2 Activity

Site usage analytics indicate:

- Unique Visitors: 24 (All Time), 1 (Last 7 Days)
- Total Views: 820 (All Time), 9 (Last 7 Days)
- Average Time per User: 12m 12s
- Peak Usage Window: 8:00 AM – 12:00 PM

---

# 12. Risks & Technical Observations

- Majority of policy and procedural information is embedded as static page content.
- Limited use of structured content architecture beyond Microsoft Lists.
- Image-based informational content may reduce long-term maintainability.
  (Can't just edit text, need to edit image externally. Content isn't searchable.)
- Navigation structure is flat and manually organized.
- Administrative governance configurations are managed at the Owner or tenant level and were not directly verifiable under Member permissions.
---

# 13. Appendix

## 13.1 Screenshots  
## 13.2 Change Log  
## 13.3 Review History  

---

End of Document