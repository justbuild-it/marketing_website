# Content Architecture

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/content-architecture`

---

## Overview

Content Architecture is a sophisticated AI-powered website content planning tool that generates a complete hierarchical structure of pages for a company's website. A specialized AI agent creates the architecture using all available company information, knowledge base data, keywords, and content strategy best practices. Users can manually edit, add, remove, and reorder pages, with each page having SEO settings, link management, content generation, social promotion, and analytics capabilities.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                   [Delete] │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Content Architecture                                      │
│             │ ★ Shuk Rentals - Content Architecture                    │
│   Sidebar   ├─────────────────────┬─────────────────────────────────────┤
│             │ ★ PAGES             │ Page Title: Learn                   │
│             │ Expand | Collapse   │ Node ID: 01KE5VW9T7TFG3...          │
│             │ FILTERS             ├─────────────────────────────────────┤
│             │ [Manual][AI Answer] │ Overview|SEO|Links|Content|Promote  │
│             │ [AI Article]        │                         |Analytics  │
│             ├─────────────────────┼─────────────────────────────────────┤
│             │ Tree View:          │ [Tab Content Area]                  │
│             │ ▼ Shuk Website      │                                     │
│             │   ▼ Top Navigation  │ Page properties, SEO settings,     │
│             │     ▼ LEARN         │ links, content, promotion options,  │
│             │       ▼ Landlord... │ or analytics data                   │
│             │         ▸ Page 1    │                                     │
│             │         ▸ Page 2    │                                     │
│             ├─────────────────────┤                                     │
│             │ ★ PAGE TEMPLATES    │                                     │
└─────────────┴─────────────────────┴─────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "Content Architecture" |
| **Breadcrumb** | "Shuk Rentals - Content Architecture" |
| **Delete Button** | Red delete button to remove architecture |

### Left Panel - Page Tree
| Element | Description |
|---------|-------------|
| **PAGES Label** | Section header with star icon |
| **Expand/Collapse All** | Toggle all tree nodes |
| **Filters** | Manual Page, AI Answer, AI Article toggles |
| **Search** | Filter pages by name |
| **Tree View** | Hierarchical website structure |
| **Add Child Page** | Button on each node to add child |
| **PAGE TEMPLATES** | Collapsible section with template options |

### Right Panel - Page Detail Tabs

#### Overview Tab
| Field | Description |
|-------|-------------|
| **Page Title** | Editable title field |
| **Page URL** | Root URL (disabled) |
| **Child URL** | Page-specific URL path |
| **Content Brief** | Description of content purpose and key messages |
| **Page Template** | Dropdown with SEO-optimized templates |
| **Word Count** | Target word count for article |
| **Edit Page** | Button to modify page settings |
| **Delete Page** | Button to remove page |
| **Generate Article** | Trigger article generation |

#### Audience & Voice Section (Overview Tab)
| Field | Status | Description |
|-------|--------|-------------|
| **Buyer Persona** | 📊 Loaded | Target decision makers |
| **Target Market** | 📊 Loaded | Audience description |
| **Differentiators** | 📊 Loaded | Unique value propositions |
| **Brand Voice** | 📊 Loaded | Company tone and messaging |

---

## Page Template Options

| Template | Use Case |
|----------|----------|
| **Pillar Hub Page** | Top-level content hubs |
| **Clustered Hub (Sub-Hub)** | Secondary topic clusters |
| **Guide (Discover/Succeed Spoke)** | Educational how-to content |
| **Comparison Page (Evaluate)** | Product/service comparisons |
| **Pricing / Offer Page (Decide)** | Conversion-focused pages |
| **Onboarding Pathway Step (Succeed)** | User onboarding content |
| **Case Study (Evidence)** | Customer success stories |

---

## Tab Functionality

### Overview Tab
- Page metadata (title, URLs, brief)
- Template selection
- Word count target
- Audience & voice context
- Action buttons (Edit, Delete, Generate Article)

### SEO Tab
| Section | Description |
|---------|-------------|
| **Primary Keywords** | Add/remove primary target keywords |
| **Secondary Keywords** | Manage supporting keywords (with tags) |
| **Meta Title & Description** | Auto-generated or manually editable |

### Links Tab
| Section | Description |
|---------|-------------|
| **Internal Text Links** | Table of link text + URL mappings |
| **Internal Content Links** | Prerequisite and supporting content links |
| **External Resources** | Citation and source links |
| **Link Strategy Tips** | Best practices guidance |

### Content Tab
| State | Description |
|-------|-------------|
| **No Article** | Shows "No article generated yet" with Generate button |
| **With Article** | Displays article content with Copy Markdown button |

### Promote Tab
| Element | Description |
|---------|-------------|
| **Supported Platforms** | X, LinkedIn, Reddit, Facebook, TikTok, Instagram, YouTube |
| **What Agent Creates** | Brand-aligned content, platform-optimized copy, engaging visuals, CTAs |
| **Send to Post Agent** | Trigger social post generation |
| **Example Preview** | Sample LinkedIn post format |

### Analytics Tab
| Section | Description |
|---------|-------------|
| **Time Range** | Last 7/30/90 Days, Last Year |
| **Key Metrics** | Page Views, Conversion Rate, Avg Time, Keyword Ranking |
| **SEO Performance** | Keyword positions with trends |
| **Optimization Recommendations** | AI-generated improvement suggestions |
| **Traffic Trend** | Chart visualization |
| **Actions** | Export Report, Set Alerts |

---

## Example Data (Shuk Rentals)

### Tree Structure
```
Shuk Website
└── Top Navigation
    ├── LEARN (12 children)
    │   ├── Landlord Challenges
    │   │   ├── Reducing Vacancy Stress
    │   │   ├── Late Rent & Collections
    │   │   ├── Common Screening Mistakes
    │   │   ├── Early Renewal Strategies
    │   │   ├── Managing Delinquent Tenants
    │   │   └── Standing Out as a Quality Landlord
    │   ├── Compliance & Legal
    │   │   ├── Fair Housing Overview
    │   │   ├── Security Deposit Laws by State
    │   │   ├── Eviction Process Basics
    │   │   └── ...more
    │   └── Market Insights
    │       └── ...
    ├── PRODUCTS
    ├── RESOURCES
    ├── CUSTOMERS
    ├── COMPANY
    └── Tenant Screening 101
```

### Sample Secondary Keywords (Learn Page)
- tenant maintenance portal
- rental messaging platform
- get covered integration
- online rent payment platform
- rental property listing platform
- landlord tenant review platform
- renewal tracking tool
- tenant pipeline software
- property management communication tool
- early lease renewal insights

---

## Feature Details (Confirmed)

### Generation
| Aspect | Details |
|--------|---------|
| **AI Agent** | Sophisticated content strategist AI |
| **Data Sources** | Knowledge Base, keywords, company info |
| **Understanding** | Deep content strategy knowledge |
| **Output** | Complete hierarchical website structure |

### Manual Editing
| Action | Supported |
|--------|-----------|
| **Add Pages** | ✅ Yes |
| **Remove Pages** | ✅ Yes |
| **Reorder Pages** | ✅ Yes |
| **Edit Properties** | ✅ Yes |

### Page Templates
| Aspect | Details |
|--------|---------|
| **Selection** | Content Architect determines optimal template |
| **Impact** | Template determines article structure and information type |

### Generate Article
| Aspect | Details |
|--------|---------|
| **Trigger** | User clicks "Generate Article" button |
| **Human-in-Loop** | Ensures only strategic content is generated |
| **Output** | Full article based on page template |

### Integration
| Feature | Connection |
|---------|------------|
| **Topics** | Articles from Topics auto-placed in architecture |
| **AI Answers** | AI-generated answers placed in architecture |
| **Assessment** | All content assessed for best location |

---

## Data Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│              Knowledge Base + Keywords + Company Info               │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│              Content Architect AI Agent                              │
│              - Analyzes company data                                 │
│              - Applies content strategy                              │
│              - Determines page hierarchy                             │
│              - Selects optimal templates                             │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                  Content Architecture                                │
│              - Hierarchical page tree                                │
│              - Page metadata & templates                             │
│              - SEO settings per page                                 │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
    ┌─────────────┬───────────────┼───────────────┬─────────────┐
    │             │               │               │             │
    ▼             ▼               ▼               ▼             ▼
┌────────┐  ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐
│ Article│  │   SEO    │   │  Links   │   │  Social  │   │Analytics │
│ Gen    │  │ Optimize │   │ Strategy │   │ Promote  │   │ Tracking │
└────────┘  └──────────┘   └──────────┘   └──────────┘   └──────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **AI-Powered Architecture** | Sophisticated agent creates complete site structure |
| **Template-Based Generation** | Each page type uses optimized article templates |
| **SEO Optimization** | Built-in keyword management and meta tags |
| **Link Strategy** | Internal and external link management |
| **Social Promotion** | One-click send to social post agent |
| **Performance Analytics** | Track page performance and get recommendations |
| **Human-in-Loop** | User controls which content gets generated |

---

## User Workflow

### 1. Review Architecture
```
Navigate to Content Architecture → Explore tree structure → Select pages
```

### 2. Configure Page
```
Select page → Review Overview → Set template → Add keywords (SEO tab)
```

### 3. Generate Article
```
Click "Generate Article" → AI creates content → Review in Content tab
```

### 4. Promote Content
```
Go to Promote tab → Click "Send to Post Agent" → Review drafts
```

### 5. Monitor Performance
```
Check Analytics tab → Review metrics → Follow recommendations
```

---

## Value Propositions

| For Role | Value |
|----------|-------|
| **Content Teams** | Complete content strategy in one view |
| **SEO Managers** | Keyword optimization built into structure |
| **Marketing Teams** | Integrated social promotion workflow |
| **Executives** | Clear content coverage visualization |
| **Product Teams** | Structured product content pages |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `content_architecture_main.png` | Main view with tree and Overview tab |
| `content_architecture_seo_tab.png` | SEO tab with keyword management |

---

## UI Improvement Opportunities

### High Priority
1. **Drag-Drop Reorder** - Visual reordering of tree nodes
2. **Bulk Actions** - Select multiple pages for actions
3. **Search Within Tree** - Highlight matching nodes

### Medium Priority
4. **Page Status Indicators** - Show article/draft/published status
5. **Template Preview** - Preview article structure before generation
6. **Progress Tracking** - Show % of architecture with content

### Low Priority
7. **Version History** - Track architecture changes
8. **Team Collaboration** - Assign pages to team members
9. **Content Calendar** - Integrate with publishing schedule

---

## Related Features

- [Knowledge Base](./knowledge_base.md) - Source of company data
- [Keyword Repository](./keyword_repository.md) - Keyword source
- [Topics](./topics.md) - Topic-based content
- [Articles](./articles.md) - Generated articles
- [Social Posts](./social_posts.md) - Social promotion

