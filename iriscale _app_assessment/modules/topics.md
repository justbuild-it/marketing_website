# Topic Strategy (formerly Topics)

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-29  
> **URL Pattern:** `/projects/{id}/topic`
> **Menu Name:** Topic Strategy (renamed from Topics)
> **Note:** Feature shows empty state with Core Idea input when no topics exist; populated state with topic table when topics generated

---

## Overview

**Topic Strategy** is a content ideation and topic management feature that generates full-funnel topic plans from a single core idea. Topics are organized hierarchically with cluster topics and article topics, each categorized by funnel stage (TOFU, MOFU, BOFU, MIDF) and tracked through an approval workflow.

**New tagline:** "Turn a single idea into a full-funnel topic system for discovery, conversion, and growth."

---

## Page Layout (Updated January 2026)

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Topic Strategy                                            │
│             │ Turn a single idea into a full-funnel topic system...     │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────┬─────────────────────────────────────────┐ │
│             │ │ CORE IDEAS  │ [Search by topic]  [Reset] [Columns]    │ │
│             │ │ [Collapse]  ├─────────────────────────────────────────┤ │
│             │ │             │ Article Topic | Brief | Cluster | ...   │ │
│             │ │ Core Idea 1 │ ───────────────────────────────────────  │ │
│             │ │ [clickable] │ Row 1: Centralized Control and Insights │ │
│             │ ├─────────────┤ Row 2: Improved Collaboration...        │ │
│             │ │ ACTIONS     │ Row 3: The Problem of Data Silos        │ │
│             │ │ [Add Core]  │ Row 4: Bridging the Gaps...              │ │
│             │ │ [Approve]   │ ...                                      │ │
│             │ │ [Reject]    │ Total results: 10                        │ │
│             │ │ [Create...] │                                          │ │
│             │ └─────────────┴─────────────────────────────────────────┘ │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components (Updated January 2026)

### Core Ideas Panel (NEW - replaces Sources Panel)
| Element | Description |
|---------|-------------|
| **Collapse Panel** | Toggle Core Ideas visibility |
| **Core Ideas List** | List of core ideas used to generate topics |
| **Add Core Idea to Generate Topics** | Primary CTA button (purple) |

### Core Idea Input Modal (NEW)
| Element | Description |
|---------|-------------|
| **Modal Title** | "Core Idea Model" |
| **Heading** | "Turn One Idea Into a Full-Funnel Topic Plan" |
| **Description** | "Enter a single concept, problem, or theme. Iriscale will generate coordinated top-, middle-, and bottom-of-funnel topics that educate, convert, and support buyers." |
| **Features** | ✦ Full-funnel coverage, ✦ Audience aware prompts |
| **Core Idea Input** | Text field with 360 character limit |
| **Helper Text** | "We'll seed your topic funnel with this description." |
| **Cancel Button** | Close modal without action |
| **Generate Topics Button** | Submit core idea to generate topics |

### Actions Panel
| Element | Description |
|---------|-------------|
| **Add Core Idea** | Opens Core Idea input modal |
| **Approve** | Approve selected topics (disabled when none selected) |
| **Reject** | Reject selected topics (disabled when none selected) |
| **Create Article from Topic** | Generate article from selected topic |

### Data Table Columns (Renamed January 2026)
| Column | Old Name | Sortable | Description |
|--------|----------|----------|-------------|
| **Article Topic** | Sub Topic | ✅ | Topic title with checkbox |
| **Article Brief** | Sub Topic Overview | ❌ | Brief description of the topic |
| **Cluster Topic** | Main Topic | ✅ | Parent topic category/cluster |
| **Funnel Stage** | Type | ✅ | Funnel stage (TOFU/MOFU/BOFU/MIDF) |
| **Topic Status** | - | ✅ | Review / Approved |
| **Article Status** | - | ✅ | Not generated / Generated |

---

## Funnel Stage Types

| Type | Full Name | Description |
|------|-----------|-------------|
| **TOFU** | Top of Funnel | Awareness-stage content |
| **MOFU** | Middle of Funnel | Consideration-stage content |
| **BOFU** | Bottom of Funnel | Decision-stage content |
| **MIDF** | Mid-Funnel | Mixed consideration content |

---

## Example Data (Iriscale GTM v0.3)

### Core Idea: "Why most marketing teams start from zero every day"

| Article Topic | Cluster Topic | Funnel Stage | Topic Status | Article Status |
|---------------|---------------|--------------|--------------|----------------|
| Centralized Control and Insights | Benefits of Unified Marketing Systems | BOFU | Review | Not generated |
| Improved Collaboration and Efficiency | Benefits of Unified Marketing Systems | BOFU | Review | Not generated |
| The Problem of Data Silos | Data Silos and their Effects | TOFU | Review | Not generated |
| Bridging the Gaps with Unified Dashboards | Data Silos and their Effects | TOFU | Review | Not generated |
| Structured Content Workflows | Enhancing Content Production Efficiency | MIDF | Review | Not generated |
| Leveraging Technology | Enhancing Content Production Efficiency | MIDF | Review | Not generated |
| The Revenue Gap | Marketing and Sales Silos | TOFU | Review | Not generated |
| Implementing Shared Goals and Metrics | Marketing and Sales Silos | TOFU | Review | Not generated |
| Routine Tasks as Productivity Sinkholes | Time Wastage from Routine Manual Tasks | TOFU | Review | Not generated |
| The Role of Automation | Time Wastage from Routine Manual Tasks | TOFU | Review | Not generated |

**Total Topics:** 10

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Core Idea Generation** | Generate full-funnel topics from a single concept (NEW) |
| **Hierarchical Organization** | Cluster topics with article topics |
| **Funnel Stage Categorization** | TOFU/MOFU/BOFU/MIDF classification |
| **Full-Funnel Coverage** | Coordinated top-, middle-, and bottom-funnel topics |
| **Approval Workflow** | Review → Approved pipeline |
| **Article Creation** | Create articles directly from approved topics |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `topics_main_iriscale.png` | Main topics view (Iriscale GTM v0.3) |

---

## Related Features

- [Content Architecture](./content_architecture.md) - Topic placement
- [Articles](./articles.md) - Generated from topics
- [Social Posts](./social_posts.md) - Generated from topics

