# Social Scheduler

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/social-scheduler`

---

## Overview

Social Media Scheduler is the publishing hub for managing and scheduling social media posts. Posts created in Social Posts flow here for approval, scheduling, and publishing to connected platforms.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Social Media Scheduler                          [Refresh] │
│             │ Manage and schedule your social media posts               │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌────────┬────────┬────────┬────────┬────────┐            │
│             │ │ Draft  │Schedul │Publish │Cancell │ Failed │            │
│             │ │   0    │   0    │   0    │   0    │   0    │            │
│             │ └────────┴────────┴────────┴────────┴────────┘            │
│             │ [Search] [Approve] [Reject] [Reset] [Columns]             │
│             │ ┌─────────────────────────────────────────────────────┐   │
│             │ │ Platform│Preview│Content│Approval│Publish│Schedule │   │
│             │ │ ────────────────────────────────────────────────────│   │
│             │ │ LinkedIn│ 👁    │ Post..│Approved│Not sch│ [Post]  │   │
│             │ │ LinkedIn│ 👁    │ Short.│Review  │Not sch│   -     │   │
│             │ └─────────────────────────────────────────────────────┘   │
│             │ Total results: 2                                          │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Status Dashboard
| Status | Description |
|--------|-------------|
| **Draft** | Posts awaiting completion |
| **Scheduled** | Posts with future publish date |
| **Published** | Successfully posted |
| **Cancelled** | User-cancelled posts |
| **Failed** | Posts that failed to publish |

### Toolbar
| Element | Description |
|---------|-------------|
| **Search** | Filter posts by content |
| **Approve** | Bulk approve selected |
| **Reject** | Bulk reject selected |
| **Reset** | Clear filters |
| **Columns** | Toggle visible columns |

### Data Table Columns
| Column | Sortable | Description |
|--------|----------|-------------|
| **Platform** | ✅ | Social platform + expand button |
| **Preview** | ❌ | Preview post button |
| **Content** | ✅ | Post content snippet |
| **Approval** | ✅ | Review / Approved status |
| **Publish** | ✅ | Not scheduled / Scheduled / Published |
| **Schedule** | ❌ | Post / Schedule actions |
| **Created** | ✅ | Creation timestamp |

---

## Example Data (Shuk Rentals)

| Platform | Content | Approval | Publish | Created |
|----------|---------|----------|---------|---------|
| LinkedIn | Say goodbye to lease renewal headaches... | Approved | Not scheduled | Jan 6, 2026 |
| LinkedIn | Short notice periods often lead to rushed... | Review | Not scheduled | Jan 6, 2026 |

**Total Posts:** 2

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Status Tracking** | 5 lifecycle stages |
| **Post Preview** | Visual preview before publishing |
| **Approval Workflow** | Review → Approved pipeline |
| **Scheduling** | Future post scheduling |
| **Direct Posting** | Immediate publish option |
| **Bulk Actions** | Multi-select operations |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `social_scheduler_main.png` | Main scheduler view |

---

## Related Features

- [Social Posts](./social_posts.md) - Post creation
- [Connections](./connections.md) - Platform connections

