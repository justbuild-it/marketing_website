# Knowledge Base

**Location:** Sidebar → INTELLIGENCE & RESEARCH → Knowledge Base  
**URL:** `/projects/{id}/manage`  
**Type:** Core foundation feature  
**Tags:** 
- [x] `TRAINING` - Essential first step for users
- [x] `VIDEO` - Great for onboarding demos
- [x] `MARKETING` - Shows AI-powered data extraction
- [x] `PROMO` - Differentiating feature

---

## Overview

The Knowledge Base is the foundational data layer for the entire Iriscale platform. It serves as the "source of truth" that powers all downstream AI-generated content including keywords, topics, articles, and social posts.

**Key Value Proposition:** Add your company website and materials once → AI extracts and structures company intelligence → All generated content stays on-brand and grounded in facts.

---

## Page Layout (3-Column)

```
┌─────────────────────────────────────────────────────────────────────────────┐
│ Knowledge Base                                    [Reset] [Publish] [Edit]  │
│ Manage sources and company research for                          2 sources  │
├──────────────────┬─────────────────────────────┬────────────────────────────┤
│ SOURCES &        │ Current Data                │ Task Monitor               │
│ COMPETITORS      │ (Source of Truth)           │ Company research tasks     │
│                  │                             │                            │
│ ▼ SOURCES (2)    │ Overview                    │ In progress: 0             │
│   + Add Source   │ [Company description...]    │ Completed: 8               │
│   • File.txt     │                             │ Failed: 0                  │
│   • Website URL  │ ▶ Industries (11)           │                            │
│                  │ ▶ Buyer Personas (12)       │ [Task list with            │
│ ▼ COMPETITORS(6) │ ▶ Products & Services (23)  │  timestamps]               │
│   + Add Comp.    │ ▶ Target Markets (6)        │                            │
│   • URL 1        │ ▶ Differentiators (11)      │                            │
│   • URL 2...     │ ▶ SEO Strategy              │                            │
└──────────────────┴─────────────────────────────┴────────────────────────────┘
```

---

## UI Components

### 1. Header Section

| Element | Description |
|---------|-------------|
| Title | "Knowledge Base" (H1) |
| Subtitle | "Manage sources and company research for" |
| Reset button | Revert changes |
| Publish State | Publish extracted data (disabled when no changes) |
| Edit Changes | Enter edit mode |
| Source count | "2 sources" badge |

### 2. Sources & Competitors Panel (Left)

#### Sources Section
- **Add Source** button (purple, primary action)
- List of existing sources with:
  - Icon (file or link type)
  - Name/URL
  - Delete button (trash icon)

#### Competitors Section
- **Add Competitor** button
- List of competitor URLs with same pattern

### 3. Add Source Modal

**Input Options:**
| Method | Description |
|--------|-------------|
| **File Upload** | Drag & drop or choose file (.txt, Markdown, PDF) |
| **Copied Text** | Paste text directly |
| **Website** | Enter URL for AI to crawl |
| **YouTube** | Enter YouTube URL for transcript extraction |

**Website Input Flow:**
```
┌─────────────────────────────────────┐
│ Add Website Link                    │
│ ┌─────────────────────────────────┐ │
│ │ https://example.com             │ │
│ └─────────────────────────────────┘ │
│ Enter a complete website URL        │
│                    [Cancel] [Add]   │
└─────────────────────────────────────┘
```

### 4. Current Data Panel (Center)

**Header:**
- Title: "Current Data (Source of Truth)"
- Expand/Collapse all buttons
- Item count: "157 total items"

**Overview Section:**
- Company description paragraph (always visible)
- AI-generated summary of the business

**Expandable Data Sections:**

| Section | Example Content |
|---------|-----------------|
| **Industries** | NAICS codes, PropTech, SaaS classifications |
| **Buyer Personas** | ICP profiles, roles, pain points |
| **Products & Services** | Feature list, capabilities |
| **Target Markets** | Geographic and demographic segments |
| **Differentiators** | Unique value propositions |
| **SEO Strategy** | Keyword themes, content approach |

Each section shows:
- Overview paragraph
- Items list with structured data

### 5. Source Data Panel (Side-by-side view)

When clicking a source, shows extracted data from that specific source:
- Same structure as Current Data
- Allows comparison between source and merged data
- Scroll sync toggle for easy comparison

### 6. Task Monitor Panel (Right)

| Section | Purpose |
|---------|---------|
| **In Progress** | Active research/extraction tasks |
| **Completed** | Finished tasks with timestamps |
| **Failed** | Error tasks for retry |
| **Agent Activity** | Live steps from AI agents |

---

## Data Flow

```
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│  Add Source  │ ──► │  AI Extracts │ ──► │ Source of    │
│  (URL/File)  │     │  & Structures│     │ Truth Data   │
└──────────────┘     └──────────────┘     └──────────────┘
                                                │
                     ┌──────────────────────────┼──────────────────────────┐
                     ▼                          ▼                          ▼
              ┌──────────────┐          ┌──────────────┐          ┌──────────────┐
              │  Keywords    │          │   Topics     │          │  Articles    │
              └──────────────┘          └──────────────┘          └──────────────┘
```

---

## Example Data (Shuk Rentals)

**Sources:**
1. `Shuk_Source_of_Truth.txt` - Manual document upload
2. `https://shuk-rentals.webflow.io/` - Company website

**Competitors (6):**
- apartments.com/rental-manager
- avail.co
- rentredi.com
- appfolio.com
- turbotenant.com
- tenantcloud.com

**Extracted Data (157 items):**
- Industries: 11 items
- Buyer Personas: 12 items
- Products & Services: 23 items
- Target Markets: 6 items
- Differentiators: 11 items
- SEO Strategy: Overview

---

## Screenshots

| File | Description |
|------|-------------|
| `knowledge_base_main.png` | Full page layout |
| `knowledge_base_add_source_modal.png` | Add source modal with options |
| `knowledge_base_add_website.png` | Website URL input |
| `knowledge_base_industries_expanded.png` | Expanded data section |
| `knowledge_base_source_detail.png` | Side-by-side source comparison |

---

## Key Capabilities

1. **Multi-source aggregation** - Combine website, documents, and text
2. **AI extraction** - Automatic structuring of company data
3. **Competitor research** - AI researches competitor sites
4. **Data comparison** - Side-by-side source vs. merged view
5. **Task monitoring** - Track research progress in real-time
6. **Edit workflow** - Review and modify extracted data

---

## User Workflow

1. **Initial Setup**
   - Add company website URL
   - Upload pitch deck, one-pagers, positioning docs
   - AI extracts and structures data

2. **Competitive Research**
   - Add competitor URLs
   - AI researches each competitor
   - Data populates for comparison

3. **Review & Refine**
   - Click "Edit Changes" to modify
   - Adjust extracted data as needed
   - "Publish State" to save

4. **Ongoing Maintenance**
   - Add new sources when positioning changes
   - Re-run research tasks
   - Keep data current

---

## Value Propositions

| For User | Benefit |
|----------|---------|
| **Time savings** | No manual data entry - AI extracts everything |
| **Consistency** | Single source of truth for all content |
| **Intelligence** | Structured competitive insights |
| **Quality** | All generated content grounded in real data |

---

## Feature Details (Confirmed)

### Source Processing
| Question | Answer |
|----------|--------|
| Website crawl scope | Many pages, most relevant - not entire site |
| Crawl depth | 1-2 levels deep |

### YouTube Integration
| Question | Answer |
|----------|--------|
| What's extracted | Transcripts only |
| Length limits | None (transcript-based) |

### Competitor Research
| Question | Answer |
|----------|--------|
| Extraction method | Same as company sources |
| Gap analysis | Separate feature: "Competitor Analysis" in menu |

### Edit Changes Flow
| Question | Answer |
|----------|--------|
| Manual editing | Yes - delete, add, and edit individual items |
| Publish trigger | Enabled when there are items to review; click to save recommended changes |

### Data Refresh
| Question | Answer |
|----------|--------|
| Refresh frequency | Future: weekly auto-refresh + manual option |
| Current state | Manual refresh available |

### Downstream Impact
| Question | Answer |
|----------|--------|
| Auto-regeneration | No - existing content is not auto-regenerated |
| Manual regeneration | Yes - individual items can be regenerated on demand |

### Limitations
| Limit | Value |
|-------|-------|
| Max sources | No hard limit; 10-20 recommended |
| Max file size | ~10MB |
| Crawl rate limits | None user-facing; API-determined |

---

## Assessment Status

| Item | Complete |
|------|----------|
| Layout documented | ✅ |
| Components identified | ✅ |
| Add source flow captured | ✅ |
| Data structure documented | ✅ |
| Screenshots taken | ✅ |
| User workflow mapped | ✅ |

---

*Assessed by: Cascade*  
*Date: January 17, 2026*  
*Version: 1.0*  
*Context: Shuk Rentals → Shuk GTM v0.2*
