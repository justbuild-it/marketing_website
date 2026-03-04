# Keyword Repository

> **Status:** ✅ Documented  
> **Last Updated:** 2026-03-01  
> **URL Pattern:** `/projects/{id}/keywords`

---

## Overview

The Keyword Repository is a centralized hub for managing SEO and marketing keywords. It uses sophisticated AI agents with multiple APIs (including Google keyword data) to generate a comprehensive set of keywords, while also allowing manual entry for pre-existing keyword lists.

**March 2026 Update:** Keywords now include an AI-generated **Priority** level (P1/P2/P3) and a **Priority Score** (0–1) that ranks each keyword's relevance to the company. Keywords processed through this AI priority pipeline are **auto-approved**, accelerating customer account setup.

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
│             │ Actions       │ - Priority (P1/P2/P3)                     │
│             │ - Approve     │ - Priority Score (0–1)                    │
│             │ - Reject      │ - AI Questions                            │
│             │ - AI Opt Ques │ - Volume                                  │
│             ├───────────────┤ - Competition                             │
│             │ Link Products │ - Products/Services                       │
│             │ & Services    │ - CPC                                     │
│             │               │ - Approval                                │
│             │               ├───────────────────────────────────────────┤
│             │               │ Total results: 332                        │
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

#### Column Definitions (Default Visible)
| Column | Type | Description |
|--------|------|-------------|
| **Keyword** | Text + Checkbox | The search term; checkbox for selection |
| **Priority** | Badge (P1/P2/P3) | AI-assigned priority level; clickable dropdown to change (P1, P2, P3, Unprioritized) |
| **Priority Score** | Number (0–1) | AI-calculated relevance score; hover shows "Relevancy reasoning" tooltip with AI explanation |
| **AI Questions** | Link / Button | "View (N)" link to existing questions, or "Submit" button to generate new ones |
| **Volume** | Number | Monthly search volume |
| **Competition** | Badge | High (red) / Medium / Low (yellow) indicator |
| **Products/Services** | Text | Linked product or service name |
| **CPC** | Currency | Cost per click value |
| **Approval** | Status | Approved (green) / Review (yellow) |

#### Hidden Columns (Available via Columns toggle)
| Column | Type | Description |
|--------|------|-------------|
| **Search Intent** | Badge | navigational / commercial / informational |
| **High Bid** | Currency | High bid estimate |
| **Low Bid** | Currency | Low bid estimate |
| **Is Competitor** | Yes/No | Whether keyword came from competitor analysis |
| **SE Type** | Text | Search engine type |
| **Language** | Text | Keyword language |
| **Created At** | Date | When keyword was created |

#### Removed Columns (since Jan 2026)
| Column | Notes |
|--------|-------|
| **Primary** | Replaced by Priority system |
| **Category** | No longer in column list |

---

## Example Data (Iriscale GTM v0.3)

| Keyword | Priority | Score | AI Questions | Volume | Competition | Products/Services | CPC | Approval |
|---------|----------|-------|-------------|--------|-------------|-------------------|-----|----------|
| ai seo tools | P1 | 0.87 | View (15) | 2,400 | low | Programmatic SEO +1 | $30.63 | Approved |
| best ai seo tools | P1 | 0.85 | View (20) | 720 | low | Programmatic SEO +1 | $22.51 | Approved |
| ai for marketing | P1 | 0.84 | View (24) | 4,400 | medium | Social Studio +1 | $18.56 | Approved |
| generative ai platform | P1 | 0.82 | View (35) | 9,900 | low | AI Visibility Analytics +1 | $15.91 | Approved |
| ai in digital marketing | P1 | 0.82 | View (20) | 2,400 | medium | Social Studio +1 | $18.92 | Approved |
| marketing ai | P2 | 0.80 | Submit | 1,600 | high | Social Studio +1 | $22.89 | Approved |
| free keyword research tool | P2 | 0.78 | Submit | 8,100 | medium | Keywords Explorer | $9.27 | Approved |

**Total Keywords:** 332
**Project:** Iriscale GTM v0.3

---

## Feature Details (Confirmed)

### Keyword Generation
| Aspect | Details |
|--------|---------|
| **AI Research** | Sophisticated AI agent using multiple APIs including Google keyword data |
| **Research Methods** | Multiple methods to develop world-class keyword sets |
| **Manual Entry** | Supported - for pre-existing keywords or known customer searches |

### Priority System (NEW - March 2026)
| Aspect | Details |
|--------|---------|
| **Priority Levels** | P1 (highest), P2, P3, Unprioritized |
| **Priority Score** | 0–1 numerical score generated by AI algorithm |
| **Score Reasoning** | Hover over score to see AI-generated "Relevancy reasoning" tooltip |
| **Auto-Approval** | Keywords processed through the priority pipeline are automatically approved |
| **Purpose** | Selects the best keyword in any situation; accelerates customer account setup |
| **User Override** | Priority level can be manually changed via dropdown on each keyword |

### Sources Panel
| Aspect | Details |
|--------|---------|
| **Supported Formats** | Text file, CSV file, or pasted text |
| **Impact on Generation** | Minor influence during AI assessment (e.g., competitor source identification) |

### Approval Workflow
| Status | Meaning |
|--------|---------|
| **Review** | Pending user decision |
| **Approved** | Keyword used throughout the tool (auto-set for priority-pipeline keywords) |
| **Rejected** | Keyword excluded from use |

### AI Optimization: Questions
| Aspect | Details |
|--------|---------|
| **Trigger** | Select keyword(s) → Click "AI Optimization: Questions" button |
| **Action** | Researches frequently asked questions related to selected keywords |
| **Output** | Results appear in "AI Optimization Questions" menu page |
| **Purpose** | Find questions users ask AI search tools (ChatGPT, etc.) |
| **Value** | Generate answers for website publication to capture AI-driven search traffic |

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
| **AI Priority Scoring** | Automatic relevance ranking with reasoning for each keyword |
| **Auto-Approval Pipeline** | Priority-scored keywords are automatically approved for immediate use |
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
| `keyword_repository_main.png` | Main interface with keyword table showing Priority and Priority Score columns |

---

## Related Features

- [Knowledge Base](./knowledge_base.md) - Source of competitor data
- [AI Optimization Questions](./ai_optimization_questions.md) - Downstream question generation
- [Search Ranking](./search_ranking.md) - Track keyword performance

---

*Reassessed by: Cascade*  
*Date: March 1, 2026*  
*Version: 1.1*  
*Context: Iriscale → Iriscale GTM v0.3*

