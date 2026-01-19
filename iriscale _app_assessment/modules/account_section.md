# Account Section

**Location:** User menu (upper right corner) → "Dean Gannon" dropdown  
**Tags:** 
- [x] `TRAINING` - Essential for user onboarding
- [ ] `VIDEO` - Basic setup walkthrough
- [x] `MARKETING` - Team collaboration features
- [ ] `PROMO`

---

## Overview
The Account section provides user profile management, company/organization administration, and team member management. Accessed via the user avatar/name dropdown in the top-right navigation.

---

## Account Menu Structure

| Menu Item | Route | Description |
|-----------|-------|-------------|
| Profile Settings | `/profile` | Personal account information and security |
| Companies | `/companies` | Organization and project management |
| People | `/people` | Team member administration across all companies |
| Sign Out | - | Logout action |

---

## 1. Profile Settings

**Route:** `/profile`  
**Page Title:** "Profile | Iriscale | Manage your profile"

### Interface Elements

#### User Card (Left Panel)
- **Avatar:** Initials-based (e.g., "DG")
- **Name:** Full name display
- **Email:** User email address
- **Status Indicators:**
  - Platform Staff: ✓/✗
  - Approved: ✓/✗
  - Invited: ✓/✗
- **Metadata:**
  - Timezone (e.g., UTC)
  - Created At (timestamp)
  - Updated At (timestamp)
  - Last Login (timestamp)

#### Personal Information (Right Panel)
- **First Name** - Editable text field
- **Last Name** - Editable text field
- **Email Address** - Editable text field
- **Edit Button** - Enables editing mode

#### Security Section
- **Change Password** button
- Description: "Keep your account secure by using a strong password."

### User Workflow
1. Click user name dropdown → Profile Settings
2. View current profile information
3. Click "Edit" to modify personal information
4. Click "Change Password" to update security credentials

### Screenshot
`screenshots/profile_settings.png`

---

## 2. Company Management

**Route:** `/companies`  
**Page Title:** "Projects & Teams | Iriscale | Manage organizations and projects"

### Interface Elements

#### Company List (Horizontal Tabs)
- Scrollable list of all companies user has access to
- Each company shows:
  - Company name
  - Settings/edit icon button
- Currently selected company is highlighted

#### Projects Panel (Center)
- **Header:** "Projects - Showing all projects in the Company"
- **Project Cards:** For each project:
  - Project name
  - Member count (e.g., "0 members")
  - Creation date
  - Status badge (e.g., "active")
  - Creator attribution (e.g., "Created by [Name]")
  - Settings/menu icon

#### Members Panel (Right)
- **Header:** "Members - Showing all company members"
- **Member Cards:** For each member:
  - Avatar (initials-based)
  - Full name
  - Role badge (Owner, Manager, Employee)
  - Email address
  - Join date
  - Status (Active/Inactive)
  - Actions menu

### Key Capabilities
| Capability | Description |
|------------|-------------|
| Multi-company support | Users can belong to multiple companies |
| Project organization | Companies contain multiple projects |
| Member management | Add/manage team members per company |
| Role-based access | Owner, Manager, Employee roles |

### User Workflow
1. Access via Account menu → Companies
2. Select a company from the horizontal tab list
3. View/manage projects within that company
4. View/manage members of that company

### Screenshot
`screenshots/companies_management.png`

---

## 3. People & Teams

**Route:** `/people`  
**Page Title:** "People | Iriscale | Manage team members"

### Interface Elements

#### Header Section
- **Title:** "People & Teams"
- **Description:** "Manage team members across all your companies and projects"
- **Invite Member** button (primary CTA)

#### Filters Bar
- **Search:** Text input for "Search members, companies..."
- **Company Filter:** Dropdown with all companies + member counts
- **Role Filter:** Dropdown with roles (All Roles, Owner, Manager, Employee)

#### Team Members Table
- **Header:** "Team Members (count)" with total count
- **Columns:**
  - Member (avatar, name, email)
  - Company (with expandable company list)
  - Role (Owner/Manager/Employee with icon)
  - Joined (date)
  - Status (Active badge)
  - Actions (menu icon)

#### Pending Invitations Section
- **Header:** "Pending Invitations (count)"
- **Company Filter:** Dropdown for filtering by company
- **Table Columns:**
  - Email
  - Company
  - Role
  - Invited By
  - Sent Date (sortable)
  - Expires
  - Message
  - Actions
- **Empty State:** "No Pending Invitations" with helper text

### Key Capabilities
| Capability | Description |
|------------|-------------|
| Cross-company view | See all team members across all companies |
| Search & filter | Find members by name, email, company, or role |
| Invite members | Send invitations to new team members |
| Role management | Assign Owner, Manager, or Employee roles |
| Invitation tracking | Monitor pending invitations and expiration |

### User Workflow
1. Access via Account menu → People
2. Use search/filters to find specific members
3. Click "Invite Member" to add new team members
4. Use row actions to manage individual members
5. Monitor pending invitations in lower section

### Screenshot
`screenshots/people_teams.png`

---

## Value Propositions

### For Training Documentation
- **Profile Settings:** "Update your personal information and change your password from the Profile Settings page. Access it by clicking your name in the top-right corner."
- **Companies:** "Manage multiple companies and their projects from a single dashboard. Switch between companies using the tab selector."
- **People:** "View and manage all team members across your organizations. Invite new members, assign roles, and track pending invitations."

### For Marketing Website
- **Multi-tenant architecture:** "Manage multiple companies and projects from one account"
- **Team collaboration:** "Invite team members with role-based permissions (Owner, Manager, Employee)"
- **Centralized administration:** "Single dashboard to manage all your organizations and teams"

### For Video Script
1. Show login → click user dropdown
2. Walk through Profile Settings (quick edit demo)
3. Navigate to Companies → show company switching
4. Navigate to People → demonstrate invite flow and filtering

---

## Related Features
- **Projects & Teams** (sidebar) - Alternative access to project management
- **Top Navigation** - Company/project selector dropdown

---

## Technical Notes
- Routes are protected (require authentication)
- Real-time member counts in filters
- Avatar fallback to initials when no image

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
