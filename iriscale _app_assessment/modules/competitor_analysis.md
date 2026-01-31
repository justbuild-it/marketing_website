# Competitor Analysis

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-28  
> **URL Pattern:** `/projects/{id}/competitor-analysis`

---

## Overview

Competitor Analysis provides deep, AI-generated competitive intelligence reports comparing your business against competitors. Analyses are triggered when competitors are added in the Knowledge Base and produce comprehensive, editable markdown documents with strategic insights, feature matrices, and positioning recommendations.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Competitor Analysis                                       │
│             │ Compare your business with competitors to identify...     │
│   Sidebar   ├─────────────────────┬─────────────────────────────────────┤
│             │ Search analyses...  │ [Your Co] vs [Competitor]           │
│             ├─────────────────────┤ [Preview] [Edit]    Auto-save [ON]  │
│             │ Analysis List       ├─────────────────────────────────────┤
│             │ • vs Competitor 1   │                                     │
│             │ • vs Competitor 2   │  📊 Competitive Analysis Document   │
│             │ • vs Competitor 3   │                                     │
│             │ • vs Competitor 4   │  - Overall Summary                  │
│             │ • vs Competitor 5   │  - Positioning Gap Analysis         │
│             │ • vs Competitor 6   │  - Feature Matrix                   │
│             │                     │  - ...more sections                 │
└─────────────┴─────────────────────┴─────────────────────────────────────┘
```

---

## UI Components

### Header Section
| Element | Description |
|---------|-------------|
| **Title** | "Competitor Analysis" |
| **Subtitle** | "Compare your business with competitors to identify strategic opportunities and market positioning" |
| **Icon** | Purple comparison icon |

### Left Panel - Analysis List
| Element | Description |
|---------|-------------|
| **Search** | Filter analyses by competitor name |
| **Analysis Cards** | Clickable cards showing "[Your Co] vs [Competitor]" |
| **Date** | When analysis was created/updated |
| **Delete Button** | Remove analysis (per card) |

### Right Panel - Analysis Detail
| Element | Description |
|---------|-------------|
| **Title Bar** | "[Your Co] vs [Competitor]" |
| **Preview Button** | Read-only view mode |
| **Edit Button** | Editable markdown mode |
| **Auto-save Toggle** | Enable/disable automatic saving |
| **Article Content** | Rich markdown document |

---

## Analysis Document Structure

### Metadata Header
| Field | Example |
|-------|---------|
| **Analysis Date** | December 7, 2025 |
| **Status** | Complete |
| **Confidence** | High |

### Document Sections

| Section | Icon | Description |
|---------|------|-------------|
| **1. Overall Summary** | 📊 | High-level strategic comparison |
| **2. Positioning Gap Analysis** | 🎯 | Market positioning differences |
| **3. Product & Services Feature Matrix** | 🛠️ | Detailed feature-by-feature comparison |
| **4. Target Audience Analysis** | 👥 | Audience comparison and opportunities |
| **5. Pricing & Business Model** | 💰 | Pricing strategy comparison |
| **6. Strengths & Weaknesses** | ⚖️ | SWOT-style analysis |
| **7. Strategic Opportunities** | 🚀 | Growth and differentiation opportunities |
| **8. Competitive Sales Battle Card** | 🥊 | Sales-focused competitive intelligence (NEW) |
| **9. Cooperation & Partnership Analysis** | 🤝 | Partnership feasibility and strategy (NEW) |
| **Key Takeaways** | 🎯 | Summary recommendations |

---

## Example Data (Shuk Rentals)

### Competitor Analyses Available
| Analysis | Competitor | Date |
|----------|------------|------|
| Shuk Rentals vs Apartments.com (Rental Manager) | Apartments.com | Jan 4 |
| Shuk Rentals vs AppFolio | AppFolio | Jan 4 |
| Shuk Rentals vs Avail | Avail | Jan 3 |
| Shuk Rentals vs TenantCloud | TenantCloud | Jan 3 |
| Shuk Rentals vs TurboTenant | TurboTenant | Jan 3 |
| Shuk Rentals vs RentRedi | RentRedi | Jan 3 |

### Sample Feature Matrix (Shuk vs Apartments.com)

#### Core Operations
| Feature | Shuk | Apartments.com |
|---------|------|----------------|
| Online Rent Collection | ✅ Yes | ✅ Yes |
| Tenant Screening | ✅ Yes | ✅ Yes |
| Lease Management | ✅ Yes | ✅ Yes |
| Maintenance Tracking | ✅ Yes | ✅ Yes |
| Expense Management | ✅ Yes | ✅ Yes |
| Financial Reporting | ✅ Yes | ⚠️ Partial |

#### Advanced Features
| Feature | Shuk | Apartments.com |
|---------|------|----------------|
| Lease Renewal Prediction | ✅ Yes | ❌ No |
| Two-Way Reviews | ✅ Yes | ❌ No |
| Year-Round Marketing | ✅ Yes | ❌ No |
| Service Provider Network | ✅ Yes | ❌ No |

#### Marketing & Listing
| Feature | Shuk | Apartments.com |
|---------|------|----------------|
| Property Listing | ⚠️ Partial | ✅ Yes |
| Multiple Marketplace Integration | ❌ No | ✅ Yes |
| 3D Tours | ❌ No | ✅ Yes |
| Rent Comp Reports | ❌ No | ✅ Yes |

### Positioning Comparison Table
| Attribute | Shuk | Apartments.com |
|-----------|------|----------------|
| Market Position | Premium Specialist | Free Comprehensive |
| Target Sophistication | Quality/Experienced | All Levels |
| Value Proposition | Predictive Insights | Complete Toolkit |
| Pricing Strategy | Paid Premium | Free Platform |
| Portfolio Focus | 1-100 Units | All Sizes |

---

## Feature Details (Confirmed)

### Generation Trigger
| Aspect | Details |
|--------|---------|
| **Trigger** | Competitor added in Knowledge Base |
| **Process** | AI automatically generates comprehensive analysis |
| **Source Data** | Knowledge Base competitor information |

### Refresh Frequency
| Current | Future |
|---------|--------|
| Manual refresh | Automated weekly updates |

### Edit Capabilities
| Aspect | Details |
|--------|---------|
| **Format** | Editable markdown with rich data |
| **Modes** | Preview (read-only) and Edit (markdown) |
| **Auto-save** | Toggle to automatically save changes |

### Export/Share
| Method | Details |
|--------|---------|
| **Current** | Copy screen |
| **Future** | TBD |

### Integration
| Feature | Connection |
|---------|------------|
| **AI Agents** | Used to create competitive campaigns |
| **Other Actions** | Provides competitor info for various workflows |

---

## Data Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                Knowledge Base: Add Competitor                        │
│                (Website URL + Company Info)                          │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│              AI Analysis Generation Triggered                        │
│              - Website crawl                                         │
│              - Feature extraction                                    │
│              - Positioning analysis                                  │
│              - Gap identification                                    │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
                                  ▼
┌─────────────────────────────────────────────────────────────────────┐
│                 Competitor Analysis Document                         │
│              - Overall Summary                                       │
│              - Positioning Gap Analysis                              │
│              - Feature Matrix                                        │
│              - Strategic Recommendations                             │
└─────────────────────────────────┬───────────────────────────────────┘
                                  │
         ┌────────────────────────┼────────────────────────┐
         │                        │                        │
         ▼                        ▼                        ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  User Review    │    │  AI Agents      │    │  Competitive    │
│  & Edit         │    │  (Campaigns)    │    │  Keywords       │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Automated Generation** | AI creates comprehensive analyses from competitor data |
| **Feature Matrices** | Detailed side-by-side feature comparisons |
| **Positioning Analysis** | Strategic market positioning insights |
| **Editable Content** | Full markdown editing with auto-save |
| **Multiple Competitors** | Manage analyses for all competitors |
| **AI Agent Integration** | Feeds competitive campaigns and workflows |
| **Sales Battle Cards** | Actionable competitive intelligence for sales teams (NEW) |
| **Partnership Analysis** | Strategic cooperation/partnership recommendations (NEW) |

---

## User Workflow

### 1. Add Competitor (Knowledge Base)
```
Navigate to Knowledge Base → Add competitor website → AI generates analysis
```

### 2. Review Analysis
```
Navigate to Competitor Analysis → Select competitor → Review document
```

### 3. Edit Analysis
```
Click "Edit" → Modify markdown content → Auto-save or manual save
```

### 4. Use in Campaigns
```
AI agents access competitor data → Create competitive campaigns
```

---

## Value Propositions

| For Role | Value |
|----------|-------|
| **Marketing Teams** | Competitive positioning and messaging guidance |
| **Product Teams** | Feature gap identification and prioritization |
| **Sales Teams** | Competitive battlecards and differentiation points |
| **Executives** | Strategic market landscape understanding |
| **Content Teams** | Competitive content angles and topics |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `competitor_analysis_main.png` | Main view with analysis list and document |
| `competitor_analysis_feature_matrix.png` | Feature comparison table |

---

## UI Improvement Opportunities

### High Priority
1. **Export Options** - PDF/Word export for battlecards
2. **Comparison View** - Side-by-side multiple competitors
3. **Change Tracking** - Show what's changed since last analysis

### Medium Priority
4. **Templates** - Different analysis templates for different needs
5. **Highlights** - Mark key differentiators and gaps
6. **Share Links** - Shareable links for team members

### Low Priority
7. **Version History** - Track document revisions
8. **Comments** - Add notes and annotations
9. **Custom Sections** - Add custom analysis sections

---

---

## New Sections (January 2026 Update)

### Section 8: 🥊 Competitive Sales Battle Card

A comprehensive sales enablement resource designed to help sales teams compete directly against specific competitors.

#### Purpose
Provides actionable competitive intelligence for sales conversations, objection handling, and deal positioning when directly competing for business.

#### Subsections

| Subsection | Description |
|------------|-------------|
| **8.1 One-Sentence Competitive Positioning** | Quick positioning statement for sales conversations |
| **8.2 Ideal & Poor Fit Signals** | Indicators of when prospect is good/bad fit vs competitor |
| **8.3 Top 3 Sales-Critical Differentiators** | Key differentiators to emphasize in sales |
| **8.4 Common Competitor Claims & Recommended Responses** | Objection handling guide with specific rebuttals |
| **8.5 Trap Questions for Sales Discovery** | Questions to uncover prospect pain points competitor can't solve |
| **8.6 Switching Narrative & Risk Reduction** | How to position switching and reduce perceived risk |
| **8.7 Proof to Use Against This Competitor** | Specific proof points, testimonials, and data |
| **8.8 Landmines to Avoid** | Topics/claims to avoid that favor competitor |
| **8.9 Recommended Close Paths** | Suggested closing strategies for competitive deals |
| **8.10 Internal Sales Intelligence** | Non-customer-facing competitive insights for sales team |

#### Value for Sales Teams

| Use Case | Benefit |
|----------|---------|
| **Discovery calls** | Trap questions reveal competitor weaknesses |
| **Objection handling** | Pre-built responses to common competitor claims |
| **Positioning** | Clear differentiation talking points |
| **Closing** | Recommended paths based on competitive dynamics |
| **Internal prep** | Intelligence not shared with prospects |

---

### Section 9: 🤝 Cooperation & Partnership Analysis

Strategic analysis of potential cooperation or partnership opportunities with the competitor.

#### Purpose
Evaluates whether formal or informal partnership with the competitor could benefit both parties, and recommends a strategic stance.

#### Subsections

| Subsection | Description |
|------------|-------------|
| **9.1 Cooperation Feasibility Assessment** | Analysis of whether partnership makes strategic sense |
| **9.2 Partnership Opportunity Zones** | Areas where cooperation could create mutual value |
| **9.3 Viable Partnership Models** | Specific partnership structures with feasibility ratings |
| **9.4 Strategic Upside vs Strategic Risk** | Benefits and risks of partnership |
| **9.5 Signals to Monitor Before Partnering** | Positive and negative indicators for partnership timing |
| **9.6 Recommended Strategic Stance & Next Steps** | Final recommendation and action items |

#### Partnership Models Evaluated

| Model | Description | Typical Feasibility |
|-------|-------------|---------------------|
| **Referral Partnership** | Mutual customer referrals | Medium |
| **API Integration** | Technical connection between platforms | Low-Medium |
| **Co-branded Education** | Joint webinars/content | Low |
| **White-label Features** | One powers features for the other | High complexity |

#### Strategic Outputs

- **Recommended Stance:** Clear recommendation (partner, avoid, monitor)
- **Rationale:** Strategic reasoning for the recommendation
- **Next Steps:** Specific actions to take
- **Tactical Approach:** How to position against/with competitor

---

## Related Features

- [Knowledge Base](./knowledge_base.md) - Source of competitor data
- [Keyword Repository](./keyword_repository.md) - Competitor keywords
- [Articles](./articles.md) - Competitive content creation
- [AI Agents](./opportunity_agent.md) - Competitive campaign automation

