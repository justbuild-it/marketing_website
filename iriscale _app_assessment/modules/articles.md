# Articles

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/articles`

---

## Overview

The Articles feature (internally labeled "Content") is a content management hub where users can review, edit, and publish AI-generated articles. Articles are created from the Content Architecture feature and can be approved or rejected through a workflow system.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Content                                                   │
│             │ Review, edit, and publish your content                    │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────┐ ┌───────────────────────────────────────┐ │
│             │ │ ACTIONS     │ │ [Search] [Reset] [Columns]            │ │
│             │ │ Create      │ ├───────────────────────────────────────┤ │
│             │ │ Article     │ │ Title | Desc | CA | Process | Approve │ │
│             │ │ ─────────── │ │ ───────────────────────────────────── │ │
│             │ │ Selected: 0 │ │ Row 1...                              │ │
│             │ │ [Approve]   │ │ Row 2...                              │ │
│             │ │ [Reject]    │ │ Row 3...                              │ │
│             │ └─────────────┘ └───────────────────────────────────────┘ │
│             │                 Total results: 5                          │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "Content" |
| **Subtitle** | "Review, edit, and publish your content" |

### Actions Panel
| Element | Description |
|---------|-------------|
| **Create Article** | Manually create new article |
| **Selected Count** | Shows number of selected items |
| **Approve** | Bulk approve selected articles |
| **Reject** | Bulk reject selected articles |

### Data Table Columns
| Column | Sortable | Description |
|--------|----------|-------------|
| **Title** | ✅ | Article title (with checkbox) |
| **Description** | ❌ | Brief content description |
| **Content Architecture** | ❌ | Link to page in architecture |
| **Processing** | ✅ | Completed / Processing status |
| **Approval** | ✅ | Review / Approved status |
| **Created At** | ✅ | Creation timestamp |
| **Actions** | ❌ | Row-level actions menu |

---

## Example Data (Shuk Rentals)

| Title | Description | Processing | Approval |
|-------|-------------|------------|----------|
| Getting Started as a Landlord | Foundational educational guide for new landlords | Completed | Review |
| Lease Management Basics | Educational guide covering lease creation | Completed | Review |
| Rent Collection Strategies | Strategic guide comparing payment methods | Completed | Review |
| Rental Management Guides | Clustered hub organizing 22 guides | Completed | Review |
| Security Deposit Laws by State | Reference guide for deposit regulations | Completed | Review |

**Total Articles:** 5

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Article Creation** | Manual or AI-generated articles |
| **Content Architecture Link** | Direct link to page in site structure |
| **Approval Workflow** | Review → Approved pipeline |
| **Bulk Actions** | Multi-select approve/reject |
| **Search & Filter** | Find articles by title/description |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `articles_main.png` | Main articles list view |

---

## Related Features

- [Content Architecture](./content_architecture.md) - Source of article generation
- [AI Optimization Answers](./ai_optimization_answers.md) - Related content type

