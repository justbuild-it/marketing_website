# Social Posts

> **Status:** ✅ Documented  
> **Last Updated:** 2026-03-01  
> **URL Pattern:** `/projects/{id}/socials`

---

## Overview

Social Media Posts is an AI-powered social content generator that creates platform-optimized posts from articles, URLs, or custom content. The feature was **completely reworked** in February–March 2026 with a new post sets–based architecture that simplifies creation, editing, selection, and scheduling.

**March 2026 Update:** The UI was rebuilt from a single 3-panel creation page to a multi-page flow: **Post Sets list → Create wizard → Post Set detail/review**. Posts are now organized into "post sets" (groups of posts generated from a single source), with bulk actions for approval and scheduling.

---

## Page Layout – Post Sets List (Main Page)

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Social Media Posts              [+ Create New Post]        │
│             │ Create and manage social posts to promote your content    │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ [Filter by tags]          [Search post sets...]           │
│             ├───────────────────────────────────────────────────────────┤
│             │ ┌──────────────┐  ┌──────────────┐  ┌──────────────┐    │
│             │ │ Post Set 1   │  │ Post Set 2   │  │ Post Set 3   │    │
│             │ │ [in] 3 posts │  │ [in][X] 6p   │  │ [in] 21p     │    │
│             │ │ iriscale.com │  │ iriscale.com │  │ iriscale.com │    │
│             │ │ #tags        │  │ #ai #seo     │  │ #Analytics.. │    │
│             │ │ 2/27/2026    │  │ 2/23/2026    │  │ 2/20/2026    │    │
│             │ │      Open →  │  │      Open →  │  │      Open →  │    │
│             │ └──────────────┘  └──────────────┘  └──────────────┘    │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## UI Components – Post Sets List

### Header
| Element | Description |
|---------|-------------|
| **Title** | "Social Media Posts" |
| **Subtitle** | "Create and manage social posts to promote your content" |
| **Create New Post** | Purple button → navigates to Create wizard |

### Toolbar
| Element | Description |
|---------|-------------|
| **Filter by tags** | Text input with autocomplete for tag-based filtering |
| **Search post sets** | Text search across post set names |

### Post Set Cards
| Element | Description |
|---------|-------------|
| **Title** | Post set name (e.g., "Ai Impact Seo Strategies") |
| **Platform Icons** | LinkedIn, X, etc. – shows which platforms have posts |
| **Post Count** | "3 posts", "21 posts", etc. |
| **Source URL** | Link icon + domain (e.g., iriscale.com) |
| **Tags** | Hashtag pills (e.g., #AI, #SEO, #DigitalMarketing) with "+N" overflow |
| **Date** | Creation date |
| **Open →** | Link to post set detail page |
| **Delete** | Trash icon button per card |

---

## Page Layout – Create Social Posts (Wizard)

```
┌─────────────────────────────────────────────────────────────────────────┐
│ ← Back to Posts                                                         │
├─────────────────────────────────────────────────────────────────────────┤
│ Create Social Posts  [Beta]              No platform yet | Connected: X │
│ Stay on-brand and generate ready-to-review social drafts from any link │
├─────────────────────────────────────────────────────────────────────────┤
│ 1. Content                                              REQUIRED       │
│    Content URL *        Post set name *                                │
│ ────────────────────────────────────────────────────────────────────── │
│ 2. Platforms   ⓘ Choose one or more channels                          │
│    [LinkedIn] [X] [Facebook] [Instagram] [TikTok] [YouTube]           │
│    Connected: None                                                     │
│ ────────────────────────────────────────────────────────────────────── │
│ ▶ 3. Options                                                           │
│ ▶ Advanced (KPI, brand voice, emoji settings)                          │
│ ────────────────────────────────────────────────────────────────────── │
│ [Cancel]                     [🚀 Generate Posts]                       │
└─────────────────────────────────────────────────────────────────────────┘
```

### Step 1: Content (Required)
| Field | Description |
|-------|-------------|
| **Content URL** | Paste article, landing page, or resource URL; AI pulls page context |
| **Post set name** | Descriptive name; autocomplete to reuse earlier post sets |

### Step 2: Platforms
| Platform | Status |
|----------|--------|
| **LinkedIn** | Available (linked/not linked indicator) |
| **X** | Available |
| **Facebook** | Available |
| **Instagram** | Available |
| **TikTok** | Available |
| **YouTube** | Available |

### Step 3: Options (Expandable)
| Field | Description |
|-------|-------------|
| **Intent preset** | Dropdown: Promote, Educate, Announce, Launch, Nurture, Engage |
| **Additional instructions** | Free text for custom AI guidance |
| **Click-through URL** | Custom landing page (defaults to content URL) |
| **Tags** | Optional, max 8; autocomplete, auto-normalized to lowercase-with-hyphens |

### Advanced (Expandable)
| Field | Description |
|-------|-------------|
| **Target KPI** | None (Auto-select), CTR, Engagement Rate, Reach, Impressions, Conversions, Shares, Comments, Saves, Lead Generation |
| **Tone** | Adaptive (auto-detect), Professional, Casual, Enthusiastic, Educational, Conversational |
| **Emoji flair** | Toggle switch – "Let AI sprinkle light emojis when relevant" |
| **UTM Medium** | Auto-filled; adjustable (default: "social") |

---

## Page Layout – Post Set Detail/Review

```
┌─────────────────────────────────────────────────────────────────────────┐
│ ← Back to Posts                                                         │
├──────────────────────────────────────────┬──────────────────────────────┤
│ Post Set Title  [Completed]              │ [All platforms] [LinkedIn]   │
│ 🔗 Source  3 posts                       │                              │
│ CREATED: Feb 27  UPDATED: Feb 27         │                              │
│ ✏️ Edit tags                              │                              │
├──────────────────────────────────────────┤                              │
│ [☐ Select all]  3 visible  [Approve][Sch]│  ┌────────────────────────┐ │
├──────────────────────────────────────────┤  │   LinkedIn Preview     │ │
│ ☐ [in] LinkedIn  Draft                   │  │   Your Company         │ │
│ Created/Updated timestamps  Copy|Edit|Vie│  │   Promoted             │ │
│ ┌──────────────────────────────────────┐ │  │                        │ │
│ │ [Image] 🚀 Ready to transform...     │ │  │   [Post content...]    │ │
│ │ Pattern: AIDA                        │ │  │                        │ │
│ │ [Full post text with hashtags...]    │ │  │   [Image]              │ │
│ │ platform:linkedin    453/3000        │ │  │                        │ │
│ │ UTM URL: https://...  [Copy] [Edit]  │ │  │   Like Comment Share   │ │
│ └──────────────────────────────────────┘ │  └────────────────────────┘ │
│                                          │                              │
│ ☐ [in] LinkedIn  Draft                   │                              │
│ [Next post...]                           │                              │
└──────────────────────────────────────────┴──────────────────────────────┘
```

### Post Set Header
| Element | Description |
|---------|-------------|
| **Title** | Post set name with status badge (Completed / Draft) |
| **Platform Filter** | "All platforms" / individual platform buttons |
| **Source** | Link to original content URL |
| **Post Count** | Total posts in set |
| **Timestamps** | Created and Updated dates |
| **Edit Tags** | Button to modify post set tags |

### Bulk Actions Bar
| Element | Description |
|---------|-------------|
| **Select all** | Checkbox to select all visible posts |
| **Visible count** | "3 visible" indicator |
| **Approve** | Bulk approve selected posts (disabled until selection) |
| **Schedule** | Bulk schedule selected posts (disabled until selection) |

### Individual Post Cards
| Element | Description |
|---------|-------------|
| **Checkbox** | Selection for bulk actions |
| **Platform Badge** | LinkedIn, X, etc. |
| **Status** | "draft" badge |
| **Timestamps** | Created / Updated dates |
| **Copy** | Copy post content to clipboard |
| **Edit** | Open inline editor |
| **View** | Preview post |
| **Post Image** | AI-generated image thumbnail |
| **Headline** | Bold opening line of post |
| **Pattern** | Writing pattern used (e.g., "AIDA: Attention → Interest → Desire → Action") |
| **Full Text** | Complete post content with hashtags |
| **Platform Tag** | "platform:linkedin" indicator |
| **Character Count** | "453/3000" (used/max for platform) |
| **UTM URL** | Auto-generated tracking URL with Copy UTM and Edit UTM buttons |

### Preview Panel (Right Side)
| Element | Description |
|---------|-------------|
| **Platform Mockup** | Realistic LinkedIn/X/etc. post preview |
| **Company Info** | "Your Company" + "Promoted" label |
| **Post Content** | Full post text as it would appear |
| **Media** | Post image preview |
| **Engagement Buttons** | Like, Comment, Share, Send (non-functional mockup) |

---

## Supported Platforms

| Platform | Available |
|----------|-----------|
| **LinkedIn** | ✅ |
| **X (Twitter)** | ✅ |
| **Facebook** | ✅ |
| **Instagram** | ✅ |
| **TikTok** | ✅ |
| **YouTube** | ✅ |

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
| **AI Content Generation** | Platform-optimized posts with pattern indicators (AIDA, etc.) |
| **Post Sets** | Organize related posts into named, tagged, searchable sets |
| **Multi-Step Wizard** | Clean 3-step creation: Content → Platforms → Options/Advanced |
| **Bulk Actions** | Select all, approve, schedule multiple posts at once |
| **UTM Tracking** | Auto-generated UTM URLs per platform with edit capability |
| **Platform Preview** | Real-time LinkedIn/X mockup preview |
| **Tag Management** | Filter and search post sets by tags |
| **Multi-Platform** | 6 social platforms supported |
| **KPI Targeting** | Optimize for specific metrics (CTR, Engagement, Conversions, etc.) |
| **Tone Control** | Professional, Casual, Enthusiastic, Educational, Conversational |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `social_posts_main.png` | Post sets list view with cards |
| `social_posts_create.png` | Create wizard with Content, Platforms, Options steps |
| `social_posts_detail.png` | Post set detail/review with individual posts and LinkedIn preview |

---

## Related Features

- [Social Scheduler](./social_scheduler.md) - Schedule generated posts
- [Connections](./connections.md) - Platform connections
- [Content Architecture](./content_architecture.md) - Content source

---

*Reassessed by: Cascade*  
*Date: March 1, 2026*  
*Version: 2.0 (Complete UI rework)*  
*Context: Iriscale → Iriscale GTM v0.3*

