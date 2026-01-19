# Social Posts

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/projects/{id}/socials`

---

## Overview

Social Media Posts is an AI-powered social content generator that creates platform-optimized posts from articles, URLs, or custom content. The feature includes campaign management, strategy brief generation, audience targeting, and real-time mobile previews.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Social Media Posts                                        │
│             │ Generate AI-powered social media content for [Project]    │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌─────────────────┬─────────────────┬─────────────────┐   │
│             │ │ Content Input   │ Strategy Brief  │ Mobile Preview  │   │
│             │ ├─────────────────┼─────────────────┼─────────────────┤   │
│             │ │ Campaign Name   │ Audience/Voice  │ [Platform UI]   │   │
│             │ │ Sub campaign    │ - Buyer persona │                 │   │
│             │ │ Source URL      │ - Target market │ Your Company    │   │
│             │ │ Destination URL │ - Differentiator│ Company • 2h    │   │
│             │ │ Instructions    │ - Brand Voice   │                 │   │
│             │ │ Intent/KPI      │                 │ [Post content]  │   │
│             │ │ [Platforms]     │ [Generate       │                 │   │
│             │ │ [Generate]      │  Strategy]      │ Like Comment    │   │
│             │ └─────────────────┴─────────────────┴─────────────────┘   │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components

### Content Input Panel
| Field | Description |
|-------|-------------|
| **Campaign Name** | Group posts by campaign |
| **Sub campaign** | Campaign subdivision |
| **Source URL** | Article/content source |
| **Destination URL** | Landing page link |
| **Optional Instructions** | Custom AI guidance |
| **Intent** | Promote, Educate, Announce, Launch, Nurture, Engage |
| **KPI** | CTR, Engagement, Reach, Impressions, Conversions, etc. |
| **Allow emojis** | Toggle emoji inclusion |
| **Target Platform** | Facebook, Instagram, X, LinkedIn, TikTok, YouTube, Reddit |

### Strategy Brief Panel
| Section | Description |
|---------|-------------|
| **Promote/CTR Tags** | Intent and KPI indicators |
| **Buyer Persona** | Auto-populated from Knowledge Base |
| **Target Market** | Auto-populated audience data |
| **Differentiators** | Auto-populated unique value props |
| **Brand Voice** | Auto-populated tone guidelines |

### Mobile Preview Panel
| Element | Description |
|---------|-------------|
| **Dark Mode Toggle** | Preview appearance |
| **Platform Preview** | Realistic post mockup |
| **Show Visual Asset** | Toggle image display |
| **Post Counter** | Selected post / Total posts / Images |

---

## Supported Platforms

| Platform | Content Types |
|----------|---------------|
| **Facebook** | Pages, Groups, Ads Manager |
| **Instagram** | Posts, Stories, Reels |
| **X (Twitter)** | Tweets, Threads, Spaces |
| **LinkedIn** | Posts, Articles, Company Updates |
| **TikTok** | Videos, Live, Ads |
| **YouTube** | Videos, Shorts, Live Streaming |
| **Reddit** | Posts, Comments, Communities |

---

## Intent Options

| Intent | Use Case |
|--------|----------|
| **Promote** | Drive traffic/sales |
| **Educate** | Share knowledge |
| **Announce** | News/updates |
| **Launch** | New product/feature |
| **Nurture** | Build relationships |
| **Engage** | Community interaction |

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **AI Content Generation** | Platform-optimized posts |
| **Campaign Management** | Organize by campaign/sub-campaign |
| **Strategy Auto-Population** | Pull from Knowledge Base |
| **Multi-Platform** | 7 social platforms supported |
| **Real-Time Preview** | Mobile mockup preview |
| **KPI Targeting** | Optimize for specific metrics |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `social_posts_main.png` | Main post generation interface |

---

## Related Features

- [Social Scheduler](./social_scheduler.md) - Schedule generated posts
- [Connections](./connections.md) - Platform connections
- [Content Architecture](./content_architecture.md) - Content source

