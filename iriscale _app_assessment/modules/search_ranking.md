# Search Ranking Intelligence

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/search-ranking`

---

## Overview

Search Ranking Intelligence is a powerful AI-powered discovery tool that monitors company visibility across major AI search providers. It serves multiple purposes: monitoring your company's AI search visibility, competitor tracking, and market research. Results guide strategic improvements to content and positioning.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Search Ranking Intelligence                               │
│             │ Run AI-powered discovery queries and explore ranking...   │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ [Search New Query] [Select Previous Query]                │
│             ├───────────────────────────────────────────────────────────┤
│             │ Selected Query: [query text]          Version: [date]     │
│             │ [X versions]              [Browse History] [Regenerate]   │
│             ├───────────────────────────────────────────────────────────┤
│             │ Top Ranking Companies                    [Table] [Chart]  │
│             │ Review company signals from multiple AI providers         │
│             ├───────────────────────────────────────────────────────────┤
│             │ Tabs: Provider Rankings | Provider Insights | ...         │
│             │ [Providers dropdown]                                      │
│             ├───────────────────────────────────────────────────────────┤
│             │ Data Visualization (Chart or Table)                       │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "Search Ranking Intelligence" |
| **Subtitle** | "Run AI-powered discovery queries and explore ranking trends for key companies" |

### Query Controls
| Element | Description |
|---------|-------------|
| **Search New Query** | Button to create a new discovery query |
| **Select Previous Query** | Button to load saved queries |
| **New Discovery Query** | Text input for entering queries |
| **Run Search** | Execute button (disabled until query entered) |
| **Placeholder** | "e.g., Top dehydrated onion suppliers in India" |

### Query Display (When Data Exists)
| Element | Description |
|---------|-------------|
| **Selected Query** | Shows current query text |
| **Version Date** | Timestamp of current version |
| **X versions** | Count of available versions |
| **Browse History** | View previous versions |
| **Regenerate** | Re-run query for fresh results |

### View Controls
| Element | Description |
|---------|-------------|
| **Table** | Tabular data view |
| **Chart** | Visual chart view with bar graphs |

### Analysis Tabs
| Tab | Description |
|-----|-------------|
| **Provider Rankings** | Compare rankings across AI providers |
| **Provider Insights** | Detailed insights per provider |
| **Company Comparison** | Compare companies head-to-head |
| **Provider Coverage** | See which providers mention which companies |
| **Top Companies** | View highest-ranked companies |
| **Ranking Distribution** | Distribution visualization |

### Filters
| Element | Description |
|---------|-------------|
| **Providers** | Dropdown to filter by AI provider |
| **Show** | Top 10/15/20/30 companies selector |
| **Search** | Filter by company or website |
| **Columns** | Toggle visible columns |

---

## AI Providers

All major AI search providers are queried automatically:

| Provider | Logo | Description |
|----------|------|-------------|
| **Claude** | ✓ | Anthropic's AI assistant |
| **OpenAI** | ✓ | ChatGPT/GPT-4 |
| **Gemini** | ✓ | Google's AI |
| **Perplexity** | ✓ | AI search engine |
| **Grok** | ✓ | xAI's assistant |

*Users cannot select providers - all major providers are queried automatically.*

---

## Table View Columns

| Column | Description |
|--------|-------------|
| **Company** | Company name |
| **Website** | Direct link to company site |
| **Source** | Where company was found (forbes.com, clutch.co, etc.) |
| **Found By** | Which AI providers mentioned it |
| **Best Rank** | Best ranking across all providers |
| **Claude Rank** | Ranking from Claude |
| **OpenAI Rank** | Ranking from ChatGPT |
| **Gemini Rank** | Ranking from Google Gemini |
| **Perplexity Rank** | Ranking from Perplexity |
| **Grok Rank** | Ranking from Grok |

---

## Example Data (Lunour - Brand Agencies Query)

**Query:** "What brand agencies are recommended for my software startup?"

| Company | Website | Best Rank | Claude | OpenAI | Gemini | Perplexity | Grok |
|---------|---------|-----------|--------|--------|--------|------------|------|
| Pentagram | pentagram.com | 1 | 1 | 1 | 5 | 7 | 3 |
| Interbrand | interbrand.com | 1 | — | 3 | — | — | 1 |
| Mission Control | missioncontrol.studio | 1 | — | — | — | 1 | — |
| Red Antler | redantler.com | 1 | — | — | 1 | 5 | — |
| Clay | clay.global | 2 | 6 | — | 3 | 2 | 9 |
| Focus Lab | focuslab.agency | 2 | 8 | — | 2 | 4 | 7 |
| Collins | wearecollins.com | 2 | 2 | 2 | — | — | — |
| Landor & Fitch | landorandfitch.com | 3 | 3 | — | — | 3 | — |

**Total Results:** 39 companies across 5 AI providers

---

## Feature Details (Confirmed)

### Query Purpose
| Use Case | Description |
|----------|-------------|
| **Company Visibility** | Monitor how your company ranks in AI search results |
| **Competitor Tracking** | See where competitors appear in AI responses |
| **Market Research** | Discover top players in any industry/niche |
| **Strategic Guidance** | Results guide what to improve in content/positioning |

### Ranking Methodology
| Aspect | Details |
|--------|---------|
| **Best Rank** | Calculated from best position across all providers |
| **Individual Ranks** | Each provider's ranking displayed separately |
| **Dash (—)** | Indicates company not mentioned by that provider |

### Version History
| Trigger | Details |
|---------|---------|
| **Automatic** | Weekly refresh of queries |
| **Manual** | Click "Regenerate" for on-demand refresh |

### Integration
| Feature | Connection |
|---------|------------|
| **AI Questions** | Important discoveries push to AI question tracking tool |
| **Content Strategy** | Informs what content to create/improve |

### Provider Selection
| Aspect | Details |
|--------|---------|
| **Selection** | Not user-selectable |
| **Coverage** | All major AI providers queried automatically |

---

## Chart View

The Provider Rankings Comparison chart displays:
- **X-axis:** Companies (Top 10/15/20/30)
- **Y-axis:** Ranking Position (0-10, lower is better)
- **Bars:** Color-coded by AI provider
- **Legend:** Provider logos with names

---

## Data Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                    User Enters Discovery Query                       │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│              AI Queries Sent to All Major Providers                  │
│     Claude | OpenAI | Gemini | Perplexity | Grok                    │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                   Results Aggregated & Ranked                        │
│              - Company extraction                                    │
│              - Website identification                                │
│              - Source attribution                                    │
│              - Ranking calculation                                   │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
         ┌────────────────────────┼────────────────────────┐
         │                        │                        │
         ▼                        ▼                        ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  Table View     │    │  Chart View     │    │  Version        │
│  (Detailed)     │    │  (Visual)       │    │  History        │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                  │
                                  ▼
                    ┌─────────────────────────┐
                    │  Strategic Insights     │
                    │  → AI Questions         │
                    │  → Content Strategy     │
                    └─────────────────────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Multi-Provider Queries** | Query all major AI search providers simultaneously |
| **Company Discovery** | Identify top players in any market |
| **Ranking Analysis** | Compare rankings across providers |
| **Version History** | Track changes over time with weekly auto-refresh |
| **Visual Analytics** | Chart and table views for different insights |
| **Source Attribution** | See where AI providers find their information |

---

## User Workflow

### 1. Create New Query
```
Click "Search New Query" → Enter query → Click "Run Search"
```

### 2. Analyze Results
```
View Table for details → Switch to Chart for visuals → Filter by provider
```

### 3. Compare Providers
```
Use tabs: Provider Rankings → Provider Insights → Company Comparison
```

### 4. Track Changes
```
Browse History → Compare versions → Regenerate for fresh data
```

---

## Value Propositions

| For Role | Value |
|----------|-------|
| **Marketing Teams** | Understand competitive landscape in AI search |
| **SEO Managers** | Monitor company visibility across AI platforms |
| **Content Teams** | Identify content gaps and opportunities |
| **Executives** | Strategic insights on market positioning |
| **Sales Teams** | Know top competitors mentioned by AI |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `search_ranking_main.png` | Empty state (Shuk Rentals) |
| `search_ranking_lunour_clean.png` | Populated view with query |
| `search_ranking_lunour_chart.png` | Chart view with provider comparison |
| `search_ranking_lunour_table.png` | Table view with detailed rankings |

---

## UI Improvement Opportunities

### High Priority
1. **Highlight Own Company** - Visually distinguish when your company appears
2. **Export Data** - Allow CSV/PDF export of results
3. **Alert System** - Notify when rankings change significantly

### Medium Priority
4. **Query Templates** - Preset queries for common use cases
5. **Trend Visualization** - Show ranking changes over time
6. **Provider Comparison** - Side-by-side provider analysis

### Low Priority
7. **Custom Scoring** - Weight providers differently
8. **Saved Queries** - Quick access to frequently used queries
9. **Competitor Watchlist** - Track specific companies

---

## Related Features

- [Keyword Repository](./keyword_repository.md) - Keyword management
- [AI Optimization Questions](./ai_optimization_questions.md) - Question tracking
- [Competitor Analysis](./competitor_analysis.md) - Detailed competitor research

