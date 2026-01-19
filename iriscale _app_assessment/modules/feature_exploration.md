# Feature Exploration Page

**Route:** `/` (root URL)  
**Page Title:** "Iriscale"  
**Purpose:** Main landing page after login - guides users through platform features  
**Tags:** 
- [x] `TRAINING` - Primary onboarding/orientation tool
- [x] `VIDEO` - Excellent for product tour videos
- [x] `MARKETING` - Shows platform breadth
- [ ] `PROMO`

> **Note:** This page is flagged for UI improvements

---

## Overview

The Feature Exploration page serves as the main dashboard/home page for users after logging in. It provides:
1. A progress tracker showing feature exploration status
2. A categorized list of all platform features
3. Contextual help/guidance for each feature

---

## Page Layout Structure

```
┌─────────────────────────────────────────────────────────────────────────┐
│ HEADER: [Logo] [Org Selector] [Project Selector]    [AI Agent][User]   │
├──────────┬──────────────────────────────────────────────────────────────┤
│          │  ┌─────────────────────────────────────────────────────────┐ │
│          │  │ EXPLORATION                           13/13 explored   │ │
│ SIDEBAR  │  │ Feature Exploration                 0 features to disc │ │
│          │  │ Track your journey through the platform                │ │
│          │  ├─────────────────────┬───────────────────────────────────┤ │
│          │  │ Features            │ [Selected Feature Name]          │ │
│          │  │                     │ [Short description]              │ │
│          │  │ INTELLIGENCE &      │ ┌─────────┐ ┌──────┐             │ │
│          │  │ RESEARCH            │ │Explored │ │ View │             │ │
│          │  │ ├─ Knowledge Base   │ └─────────┘ └──────┘             │ │
│          │  │ ├─ Keyword Repo     │                                  │ │
│          │  │ ├─ Search Ranking   │ Overview                         │ │
│          │  │ └─ Competitor...    │ [Paragraph description]          │ │
│          │  │                     │                                  │ │
│          │  │ STRATEGY &          │ How to use it                    │ │
│          │  │ PLANNING            │ • Step 1                         │ │
│          │  │ ├─ Content Arch     │   - Sub-step                     │ │
│          │  │ ├─ Topics           │ • Step 2                         │ │
│          │  │ └─ AI Opt Questions │   - Sub-step                     │ │
│          │  │                     │                                  │ │
│          │  │ CONTENT CREATION    │ What you get / Best practices    │ │
│          │  │ ...                 │ • Benefit 1                      │ │
│          │  │                     │ • Benefit 2                      │ │
│ Getting  │  └─────────────────────┴───────────────────────────────────┘ │
│ started  │                                                              │
│ 100%     │                                                              │
└──────────┴──────────────────────────────────────────────────────────────┘
```

---

## UI Components - Detailed Breakdown

### 1. Page Header Section

| Element | Content | UI Details |
|---------|---------|------------|
| Breadcrumb label | "EXPLORATION" | Small caps, muted text |
| Page title | "Feature Exploration" | H1, large font |
| Subtitle | "Track your journey through the platform" | Muted description text |
| Progress counter | "13/13 explored" | Right-aligned stat |
| Discovery counter | "0 features to discover" | Secondary stat below |

**Current State Observations:**
- Progress shows completion status (13/13 = 100%)
- "0 features to discover" appears when all explored

---

### 2. Features List Panel (Left Side)

**Structure:** Categorized list with section headers

| Category | Features | Count |
|----------|----------|-------|
| **INTELLIGENCE & RESEARCH** | Knowledge Base, Keyword Repository, Search Ranking, Competitor Analysis | 4 |
| **STRATEGY & PLANNING** | Content Architecture, Topics, AI Optimization Questions | 3 |
| **CONTENT CREATION** | Articles, AI Optimization Answers | 2 |
| **OPPORTUNITY & ENGAGEMENT** | Opportunity Agent | 1 |
| **PROMOTE** | Social Posts, Connections, Social Scheduler | 3 |

**Total: 13 features**

#### Feature List Item UI

Each feature item displays:
```
┌────────────────────────────────────────┐
│ [Feature Name]              [Explored] │
└────────────────────────────────────────┘
```

| Element | Style | Behavior |
|---------|-------|----------|
| Feature name | Regular text | Clickable - selects feature |
| Status badge | "Explored" (purple badge) | Shows exploration status |
| Selection state | Left border highlight (purple) | Indicates current selection |
| Hover state | Cursor pointer | Interactive feedback |

---

### 3. Feature Detail Panel (Right Side)

Displays detailed information for the selected feature.

#### Detail Panel Header
```
┌─────────────────────────────────────────────────────────┐
│ [Feature Name]                                         │
│ [Short one-line description]                           │
│                              [Explored badge] [View]   │
└─────────────────────────────────────────────────────────┘
```

| Element | Description |
|---------|-------------|
| Feature name | H2 heading |
| Description | One-line summary of feature purpose |
| Explored badge | Status indicator (purple "Explored") |
| View button | Purple primary button → navigates to actual feature page |

#### Detail Panel Content Sections

Content varies by feature but typically includes:

1. **Overview** (H2)
   - Paragraph explaining what the feature does
   - Sets context for new users

2. **How to use it** / **How to use it (recommended flow)** (H2)
   - Numbered/bulleted workflow steps
   - Each step has bold title + sub-bullets with details
   - Example structure:
     ```
     • **Add high-signal sources first**
       - Your website / landing pages
       - Pitch deck, product one-pagers
       - Pricing, positioning, competitor notes
     ```

3. **What you get** / **What good looks like** (H2)
   - Bullet list of outcomes/benefits

4. **Best practices** / **Tips** (H2)
   - Bullet list of recommendations

---

### 4. Sidebar Navigation (Collapsed View)

When sidebar is collapsed, shows icon-only navigation matching the feature categories.

### 5. Getting Started Progress Chip

| Element | Current State |
|---------|---------------|
| Location | Bottom of sidebar |
| Label | "Getting started" |
| Progress | "100%" |
| Style | Button/chip with progress indicator |

---

## Feature Content Details

### Knowledge Base
- **Description:** "Upload sources and build the AI knowledge base."
- **Overview:** Foundation for everything else in the product
- **Sections:** How to use it (4 steps), What you get, Best practices

### Keyword Repository
- **Description:** TBD (need to click to view)

### Search Ranking
- **Description:** TBD

### Competitor Analysis
- **Description:** TBD

### Content Architecture
- **Description:** "Generate structure and strategy for your site/content."
- **Overview:** Design structured blueprint of pages and topics
- **Sections:** How to use it (4 steps), What good looks like, Tips

### Topics
- **Description:** TBD

### AI Optimization Questions
- **Description:** TBD

### Articles
- **Description:** TBD

### AI Optimization Answers
- **Description:** TBD

### Opportunity Agent
- **Description:** "Find market opportunities and engagement angles."
- **Overview:** Find growth opportunities and engagement strategy
- **Sections:** How to use it (4 steps), Best practices

### Social Posts
- **Description:** TBD

### Connections
- **Description:** TBD

### Social Scheduler
- **Description:** TBD

---

## User Interaction Patterns

| Action | Result |
|--------|--------|
| Click feature in list | Feature detail panel updates with selected feature info |
| Click "View" button | Navigates to actual feature page (e.g., `/projects/{id}/opportunity-agent`) |
| Hover on feature item | Shows pointer cursor |
| Click sidebar collapse | Sidebar collapses to icons only |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `feature_exploration_main.png` | Default view with Knowledge Base selected |
| `feature_exploration_content_arch.png` | Content Architecture selected |
| `feature_exploration_opportunity.png` | Opportunity Agent selected (scrolled down) |
| `feature_exploration_full.png` | Full page screenshot |

---

## UI Improvement Considerations

### Current Strengths
- Clear categorization of features
- Progress tracking provides gamification/completion incentive
- Contextual help reduces need to read separate docs
- "View" button provides clear navigation path

### Potential Improvement Areas

#### 1. Progress/Status Indicators
- **Current:** "Explored" badge only (binary state)
- **Consider:** More granular progress (e.g., "Started", "In Progress", "Mastered")
- **Consider:** Visual progress bar per category

#### 2. Feature Discovery
- **Current:** "0 features to discover" when complete
- **Consider:** What happens for new users? Need to see unexplored state

#### 3. Navigation
- **Current:** Must click each feature to see details
- **Consider:** Expandable/collapsible sections in list view
- **Consider:** Quick preview on hover

#### 4. Content Structure
- **Current:** Long scrolling content in detail panel
- **Consider:** Tabbed interface (Overview | Steps | Tips)
- **Consider:** Collapsible sections within detail panel

#### 5. Visual Hierarchy
- **Current:** Category headers blend with feature items
- **Consider:** Stronger visual separation between categories
- **Consider:** Icons for each feature (not just categories)

#### 6. Empty/New User State
- **Question:** What does this page look like for a brand new project with no exploration?
- **Need to verify:** Unexplored feature styling

#### 7. Mobile Responsiveness
- **Question:** How does the two-panel layout adapt on smaller screens?

---

## Technical Details

- **Route:** `/` (root)
- **Data:** Feature exploration status tracked per user/project
- **State:** Selected feature persisted during session
- **Navigation:** "View" button uses project-scoped URLs

---

## Related Components

- **Sidebar navigation** - Mirrors feature categories
- **Getting Started chip** - Links to this page's progress
- **Individual feature pages** - Linked via "View" button

---

## Assessment Status

| Item | Complete |
|------|----------|
| Layout documented | ✅ |
| Components identified | ✅ |
| Interactions captured | ✅ |
| Screenshots taken | ✅ |
| Improvement areas noted | ✅ |
| All feature content captured | ⬜ (partial - need to click through all) |

---

*Assessed by: Cascade*  
*Date: January 17, 2026*  
*Version: 1.0*  
*Context: Shuk Rentals → Shuk GTM v0.2 (100% explored state)*
