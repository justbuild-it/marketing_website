# AI Optimization Questions

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/ai-optimizations`

---

## Overview

AI Optimization Questions is a feature that identifies and manages questions customers ask AI systems. The platform uses APIs and research to generate relevant questions based on approved keywords. Users can review, approve, and generate optimized answers that are automatically placed in the best location within the content architecture.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ AI Optimizations                                          │
│             │ Questions your customers ask AI                           │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────┐ ┌─────────────────────────────────────┐   │
│             │ │ ACTIONS     │ │ Search by keyword or question...    │   │
│             │ │ AI Answer   │ ├─────────────────────────────────────┤   │
│             │ │ Generation  │ │ [Reset] [Columns]                   │   │
│             │ │ ─────────── │ ├────────────────────────────────────────┤│
│             │ │ [Approve]   │ │ Question │ Keyword │ Answer │ Type  │  ││
│             │ │ [Reject]    │ │          │         │        │ Approv│  ││
│             │ └─────────────┘ │ Row 1... │         │        │       │  ││
│             │                 │ Row 2... │         │        │       │  ││
│             │                 │ Row 3... │         │        │       │  ││
│             │                 └──────────────────────────────────────┘  │
│             │                 Total results: 19                         │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "AI Optimizations" |
| **Subtitle** | "Questions your customers ask AI" |

### Actions Panel
| Element | Description |
|---------|-------------|
| **AI Answer Generation** | Trigger answer generation for selected questions |
| **Approve** | Approve selected questions for answer generation |
| **Reject** | Reject selected questions |
| **Collapse** | Toggle panel visibility |

### Toolbar
| Element | Description |
|---------|-------------|
| **Search** | Filter by keyword or question phrase |
| **Reset** | Clear all filters and sorting |
| **Columns** | Toggle visible columns |

### Data Table
| Column | Sortable | Description |
|--------|----------|-------------|
| **Question Phrase** | ✅ | The customer question (checkbox for selection) |
| **Keyword** | ✅ | Associated keyword from repository |
| **Answer** | ❌ | Answer status (- if none generated) |
| **Type** | ✅ | Source: AI or People Also Ask |
| **Q Approval** | ✅ | Review / Approved status |
| **Created At** | ✅ | Question creation timestamp |

---

## Feature Details (Confirmed)

### Question Source
| Aspect | Details |
|--------|---------|
| **Generation Method** | AI uses APIs and research |
| **Input** | Approved keywords from repository |
| **Types** | AI-generated, People Also Ask |

### Answer Generation Workflow
| Step | Description |
|------|-------------|
| 1 | User reviews generated questions |
| 2 | User approves relevant questions |
| 3 | User selects keyword |
| 4 | User clicks "Generate Answer" |
| 5 | AI creates optimized answer |

### Integration with Content Architecture
| Aspect | Details |
|--------|---------|
| **Placement** | AI assesses best location in content architecture |
| **Automation** | Automatic placement once answer approved |
| **Destination** | Website content based on architecture structure |

---

## Example Data (Shuk Rentals)

### Sample Questions
| Question | Keyword | Type | Status |
|----------|---------|------|--------|
| Can property management software integrate with marketing tools? | property management software | AI | Review |
| How can property management software help reduce vacancies? | property management software | AI | Approved |
| How does Shuk compare to other property management software? | property management software | AI | Review |
| Is there any free property management software? | property management software | People Also Ask | Review |
| What is the 2% rule for rental property? | property management software | People Also Ask | Review |

### Statistics
| Metric | Value |
|--------|-------|
| **Total Questions** | 19 |
| **Approved** | ~4 |
| **Pending Review** | ~15 |

---

## Data Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                    Approved Keywords                                 │
│                 (from Keyword Repository)                            │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    AI Question Generation                            │
│              - API research                                          │
│              - People Also Ask extraction                            │
│              - AI-powered question creation                          │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    Question Review Queue                             │
│              - User reviews questions                                │
│              - Approve or reject                                     │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    Answer Generation                                 │
│              - AI creates optimized answer                           │
│              - User reviews and approves                             │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    Content Architecture Placement                    │
│              - AI determines best location                           │
│              - Auto-placement on website                             │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **AI-Powered Question Discovery** | Automated question generation from keywords |
| **Multiple Sources** | AI generation + People Also Ask extraction |
| **Approval Workflow** | Human-in-loop for quality control |
| **Smart Answer Generation** | Context-aware answer creation |
| **Auto-Placement** | AI determines optimal website location |
| **Bulk Actions** | Approve/reject multiple questions |

---

## User Workflow

### 1. Review Questions
```
Navigate to AI Optimizations → Review question list → Check relevance
```

### 2. Approve Questions
```
Select questions → Click "Approve" → Questions marked for answer generation
```

### 3. Generate Answers
```
Select approved questions → Choose keyword → Click "AI Answer Generation"
```

### 4. Answer Placement
```
Review generated answer → Approve → AI places in content architecture
```

---

## Value Propositions

| For Role | Value |
|----------|-------|
| **Content Teams** | Pre-researched questions to answer |
| **SEO Managers** | Target "People Also Ask" opportunities |
| **Marketing Teams** | Customer-centric content ideas |
| **Product Teams** | Understand customer queries |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `ai_optimization_questions_main.png` | Main question list view |

---

## UI Improvement Opportunities

### High Priority
1. **Question Grouping** - Group questions by keyword/topic
2. **Priority Indicators** - Show search volume or importance
3. **Answer Preview** - Preview before generation

### Medium Priority
4. **Batch Approve by Keyword** - Approve all questions for a keyword
5. **Duplicate Detection** - Flag similar questions
6. **Export Options** - Export questions to CSV

---

## Related Features

- [Keyword Repository](./keyword_repository.md) - Source of keywords
- [Content Architecture](./content_architecture.md) - Answer placement
- [AI Optimization Answers](./ai_optimization_answers.md) - Generated answers
- [Articles](./articles.md) - Content generation

