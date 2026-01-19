# Keyword Repository

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/keywords`

---

## Overview

The Keyword Repository is a centralized hub for managing SEO and marketing keywords. It uses sophisticated AI agents with multiple APIs (including Google keyword data) to generate a comprehensive set of keywords, while also allowing manual entry for pre-existing keyword lists.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Keyword Repository                                        │
│             │ Use in all AI tools and workflows                         │
│             │ Add keywords information to the AI knowledge base...      │
│   Sidebar   ├───────────────┬───────────────────────────────────────────┤
│             │ Sources       │ Search | Reset | Columns                  │
│             │ + Add Source  ├───────────────────────────────────────────┤
│             │               │ Keyword Table                             │
│             ├───────────────┤ - Keyword                                 │
│             │ Actions       │ - Primary                                 │
│             │ - Approve     │ - Volume                                  │
│             │ - Reject      │ - Competition                             │
│             │ - AI Opt Ques │ - Category                                │
│             │ - Expand PKWs │ - Products/Services                       │
│             ├───────────────┤ - Search Intent                           │
│             │ Link Products │ - CPC                                     │
│             │ & Services    │ - Approval                                │
│             │               │ - Is Competitor                           │
│             │               ├───────────────────────────────────────────┤
│             │               │ Total results: 458                        │
└─────────────┴───────────────┴───────────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "Keyword Repository" |
| **Subtitle** | "Use in all AI tools and workflows" |
| **Description** | "Add keywords information to the AI knowledge base and start creating campaigns immediately" |

### Left Panel - Sources
| Element | Description |
|---------|-------------|
| **Add Source Button** | Opens source input interface |
| **Source Types** | Text file, CSV file, or pasted text |
| **Current State** | "No sources added yet" (when empty) |

### Left Panel - Actions
| Action | Function |
|--------|----------|
| **Approve** | Marks selected keywords as approved for use throughout the tool |
| **Reject** | Marks selected keywords as rejected (excluded from use) |
| **AI Optimization: Questions** | Researches frequently asked questions related to selected keywords |
| **Expand Primary KW's** | *(Deprecated - being replaced by Advanced AI Keyword Agent)* |

### Left Panel - Link Products & Services
| Element | Description |
|---------|-------------|
| **Dropdown** | Search combobox for products & services |
| **Button** | "Select a keyword first" (disabled until selection) |
| **Purpose** | Associates keywords with specific products/services |

### Main Panel - Toolbar
| Element | Description |
|---------|-------------|
| **Search** | Text input: "Search by keyword..." |
| **Reset** | Clears all filters and sorting |
| **Columns** | Toggle visible columns |

### Main Panel - Data Table

#### Column Definitions
| Column | Type | Description |
|--------|------|-------------|
| **Keyword** | Text + Checkbox | The search term; checkbox for selection |
| **Primary** | Checkbox | Marks as primary keyword |
| **Volume** | Number | Monthly search volume |
| **Competition** | Badge | High (red) / Low (yellow) indicator |
| **Category** | Text | Product category grouping |
| **Products/Services** | Text | Linked product or service name |
| **Search Intent** | Badge | navigational / commercial / informational |
| **CPC** | Currency | Cost per click value |
| **Approval** | Status | Approved (green) / Review (yellow) |
| **Is Competitor** | Yes/No | Whether keyword came from competitor analysis |

---

## Example Data (Shuk Rentals)

| Keyword | Volume | Competition | Products/Services | Intent | CPC | Status | Competitor |
|---------|--------|-------------|-------------------|--------|-----|--------|------------|
| affordable renters insurance | 74,000 | high | Renters Insurance | navigational | $32.78 | Approved | Yes |
| property management software | 27,100 | low | Property Management | navigational | $118.82 | Approved | Yes |
| innago | 22,200 | low | - | navigational | $5.18 | Review | No |
| background check for tenants | 12,100 | high | Application & Screenings | navigational | $15.09 | Review | Yes |
| background check for renters | 12,100 | high | TransUnion Tenant Screening Reports | navigational | $15.09 | Review | Yes |
| tenant screening service | 8,100 | low | TransUnion Tenant Screening Reports | navigational | $13.97 | Review | Yes |
| online rent payment | 6,600 | low | Online Rent Collection | navigational | $11.33 | Review | Yes |
| buildium property management software | 4,400 | low | - | navigational | $35.22 | Review | No |
| credit check for renters | 2,900 | high | Tenant screening | commercial | $15.70 | Review | No |

**Total Keywords:** 458

---

## Feature Details (Confirmed)

### Keyword Generation
| Aspect | Details |
|--------|---------|
| **AI Research** | Sophisticated AI agent using multiple APIs including Google keyword data |
| **Research Methods** | Multiple methods to develop world-class keyword sets |
| **Manual Entry** | Supported - for pre-existing keywords or known customer searches |

### Sources Panel
| Aspect | Details |
|--------|---------|
| **Supported Formats** | Text file, CSV file, or pasted text |
| **Impact on Generation** | Minor influence during AI assessment (e.g., competitor source identification) |

### Approval Workflow
| Status | Meaning |
|--------|---------|
| **Review** | Pending user decision |
| **Approved** | Keyword used throughout the tool |
| **Rejected** | Keyword excluded from use |

### AI Optimization: Questions
| Aspect | Details |
|--------|---------|
| **Trigger** | Select keyword(s) → Click "AI Optimization: Questions" button |
| **Action** | Researches frequently asked questions related to selected keywords |
| **Output** | Results appear in "AI Optimization Questions" menu page |
| **Purpose** | Find questions users ask AI search tools (ChatGPT, etc.) |
| **Value** | Generate answers for website publication to capture AI-driven search traffic |

### Expand Primary KW's
| Aspect | Details |
|--------|---------|
| **Status** | Being deprecated |
| **Replacement** | Advanced AI Keyword Agent |

### Products & Services Linking
| Aspect | Details |
|--------|---------|
| **Function** | Auto-assigns keywords to company products/services |
| **Downstream Impact** | Marketing agents know which keywords to use for each product/service |
| **Value** | Ensures targeted keyword usage in content creation |

### Competitor Flag
| Aspect | Details |
|--------|---------|
| **Source** | Competitive research from Knowledge Base screen |
| **Logic** | Keywords from competitor analysis that don't already exist for company |
| **Purpose** | Identify keywords competitors target for same products |

---

## Data Flow

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  Knowledge Base │    │   AI Research   │    │  Manual Entry   │
│  (Competitors)  │    │  (Google APIs)  │    │  (CSV/Text)     │
└────────┬────────┘    └────────┬────────┘    └────────┬────────┘
         │                      │                      │
         └──────────────────────┼──────────────────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │  Keyword Repository   │
                    │  (458 keywords)       │
                    └───────────┬───────────┘
                                │
         ┌──────────────────────┼──────────────────────┐
         │                      │                      │
         ▼                      ▼                      ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│ AI Optimization │    │ Products &      │    │ Content         │
│ Questions       │    │ Services Link   │    │ Creation        │
└────────┬────────┘    └────────┬────────┘    └─────────────────┘
         │                      │
         ▼                      ▼
┌─────────────────┐    ┌─────────────────┐
│ AI Q&A Feature  │    │ Marketing       │
│ (Answers)       │    │ Agents          │
└─────────────────┘    └─────────────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **AI-Powered Research** | Sophisticated keyword discovery using multiple APIs |
| **Bulk Management** | Handle hundreds of keywords with sorting/filtering |
| **Approval Workflow** | Control which keywords are active |
| **Product Association** | Link keywords to products for targeted marketing |
| **Competitor Intelligence** | Identify competitor keyword strategies |
| **Question Discovery** | Find AI-search questions for content opportunities |

---

## User Workflow

### 1. Initial Keyword Generation
```
Knowledge Base Complete → AI generates keywords → Keywords populate repository
```

### 2. Review & Approve
```
Review keywords → Approve valuable ones → Reject irrelevant ones
```

### 3. Link to Products
```
Select keyword → Search products/services → Link to relevant product
```

### 4. Generate Questions
```
Select keyword(s) → Click "AI Optimization: Questions" → Review in AI Questions page
```

---

## Value Propositions

| For Role | Value |
|----------|-------|
| **SEO Managers** | Comprehensive keyword research with competition/volume data |
| **Content Teams** | Clear direction on what keywords to target |
| **Marketing Teams** | Product-keyword associations for campaigns |
| **Executives** | Competitive intelligence on keyword strategies |

---

## Integration Points

| Connects To | Purpose |
|-------------|---------|
| **Knowledge Base** | Source of competitor keyword data |
| **AI Optimization Questions** | Generates questions from keywords |
| **Products & Services** | Links keywords to business offerings |
| **Content Creation** | Informs keyword targeting |
| **Marketing Agents** | Provides keyword context for automation |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `keyword_repository_main.png` | Main interface with keyword table |

---

## UI Improvement Opportunities

### High Priority
1. **Visual Status Indicators** - Add icons alongside color for accessibility
2. **Bulk Actions** - Select all/none, bulk approve/reject
3. **Export Functionality** - Export filtered keywords to CSV

### Medium Priority
4. **Grouping Options** - Group by product, competition level, or intent
5. **Trend Data** - Show volume trends over time
6. **Quick Filters** - Preset filters for common views (high volume, approved only)

### Low Priority
7. **Drag-Drop Reordering** - Prioritize keyword list manually
8. **Notes/Tags** - Add custom notes or tags to keywords
9. **Comparison View** - Side-by-side keyword comparison

---

## Related Features

- [Knowledge Base](./knowledge_base.md) - Source of competitor data
- [AI Optimization Questions](./ai_optimization_questions.md) - Downstream question generation
- [Search Ranking](./search_ranking.md) - Track keyword performance

