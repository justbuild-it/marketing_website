# Iriscale Feature Inventory

> **Assessment Method:** Live app exploration via MCP Playwright  
> **Note:** All features documented from direct observation - no assumptions from outdated sources

---

## Discovered Screens & Features

### Account Section (User Menu)
| # | Screen/Feature | Location/Path | Documented | Screenshots | Training | Video | Marketing | Promo |
|---|----------------|---------------|------------|-------------|----------|-------|-----------|-------|
| 1 | Profile Settings | `/profile` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 2 | Company Management | `/companies` | ✅ | ✅ | ✅ | ⬜ | ✅ | ⬜ |
| 3 | People & Teams | `/people` | ✅ | ✅ | ✅ | ⬜ | ✅ | ⬜ |

### Header Navigation
| # | Screen/Feature | Location/Path | Documented | Screenshots | Training | Video | Marketing | Promo |
|---|----------------|---------------|------------|-------------|----------|-------|-----------|-------|
| 4 | Org/Project Selector | Header (top-left) | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |

### Main App Pages
| # | Screen/Feature | Location/Path | Documented | Screenshots | Training | Video | Marketing | Promo |
|---|----------------|---------------|------------|-------------|----------|-------|-----------|-------|
| 5 | Feature Exploration | `/` (root) | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 6 | Getting Started Flyout | Sidebar (bottom) | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |

### Sidebar Features (To Be Assessed)
| # | Screen/Feature | Location/Path | Documented | Screenshots | Training | Video | Marketing | Promo |
|---|----------------|---------------|------------|-------------|----------|-------|-----------|-------|
| 7 | Knowledge Base | `/projects/{id}/manage` | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| 7a | Knowledge Base - Internal Section | `/projects/{id}/manage` (left panel) | ✅ | ⬜ | ⬜ | ⬜ | ⬜ | ⬜ |
| 7b | Branding Guidelines | `/projects/{id}/manage` (Internal) | ✅ | ⬜ | ⬜ | ⬜ | ✅ | ⬜ |
| 7c | Brand Voice & Writing Guidelines | `/projects/{id}/manage` (Internal) | ✅ | ⬜ | ⬜ | ⬜ | ✅ | ⬜ |
| 8 | Keyword Repository | `/projects/{id}/keywords` | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 9 | Search Ranking | `/projects/{id}/search-ranking` | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 10 | Competitor Analysis | `/projects/{id}/competitor-analysis` | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 10a | Competitor Analysis - Battle Card (Section 8) | `/projects/{id}/competitor-analysis` | ✅ | ⬜ | ⬜ | ⬜ | ✅ | ⬜ |
| 10b | Competitor Analysis - Partnership (Section 9) | `/projects/{id}/competitor-analysis` | ✅ | ⬜ | ⬜ | ⬜ | ✅ | ⬜ |
| 11 | Content Architecture | `/projects/{id}/content-architecture` | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 12 | Topic Strategy (was Topics) | `/projects/{id}/topic` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 13 | AI Optimization Questions | `/projects/{id}/ai-optimizations` | ✅ | ✅ | ✅ | ✅ | ✅ | ⬜ |
| 14 | Articles | `/projects/{id}/articles` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 15 | AI Optimization Answers | `/projects/{id}/aio-answers` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 16 | Opportunity Agent | `/projects/{id}/opportunity-agent` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 16a | Blog Article Recommendations | `/projects/{id}/opportunities/{id}` | ✅ | ⬜ | ⬜ | ⬜ | ✅ | ⬜ |
| 17 | Social Posts | `/projects/{id}/socials` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 18 | Social Scheduler | `/social-scheduler` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |
| 19 | Connections | `/connections` | ✅ | ✅ | ✅ | ⬜ | ⬜ | ⬜ |

---

## Navigation Structure

```
[App Root] app.iriscale.com
├── Top Navigation
│   ├── Company Selector (dropdown)
│   ├── Project Selector (dropdown)
│   ├── AI Agent (button)
│   ├── Feedback (button)
│   ├── Beta badge
│   └── User Menu (Dean Gannon)
│       ├── Profile Settings → /profile
│       ├── Companies → /companies
│       ├── People → /people
│       └── Sign Out
│
├── Left Sidebar
│   ├── Feature Exploration (home)
│   ├── INTELLIGENCE & RESEARCH
│   │   ├── Knowledge Base
│   │   │   └── Company & Competitors Information (Left Panel)
│   │   │       ├── Company Overview (sources)
│   │   │       ├── Competitors (competitor URLs)
│   │   │       └── Internal (NEW - Jan 2026)
│   │   │           ├── Branding Guidelines
│   │   │           └── Brand Voice & Writing Guidelines
│   │   ├── Keyword Repository
│   │   ├── Search Ranking
│   │   └── Competitor Analysis
│   ├── STRATEGY & PLANNING
│   │   ├── Content Architecture
│   │   ├── Topics
│   │   └── AI Optimization Questions
│   ├── CONTENT CREATION
│   │   ├── Articles
│   │   └── AI Optimization Answers
│   ├── OPPORTUNITY & ENGAGEMENT
│   │   └── Opportunity Agent
│   ├── PROMOTE
│   │   ├── Social Posts
│   │   ├── Social Scheduler
│   │   └── Connections
│   └── Projects & Teams
│
└── Bottom Left
    └── Getting Started (progress indicator)
```

---

## Overall Progress

| Metric | Count | Total | % |
|--------|-------|-------|---|
| Screens Documented | 22 | ~22 | 100% |
| Screenshots Captured | 19 | ~22 | 86% |
| Training Content Ready | 19 | ~22 | 86% |
| Video Scripts Ready | 7 | ~22 | 32% |
| Marketing Copy Ready | 13 | ~22 | 59% |
| Promo Material Ready | 1 | ~22 | 5% |

---

## Priority Assessment

### High Priority (Core Features)
Modules most critical for initial documentation:
- [ ] 
- [ ] 
- [ ] 

### Medium Priority (Supporting Features)
Important but not launch-critical:
- [ ] 
- [ ] 
- [ ] 

### Lower Priority (Advanced Features)
Can be documented after initial release:
- [ ] 
- [ ] 
- [ ] 

---

## Notes

*Use this space to track decisions, questions, or blockers during assessment*

### Questions for Product Team
1. 
2. 
3. 

### Decisions Made
- Internal section added to Knowledge Base (Jan 2026)
- Branding Guidelines and Brand Voice Guidelines are auto-generated and editable

### Blockers
- 

### Recent Updates (January 28-29, 2026)
- Added Internal section documentation (3 new sub-features)
- Updated navigation structure to reflect Knowledge Base hierarchy
- Competitors section confirmed as existing feature (6 competitor URLs)
- **Competitor Analysis updated** with 2 new sections:
  - Section 8: Competitive Sales Battle Card (10 subsections)
  - Section 9: Cooperation & Partnership Analysis (6 subsections)
- **Topic Strategy UI overhaul** (January 29, 2026):
  - Feature renamed from "Topics" to "Topic Strategy"
  - New "Core Ideas" panel replaces "Sources" panel
  - New Core Idea input modal with full-funnel generation
  - Column names updated (Sub Topic → Article Topic, Main Topic → Cluster Topic, etc.)
- **Opportunity Agent - Blog Article Recommendations** (January 30, 2026):
  - New section in Opportunity Details page
  - AI-generates blog/article ideas from real-time social conversations
  - Includes: Topic, Target Audience, Primary Problem, Key Takeaways, Suggested Sections, Evidence, Company Expertise Angle

---

*Last Updated: January 30, 2026*
