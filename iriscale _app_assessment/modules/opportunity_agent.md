# Opportunity Agent

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/opportunity-agent`

---

## Overview

Opportunity Agent is an AI-powered monitoring system that scans social platforms (primarily Reddit) to discover business opportunities. Agents can be configured to search for specific keywords and topics, identifying posts where the company's products/services could provide value.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Opportunity Agents                                        │
│             │ Configure and manage opportunity monitoring agents        │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ [Expand All] | [Collapse All]  [Auto-refresh ▼] [Refresh] │
│             │ [Active Agents ▼]                        [+ New Agent]    │
│             │ ┌─────────────────────────────────────────────────────┐   │
│             │ │ Property Management Software trial agent            │   │
│             │ │ [Opportunities] [Edit] [...]                        │   │
│             │ │ ┌──────────┬──────────┬────────────┬──────────┐     │   │
│             │ │ │ 30       │ 8        │ 6m 36s     │ ✓ Done   │     │   │
│             │ │ │ Opps     │ Sources  │ Process    │ Status   │     │   │
│             │ │ │ from 543 │ subreddit│ 8 methods  │          │     │   │
│             │ │ └──────────┴──────────┴────────────┴──────────┘     │   │
│             │ │ Created: Jan 8, 2026    Updated: Jan 17, 2026       │   │
│             │ └─────────────────────────────────────────────────────┘   │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Header Controls
| Element | Description |
|---------|-------------|
| **Expand/Collapse All** | Toggle all agent cards |
| **Auto-refresh** | 10s, 30s, 1m, 5m intervals |
| **Refresh** | Manual refresh |
| **Filter** | Active/All/Completed/Processing/Failed |
| **New Agent** | Create new monitoring agent |

### Agent Card
| Element | Description |
|---------|-------------|
| **Agent Name** | Descriptive title |
| **Opportunities Button** | View discovered opportunities |
| **Edit Button** | Modify agent configuration |
| **More Menu** | Additional actions |

### Agent Metrics
| Metric | Description |
|--------|-------------|
| **Opportunities** | Number found / total posts scanned |
| **Sources** | Number of subreddits monitored |
| **Process Time** | Execution duration and methods |
| **Status** | Completed / Processing / Failed |

---

## Example Data (Shuk Rentals)

### Agent: Property Management Software trial agent
| Metric | Value |
|--------|-------|
| **Opportunities** | 30 from 543 posts |
| **Sources** | 8 subreddits |
| **Process Time** | 6m 36s (8 methods) |
| **Status** | Completed |
| **Created** | Jan 8, 2026 |
| **Updated** | Jan 17, 2026 |

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Multi-Platform Scanning** | Reddit (primary), expandable |
| **Keyword Monitoring** | Track specific terms |
| **Opportunity Scoring** | AI identifies relevant posts |
| **Auto-Refresh** | Continuous monitoring |
| **Multiple Agents** | Different keyword sets |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `opportunity_agent_main.png` | Main agent overview |

---

## Related Features

- [Social Posts](./social_posts.md) - Respond to opportunities
- [Keyword Repository](./keyword_repository.md) - Keyword source

