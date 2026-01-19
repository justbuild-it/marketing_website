# Organization & Project Selector

**Location:** Top navigation header (left side)  
**Tags:** 
- [x] `TRAINING` - Essential for navigation and context switching
- [x] `VIDEO` - Important for onboarding demos
- [x] `MARKETING` - Multi-tenant/multi-project capability
- [ ] `PROMO`

---

## Overview
The Organization and Project selectors in the header allow users to switch between different companies (organizations) and projects within those organizations. All app content is scoped to the selected organization and project.

**Key insight:** A typical customer will have only one organization but may have multiple projects within it.

---

## Header Layout

```
[Logo] [Organization Selector ▼] [Project Selector ▼]    [AI Agent] [Feedback] [beta] [User Menu ▼]
```

---

## 1. Organization Selector

### Interface Elements
- **Current Selection:** Displays organization name with dropdown arrow
- **Dropdown Contents:**
  - Header: "Organizations"
  - List of all organizations user has access to
  - **"+ New organization"** button at bottom

### Behavior
- Click to open dropdown
- Selecting an organization:
  - Switches context to that organization
  - Auto-selects the first (or last used) project in that org
  - All app data updates to reflect the new context

### Example Organizations (from Shuk Rentals account)
- yashoda manual testing
- Lunour
- TSI
- Iriscale
- Greenbox
- Reozom
- Encubatorr
- Mangrove
- Satta
- test2
- test1
- **Shuk Rentals** ← Selected for evaluation
- GoShare
- Mindful Child and Family Therapy
- Sagent
- Balaji Dehydration
- Creston and Company

### Screenshot
`screenshots/org_selector_dropdown.png`

---

## 2. Project Selector

### Interface Elements
- **Current Selection:** Displays project name with dropdown arrow
- **Dropdown Contents:**
  - Header: "Projects"
  - List of all projects in the selected organization
  - **"+ New project"** button at bottom

### Behavior
- Click to open dropdown
- Selecting a project:
  - Switches context to that project
  - All app data (Knowledge Base, Articles, etc.) updates to the selected project
- Projects are organization-specific (switching org changes available projects)

### Example Projects (Shuk Rentals organization)
| Project | Description |
|---------|-------------|
| **Shuk GTM v0.2** | Current/active version |
| Shuk GTM v0.1 | Previous version |

### Screenshot
`screenshots/project_selector_dropdown.png`

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| Multi-organization | Users can belong to multiple organizations |
| Multi-project | Each organization can have multiple projects |
| Context isolation | All app content is scoped to selected org + project |
| Quick switching | Dropdown selectors for fast context changes |
| Create new | Can create new organizations and projects inline |

---

## User Workflow

### Switching Organization
1. Click organization name in header
2. Dropdown shows all available organizations
3. Click desired organization
4. System auto-selects a project in that org
5. All app content updates to new context

### Switching Project (within same org)
1. Click project name in header
2. Dropdown shows all projects in current org
3. Click desired project
4. All app content updates to new project context

### Creating New Project
1. Click project selector dropdown
2. Click "+ New project" at bottom
3. (Likely opens project creation modal/form)

### Creating New Organization
1. Click organization selector dropdown
2. Click "+ New organization" at bottom
3. (Likely opens organization creation modal/form)

---

## Value Propositions

### For Training Documentation
- "Switch between organizations using the dropdown in the top-left of the header"
- "Each organization can contain multiple projects - select the project you want to work on"
- "All your content (Knowledge Base, Articles, etc.) is specific to your selected project"
- "Create new projects to separate different marketing initiatives or campaigns"

### For Marketing Website
- **Multi-tenant architecture:** "Manage multiple client accounts or business units from one login"
- **Project-based organization:** "Separate campaigns, product lines, or initiatives into distinct projects"
- **Seamless switching:** "Instantly switch between contexts without logging out"

### For Video Script
1. Show header with org/project selectors
2. Click org dropdown → show list of organizations
3. Select different org → show context change
4. Click project dropdown → show projects within org
5. Demonstrate "+ New project" button

---

## Typical Customer Setup

Based on user guidance:
- **Organizations:** Most customers will have **1 organization** (their company)
- **Projects:** Multiple projects within that organization for:
  - Different product lines
  - Different campaigns
  - Version iterations (e.g., "GTM v0.1", "GTM v0.2")
  - Testing vs. production content

---

## Related Features
- **Company Management** (`/companies`) - Full org/project administration
- **Projects & Teams** (sidebar) - Alternative access to project settings

---

## Technical Notes
- Organization/project selection persisted across sessions
- Context stored: company ID + project ID
- API calls scoped to selected context
- Switching context triggers data refresh

---

## Assessment Status

| Item | Complete |
|------|----------|
| Overview documented | ✅ |
| Capabilities listed | ✅ |
| Workflow captured | ✅ |
| Screenshots taken | ✅ |
| Value props written | ✅ |
| Use cases defined | ✅ |
| Reviewed for accuracy | ⬜ |

---

*Assessed by: Cascade*  
*Date: January 17, 2026*  
*Version: 1.0*
*Evaluation context: Shuk Rentals → Shuk GTM v0.2*
