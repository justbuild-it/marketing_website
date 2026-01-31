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

---

## Internal Section (NEW - January 2026)

The **Internal** section is a newly added area within the Knowledge Base left panel, located below the Competitors section. Its purpose is to store company documents and collateral that AI agents on the platform will use to create on-brand content.

### Location in UI

```
Company & Competitors Information (Left Panel)
├── Company Overview (3 sources)
├── Competitors (6 items)
└── Internal (2 items) ← NEW SECTION
    ├── Brand Voice & Writing Guidelines
    └── Branding Guidelines
```

### Purpose

The Internal section allows users to:
- Store documents and collateral for future campaign planning
- Maintain brand consistency across all AI-generated content
- Edit and update guidelines as the company evolves

### Add Internal Source

| Element | Description |
|---------|-------------|
| Button | "Add Internal Source" (purple, primary action) |
| Function | Allows users to add additional internal documents |

---

### Internal Document: Branding Guidelines

**Auto-generated** from the company's website and other assets.

| Attribute | Details |
|-----------|---------|
| Title | Branding Guidelines |
| Tags | Branding, Brand Identity, Visual Assets |
| Editable | ✅ Yes - via Edit button |
| Preview Mode | Default view shows formatted content |

#### Content Sections

| Section | Description |
|---------|-------------|
| **Brand Overview** | Company name, description, overall brand identity |
| **Color Palette** | Primary, accent, background, text, and link colors with hex codes |
| **Typography** | Font families (primary, heading), font stacks, font sizes (H1, H2, Body) |
| **Visual Assets** | Logo, Favicon, Open Graph Image (with actual images displayed) |
| **Design System** | Base spacing unit, border radius, component styling (inputs) |
| **Technical Details** | Frameworks, metadata (Twitter Card, viewport, OG tags, etc.) |

#### Example Data (Shuk Rentals)

| Element | Value |
|---------|-------|
| Primary Color | `#15B8A6` |
| Accent Color | `#0000EE` |
| Primary Font | Athletics |
| H1 Size | 64px |
| Border Radius | 16px |

#### Usage by Platform

- Used by **AI agents** to ensure all generated content and collateral assets match the company's brand
- Informs visual styling for any AI-created materials

---

### Internal Document: Brand Voice & Writing Guidelines

**Auto-generated** to provide writing guidance for on-brand content creation.

| Attribute | Details |
|-----------|---------|
| Title | Writer's Quick Reference Guide |
| Tags | Brand Voice, Writing Guidelines, Style Guide, Content Strategy |
| Editable | ✅ Yes - via Edit button |
| Preview Mode | Default view shows formatted content |

#### Content Sections

| Section | Description |
|---------|-------------|
| **Core Voice Pillars** | Table with pillars, meanings, and example phrases |
| **Voice Personality** | "Sounds like" vs "Does NOT sound like" examples |
| **Tone by Context** | Content type, tone, formality level, and notes |
| **Format Specs** | Word counts, emoji usage, and guidelines per content type |
| **Before/After Examples** | Transformation examples showing voice application |
| **Common Mistakes to Avoid** | List of writing pitfalls |
| **Pre-Publish Checklist** | 10-point quality checklist |

#### Core Voice Pillars (Shuk Example)

| Pillar | What it means |
|--------|---------------|
| Practical playbooks | Steps, checklists, clear definitions |
| Predictability-first | Reduce uncertainty, set expectations early |
| Transparent and proof-backed | Clear about fees/limits, support claims with proof |
| Calmly confident | Measured certainty, no hype or panic |
| Fair-minded | Avoid stereotypes, keep disputes neutral |

#### Tone by Context Table

| Content Type | Tone | Formality |
|--------------|------|-----------|
| Website marketing | Confident, benefit-led | Medium |
| Blog/guides | Practical, instructional | Medium-High |
| Marketing email | Value-first | Medium |
| Support reply | Empathetic, action-led | Medium |
| Social | Educational, light humor OK | Low-Medium |

#### Format Specs by Content Type

| Format | Length | Emoji | Notes |
|--------|--------|-------|-------|
| Long blog | 1,200–2,500 words | 0 | One CTA; transparent tradeoffs |
| Marketing email | 100–200 words | 0 | Value-first subject line |
| Transactional email | 40–120 words | 0 | Confirm action + next step |
| Product UI | As short as possible | 0 | Verb + object buttons |
| Social | 20–80 words | 2–4 | Educational + proof |

#### Usage by Platform

- Used by **writing agents** to ensure all output meets customer requirements for style, voice, and tone
- Ensures consistency across articles, social posts, emails, and other written content

---

### Edit Workflow for Internal Documents

1. Click on document in Internal section list
2. Document opens in side panel with Preview/Edit toggle
3. Click **Edit** button to enter edit mode
4. Make changes directly in the editor
5. Changes are saved and used by AI agents going forward

### Value Propositions

| For User | Benefit |
|----------|---------|
| **Brand consistency** | All AI-generated content follows company guidelines |
| **Time savings** | Guidelines auto-generated from existing assets |
| **Flexibility** | Edit and update as brand evolves |
| **Quality control** | Writing agents follow defined voice and style |

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
| **Internal section documented** | ✅ |
| **Branding Guidelines documented** | ✅ |
| **Brand Voice Guidelines documented** | ✅ |

---

*Assessed by: Cascade*  
*Date: January 28, 2026*  
*Version: 1.1*  
*Context: Shuk Rentals → Shuk GTM v0.2*
