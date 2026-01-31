# Opportunity Agent

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-30  
> **URL Pattern:** `/projects/{id}/opportunity-agent`
> **Opportunities URL:** `/projects/{id}/opportunities`
> **Opportunity Details URL:** `/projects/{id}/opportunities/{opportunity_id}`

---

## Overview

Opportunity Agent is an AI-powered monitoring system that scans social platforms (primarily Reddit) to discover business opportunities. Agents can be configured to search for specific keywords and topics, identifying posts where the company's products/services could provide value.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Opportunity Agents                                        │
│             │ Configure and manage opportunity monitoring agents        │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ [Expand All] | [Collapse All]  [Auto-refresh ▼] [Refresh] │
│             │ [Active Agents ▼]                        [+ New Agent]    │
│             │ ┌─────────────────────────────────────────────────────┐   │
│             │ │ Property Management Software trial agent            │   │
│             │ │ [Opportunities] [Edit] [...]                        │   │
│             │ │ ┌──────────┬──────────┬────────────┬──────────┐     │   │
│             │ │ │ 30       │ 8        │ 6m 36s     │ ✓ Done   │     │   │
│             │ │ │ Opps     │ Sources  │ Process    │ Status   │     │   │
│             │ │ │ from 543 │ subreddit│ 8 methods  │          │     │   │
│             │ │ └──────────┴──────────┴────────────┴──────────┘     │   │
│             │ │ Created: Jan 8, 2026    Updated: Jan 17, 2026       │   │
│             │ └─────────────────────────────────────────────────────┘   │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Header Controls
| Element | Description |
|---------|-------------|
| **Expand/Collapse All** | Toggle all agent cards |
| **Auto-refresh** | 10s, 30s, 1m, 5m intervals |
| **Refresh** | Manual refresh |
| **Filter** | Active/All/Completed/Processing/Failed |
| **New Agent** | Create new monitoring agent |

### Agent Card
| Element | Description |
|---------|-------------|
| **Agent Name** | Descriptive title |
| **Opportunities Button** | View discovered opportunities |
| **Edit Button** | Modify agent configuration |
| **More Menu** | Additional actions |

### Agent Metrics
| Metric | Description |
|--------|-------------|
| **Opportunities** | Number found / total posts scanned |
| **Sources** | Number of subreddits monitored |
| **Process Time** | Execution duration and methods |
| **Status** | Completed / Processing / Failed |

---

## Example Data (Shuk Rentals)

### Agent: Property Management Software trial agent
| Metric | Value |
|--------|-------|
| **Opportunities** | 30 from 543 posts |
| **Sources** | 8 subreddits |
| **Process Time** | 6m 36s (8 methods) |
| **Status** | Completed |
| **Created** | Jan 8, 2026 |
| **Updated** | Jan 17, 2026 |

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **Multi-Platform Scanning** | Reddit (primary), expandable |
| **Keyword Monitoring** | Track specific terms |
| **Opportunity Scoring** | AI identifies relevant posts |
| **Auto-Refresh** | Continuous monitoring |
| **Multiple Agents** | Different keyword sets |
| **Blog Article Recommendations** | AI-generated content ideas from opportunities (NEW) |

---

## Opportunity Details Page (January 2026 Update)

When viewing individual opportunity details, the page now includes comprehensive AI analysis sections:

### Page Sections

| Section | Description |
|---------|-------------|
| **Author Profile** | Reddit user info (karma, account age, verification) |
| **Subreddit Profile** | Community info (members, description, guidelines) |
| **Opportunity Metrics** | Upvotes, comments, engagement score, upvote ratio |
| **Customer Journey** | Visual indicator: Awareness → Consideration → Decision |
| **Assessment Breakdown** | Expandable scoring across 8 dimensions |
| **Original Post Content** | Full post with View Original link |
| **AI Analysis & Insights** | Relevance assessment and strategic insights |
| **Blog Article Recommendation** | AI-generated article idea (NEW) |
| **AI-Generated Response** | Tailored outreach with Copy/Edit buttons |
| **Product & Service Recommendations** | Matched solutions with % match |
| **New Product Opportunities** | Market gap identification |
| **Jobs-to-be-Done Analysis** | 7-question JTBD framework |
| **Action Recommendations** | Strategic next steps |

### Assessment Breakdown Dimensions

| Dimension | Description |
|-----------|-------------|
| **Urgency** | How time-sensitive is the need |
| **Intent** | Purchase/action intent signals |
| **Influence** | Author's reach and credibility |
| **Fit** | How well opportunity matches offering |
| **Competition** | Competitive landscape |
| **Sentiment and Emotion** | Emotional state of the author |
| **Problem-Solution Gap** | Severity of unmet need |
| **JTBD Motivation** | Jobs-to-be-Done alignment |

---

## Blog Article Recommendation (NEW - January 2026)

A new AI-powered feature that generates timely blog and article ideas directly from discovered opportunities. This helps customers create content that addresses real-time discussions happening among their potential customers.

### Purpose

Customers can find timely ideas for blogs and articles that are being discussed in real-time by their potential customers on social platforms like Reddit.

### Blog Article Recommendation Structure

| Field | Description |
|-------|-------------|
| **Topic** | AI-generated article title/topic |
| **Target Audience** | Who the article should address |
| **Primary Problem** | The core issue the article should solve |
| **Key Takeaways** | Main points readers should learn |
| **Suggested Sections** | Recommended article structure/outline |
| **Evidence from Post** | Quote from the opportunity supporting the recommendation |
| **Company Expertise Angle** | How to position company expertise in the content |

### Example Blog Article Recommendation

**Topic:** "10 Proven Strategies to Avoid Email Spam Filters and Boost Deliverability"

| Field | Example Value |
|-------|---------------|
| **Target Audience** | Digital Marketing Managers and CMOs looking to enhance email marketing effectiveness |
| **Primary Problem** | Addressing the challenge of emails landing in spam and improving deliverability rates |
| **Key Takeaways** | Understanding sender reputation, best practices for email authentication, how to warm up a new domain |
| **Suggested Sections** | Introduction to Email Deliverability, Why Emails End Up in Spam, Key Strategies for Avoiding Spam Filters, The Role of Engagement in Deliverability, Tools and Resources, Conclusion |
| **Evidence from Post** | "The biggest lesson? There's no magic bullet. It's a combination of technical setup + list quality + actual good content people want to read." |
| **Company Expertise Angle** | The company's expertise in integrating SEO, content, and social data can guide marketers in understanding how these elements impact email marketing success |

### Customer Value

| Benefit | Description |
|---------|-------------|
| **Real-Time Relevance** | Content ideas based on actual conversations happening now |
| **Audience Alignment** | Topics proven to resonate with target audience |
| **SEO Opportunity** | Address questions people are actively asking |
| **Thought Leadership** | Position as expert on trending industry topics |
| **Content Calendar** | Source of timely content ideas |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `opportunity_agent_main.png` | Main agent overview |
| `opportunity_details.png` | Opportunity details with Blog Article Recommendation |

---

## Related Features

- [Social Posts](./social_posts.md) - Respond to opportunities
- [Keyword Repository](./keyword_repository.md) - Keyword source

