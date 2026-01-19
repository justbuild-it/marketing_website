# Getting Started Flyout Panel

**Location:** Bottom of left sidebar → "Getting started X%" button  
**Trigger:** Click on the Getting Started chip  
**Type:** Flyout/popup panel overlaying main content  
**Tags:** 
- [x] `TRAINING` - Primary onboarding mechanism
- [x] `VIDEO` - Good for product tour demos
- [x] `MARKETING` - Shows guided onboarding approach
- [ ] `PROMO`

> **Note:** Flagged for UI improvements

---

## Overview

The Getting Started flyout provides a quick-access checklist of all platform features with their exploration status. It serves as a gamified onboarding tool to encourage users to discover all features.

---

## UI Components

### 1. Trigger Button (Sidebar Bottom)

```
┌──────────────────────────┐
│ Getting started    100%  │
└──────────────────────────┘
```

| Element | Description |
|---------|-------------|
| Label | "Getting started" |
| Progress | Percentage (e.g., "100%") |
| Position | Fixed at bottom of sidebar |
| Style | Dark background chip/button |

---

### 2. Flyout Panel Header

```
┌─────────────────────────────────────┐
│ GETTING STARTED                     │
│ 100% explored                       │
│ 13 of 13 features                   │
└─────────────────────────────────────┘
```

| Element | Description |
|---------|-------------|
| Title | "GETTING STARTED" (small caps) |
| Progress text | "100% explored" (large/bold) |
| Feature count | "13 of 13 features" |

---

### 3. Feature List Items

Each feature appears as a row item:

```
┌─────────────────────────────────────────────────┐
│ [✓] Knowledge Base                        OPEN  │
│     INTELLIGENCE & RESEARCH                     │
└─────────────────────────────────────────────────┘
```

| Element | Description |
|---------|-------------|
| Status icon | Checkmark (green circle) when explored |
| Feature name | Primary text (bold) |
| Category label | Secondary text (muted, category name) |
| Action | "OPEN" link/button on right |

---

## Complete Feature List (13 items)

| # | Feature | Category | Status Shown |
|---|---------|----------|--------------|
| 1 | Knowledge Base | INTELLIGENCE & RESEARCH | ✓ Explored |
| 2 | Keyword Repository | INTELLIGENCE & RESEARCH | ✓ Explored |
| 3 | Search Ranking | INTELLIGENCE & RESEARCH | ✓ Explored |
| 4 | Competitor Analysis | INTELLIGENCE & RESEARCH | ✓ Explored |
| 5 | Content Architecture | STRATEGY & PLANNING | ✓ Explored |
| 6 | Topics | STRATEGY & PLANNING | ✓ Explored |
| 7 | AI Optimization Questions | STRATEGY & PLANNING | ✓ Explored |
| 8 | Articles | CONTENT CREATION | ✓ Explored |
| 9 | AI Optimization Answers | CONTENT CREATION | ✓ Explored |
| 10 | Opportunity Agent | OPPORTUNITY & ENGAGEMENT | ✓ Explored |
| 11 | Social Posts | PROMOTE | ✓ Explored |
| 12 | Connections | PROMOTE | ✓ Explored |
| 13 | Social Scheduler | PROMOTE | ✓ Explored |

---

## Interaction Patterns

| Action | Result |
|--------|--------|
| Click "Getting started" chip | Opens flyout panel |
| Click outside flyout | Closes flyout (assumed) |
| Click "OPEN" on feature | Navigates to that feature page |
| Click feature row | Likely navigates to feature page |

---

## Visual Design Details

### Color Scheme
- **Background:** Dark (navy/charcoal)
- **Text:** White/light
- **Checkmarks:** Green circles with white check
- **"OPEN" links:** Muted/secondary color

### Layout
- **Position:** Appears to overlay above the trigger button
- **Width:** Approximately matches sidebar width
- **Height:** Scrollable list if needed
- **Z-index:** Above main content

---

## Screenshots

| File | Description |
|------|-------------|
| `getting_started_flyout.png` | Full page with flyout open |
| `getting_started_flyout_full.png` | Cropped flyout panel only |

---

## Current State Analysis

### Strengths
1. **Gamification** - Progress percentage creates completion incentive
2. **Quick access** - Always visible in sidebar
3. **Feature discovery** - Lists all 13 core features in one place
4. **Direct navigation** - "OPEN" buttons provide quick access
5. **Category context** - Shows which category each feature belongs to

### Weaknesses / Improvement Opportunities

#### 1. Visual Hierarchy
- **Issue:** All items look the same (flat list)
- **Recommendation:** Group items by category with visual separators or collapsible sections

#### 2. Progress Indication Per Item
- **Current:** Binary (explored/not explored)
- **Recommendation:** Consider more granular states:
  - Not started
  - In progress
  - Completed
  - Mastered (used X times)

#### 3. Onboarding Flow Guidance
- **Issue:** Just a checklist, no suggested order
- **Recommendation:** Add numbered steps or "Start here" / "Next" indicators
- **Recommendation:** Highlight recommended first feature for new users

#### 4. Empty State / New User Experience
- **Question:** What does 0% explored look like?
- **Recommendation:** Ensure encouraging messaging for new users
- **Recommendation:** Consider adding brief descriptions in flyout

#### 5. Completion Celebration
- **Question:** What happens at 100%?
- **Recommendation:** Add celebration animation/message
- **Recommendation:** Offer "What's next" guidance or advanced features

#### 6. Dismissal Behavior
- **Question:** How to close? Click outside? X button?
- **Recommendation:** Clear close affordance if not present

#### 7. Mobile Experience
- **Question:** How does flyout work on mobile?
- **Recommendation:** Ensure responsive design for smaller screens

#### 8. Feature Descriptions
- **Issue:** No description in flyout, only name + category
- **Recommendation:** Add brief one-liner or hover tooltip

#### 9. Action Clarity
- **Issue:** "OPEN" vs clicking row - which navigates?
- **Recommendation:** Clarify interaction model

---

## Improvement Recommendations Summary

### Quick Wins
1. Add category grouping/separators to the list
2. Add brief feature descriptions (1 line each)
3. Ensure clear close button/affordance

### Medium Effort
4. Implement suggested order with "Start here" indicator
5. Add celebration state at 100% completion
6. Add progress states beyond binary (started/in-progress/complete)

### Larger Improvements
7. Interactive onboarding tutorial overlay
8. Context-sensitive tips based on what user hasn't explored
9. Time-based nudges for unexplored features

---

## Relationship to Feature Exploration Page

| Getting Started Flyout | Feature Exploration Page |
|------------------------|--------------------------|
| Quick checklist view | Full detail view |
| Shows progress + navigation | Shows progress + help content |
| Always accessible (sidebar) | Dedicated page (root URL) |
| No feature descriptions | Full feature descriptions |
| "OPEN" action only | "View" + detail panel |

**Recommendation:** These should complement each other. Consider:
- Clicking feature in flyout → opens Feature Exploration with that feature selected
- Or: flyout shows mini-preview on hover

---

## Technical Notes

- Flyout triggered by click on sidebar button
- Panel appears as overlay (not route change)
- Feature exploration status tracked per project
- List matches sidebar navigation structure

---

## Assessment Status

| Item | Complete |
|------|----------|
| Layout documented | ✅ |
| Components identified | ✅ |
| Interactions captured | ✅ |
| Screenshots taken | ✅ |
| Improvement areas noted | ✅ |
| New user state captured | ⬜ (need fresh project) |

---

*Assessed by: Cascade*  
*Date: January 17, 2026*  
*Version: 1.0*  
*Context: Shuk Rentals → Shuk GTM v0.2 (100% explored state)*
