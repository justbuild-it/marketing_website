# AI Optimization Answers

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/aio-answers`

---

## Overview

AI Optimization Answers (AIO Answers) is where generated answers to approved questions are managed. These answers are created from the AI Optimization Questions feature and are automatically placed in the Content Architecture once approved.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ AIO Answers                                               │
│             │ Review and manage your AI-generated answers               │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────────┐ ┌─────────────────────────────────┐   │
│             │ │ ACTIONS         │ │ [Search] [Reset] [Columns]      │   │
│             │ │ [Approve]       │ ├─────────────────────────────────┤   │
│             │ │ [Reject]        │ │ Question | Answer | CA | Status │   │
│             │ │ ─────────────── │ │ ─────────────────────────────── │   │
│             │ │ Create Email    │ │ Row 1...                        │   │
│             │ │ Export to CMS   │ │ Row 2...                        │   │
│             │ ├─────────────────┤ └─────────────────────────────────┘   │
│             │ │ Linked Page     │ Total results: 2                      │
│             │ │ Overview        │                                       │
│             │ └─────────────────┘                                       │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Actions Panel
| Element | Description |
|---------|-------------|
| **Approve** | Approve selected answers |
| **Reject** | Reject selected answers |
| **Create Email Campaign** | Generate email from answer |
| **Export to CMS** | Export answer to CMS |
| **Linked Page Overview** | Shows content architecture placement |

### Data Table Columns
| Column | Sortable | Description |
|--------|----------|-------------|
| **Question** | ❌ | The original question (expandable) |
| **Answer** | ❌ | View answer button |
| **Content Architecture** | ❌ | Link to page placement |
| **Processing** | ✅ | Completed / Processing |
| **Approval** | ✅ | Review / Approved |
| **Created At** | ✅ | Creation timestamp |

---

## Example Data (Shuk Rentals)

| Question | Processing | Approval | Created |
|----------|------------|----------|---------|
| How can property management software help reduce vacancies? | Completed | Review | Jan 6, 2026 |
| How to transition from spreadsheets to property management software? | Completed | Review | Jan 5, 2026 |

**Total Answers:** 2

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Answer Management** | Review AI-generated answers |
| **Auto-Placement** | AI determines content architecture location |
| **Email Campaigns** | Generate email content from answers |
| **CMS Export** | Push answers to external CMS |
| **Approval Workflow** | Human-in-loop quality control |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `ai_optimization_answers_main.png` | Main answers list view |

---

## Related Features

- [AI Optimization Questions](./ai_optimization_questions.md) - Source questions
- [Content Architecture](./content_architecture.md) - Answer placement

