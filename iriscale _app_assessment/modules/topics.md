# Topics

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/topic`
> **Note:** Feature requires topic data; returned 404 on Shuk Rentals (no topics generated), works on Iriscale GTM v0.3

---

## Overview

Topics is a content ideation and topic management feature that generates sub-topics from various sources (URLs, text). Topics are organized hierarchically with main topics and sub-topics, each categorized by funnel stage (TOFU, MOFU, BOFU, MIDF) and tracked through an approval workflow.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Topic                                                     │
│             │ Generate topics, create content, publish, win             │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────┬─────────────────────────────────────────┐ │
│             │ │ SOURCES     │ [Search by topic]  [Reset] [Columns]    │ │
│             │ │ [Collapse]  ├─────────────────────────────────────────┤ │
│             │ │             │ Sub Topic | Overview | Main | Type |... │ │
│             │ │ Source 1    │ ───────────────────────────────────────  │ │
│             │ │ [COMPLETED] │ Row 1: Centralized Control and Insights │ │
│             │ ├─────────────┤ Row 2: Improved Collaboration...        │ │
│             │ │ ACTIONS     │ Row 3: The Problem of Data Silos        │ │
│             │ │ [Topic Gen] │ Row 4: Bridging the Gaps...              │ │
│             │ │ [Approve]   │ ...                                      │ │
│             │ │ [Reject]    │ Total results: 10                        │ │
│             │ │ [Create...] │                                          │ │
│             │ └─────────────┴─────────────────────────────────────────┘ │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Sources Panel
| Element | Description |
|---------|-------------|
| **Collapse Panel** | Toggle sources visibility |
| **Source List** | URLs/text used for topic generation |
| **Status Badge** | COMPLETED / PROCESSING |

### Actions Panel
| Element | Description |
|---------|-------------|
| **Topic Generation** | Generate topics from source |
| **Approve** | Approve selected topics |
| **Reject** | Reject selected topics |
| **Create Article** | Generate article from topic |
| **Create GEO content** | Generate geo-targeted content |
| **Create Social Post** | Generate social post from topic |

### Add New Source
| Element | Description |
|---------|-------------|
| **Source Input** | Text box for URL or text |
| **Generate Source** | Process source for topics |
| **Cancel** | Cancel source addition |

### Data Table Columns
| Column | Sortable | Description |
|--------|----------|-------------|
| **Sub Topic** | ✅ | Topic title with checkbox |
| **Sub Topic Overview** | ❌ | Brief description |
| **Main Topic** | ✅ | Parent topic category |
| **Type** | ✅ | Funnel stage (TOFU/MOFU/BOFU/MIDF) |
| **Topic Status** | ✅ | Review / Approved |
| **Article Status** | ❌ | Article creation status |
| **Topic Sources** | ❌ | Source count link |
| **Sub-Topic Sources** | ❌ | Sub-source count |
| **Related Data** | ❌ | Related items count |

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

### Source: "Why most marketing teams start from zero every day"

| Sub Topic | Main Topic | Type | Status |
|-----------|------------|------|--------|
| Centralized Control and Insights | Benefits of Unified Marketing Systems | BOFU | Review |
| Improved Collaboration and Efficiency | Benefits of Unified Marketing Systems | BOFU | Review |
| The Problem of Data Silos | Data Silos and their Effects | TOFU | Review |
| Bridging the Gaps with Unified Dashboards | Data Silos and their Effects | TOFU | Review |
| Structured Content Workflows | Enhancing Content Production Efficiency | MIDF | Review |
| Leveraging Technology | Enhancing Content Production Efficiency | MIDF | Review |
| The Revenue Gap | Marketing and Sales Silos | TOFU | Review |
| Implementing Shared Goals and Metrics | Marketing and Sales Silos | TOFU | Review |
| Routine Tasks as Productivity Sinkholes | Time Wastage from Routine Manual Tasks | TOFU | Review |
| The Role of Automation | Time Wastage from Routine Manual Tasks | TOFU | Review |

**Total Topics:** 10

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Source-Based Generation** | Generate topics from URLs or text |
| **Hierarchical Organization** | Main topics with sub-topics |
| **Funnel Stage Categorization** | TOFU/MOFU/BOFU/MIDF classification |
| **Multi-Content Creation** | Articles, GEO content, Social posts |
| **Approval Workflow** | Review → Approved pipeline |
| **Related Data Links** | Connected sources and data |

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

