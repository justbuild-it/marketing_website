# Connections

> **Status:** ✅ Documented  
> **Last Updated:** 2026-01-17  
> **URL Pattern:** `/connections`

---

## Overview

Social Connections is the platform authentication hub where users connect their social media accounts to enable automated posting and scheduling. The feature supports 7 major social platforms with OAuth-based connections.

---

## Page Layout

```
┌─────────────────────────────────────────────────────────────────────────┐
│ Header: Org/Project Selector                                            │
├─────────────┬───────────────────────────────────────────────────────────┤
│             │ Social Connections                                        │
│             │ Manage your social media accounts and active profile      │
│   Sidebar   ├───────────────────────────────────────────────────────────┤
│             │ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐        │
│             │ │ Not Connected│ │ Not Connected│ │ Not Connected│        │
│             │ │ [Facebook]   │ │ [Instagram]  │ │ [X/Twitter]  │        │
│             │ │ Pages,Groups │ │ Posts,Stories│ │ Tweets,Thread│        │
│             │ │ [Connect]    │ │ [Connect]    │ │ [Connect]    │        │
│             │ │ [Invite]     │ │ [Invite]     │ │ [Invite]     │        │
│             │ └──────────────┘ └──────────────┘ └──────────────┘        │
│             │ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐        │
│             │ │ [LinkedIn]   │ │ [TikTok]     │ │ [YouTube]    │        │
│             │ │ Posts,Articles│ │ Videos,Live │ │ Videos,Shorts│        │
│             │ └──────────────┘ └──────────────┘ └──────────────┘        │
│             │ ┌──────────────┐                                          │
│             │ │ [Reddit]     │                                          │
│             │ │ Posts,Comment│                                          │
│             │ └──────────────┘                                          │
└─────────────┴───────────────────────────────────────────────────────────┘
```

---

## Supported Platforms

| Platform | Features | Content Types |
|----------|----------|---------------|
| **Facebook** | Business pages | Pages, Groups, Ads Manager |
| **Instagram** | Business accounts | Posts, Stories, Reels |
| **X (Twitter)** | Personal/Business | Tweets, Threads, Spaces |
| **LinkedIn** | Company pages | Posts, Articles, Company Updates |
| **TikTok** | Business accounts | Videos, Live, Ads |
| **YouTube** | Channels | Videos, Shorts, Live Streaming |
| **Reddit** | Personal accounts | Posts, Comments, Communities |

---

## UI Components

### Platform Card
| Element | Description |
|---------|-------------|
| **Status Badge** | Not Connected / Connected |
| **Platform Icon** | Visual identifier |
| **Platform Name** | Facebook, Instagram, etc. |
| **Description** | Account type description |
| **Feature Tags** | Supported content types |
| **Connect Account** | OAuth connection button |
| **Generate Invite Link** | Team member invitation |

### Connection Actions
| Action | Description |
|--------|-------------|
| **Connect Account** | Initiate OAuth flow |
| **Generate Invite Link** | Create shareable link for team members |
| **Disconnect** | Remove platform connection (when connected) |

---

## Connection Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                     User Clicks "Connect Account"                    │
└─────────────────────────────────────┬───────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────┐
│                     OAuth Redirect to Platform                       │
│                     (Facebook, LinkedIn, etc.)                       │
└─────────────────────────────────────┬───────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────┐
│                     User Authorizes Permissions                      │
└─────────────────────────────────────┬───────────────────────────────┘
                                      │
                                      ▼
┌─────────────────────────────────────────────────────────────────────┐
│                     Return to Iriscale                               │
│                     Connection Stored                                │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Key Capabilities

| Capability | Description |
|------------|-------------|
| **OAuth Integration** | Secure platform authentication |
| **Multi-Platform** | 7 major platforms supported |
| **Team Sharing** | Invite links for team members |
| **Organization-Level** | Connections shared across projects |
| **Auto-Refresh** | Token management |

---

## Screenshots

| Screenshot | Description |
|------------|-------------|
| `connections_main.png` | Main connections grid |

---

## Related Features

- [Social Posts](./social_posts.md) - Create posts for platforms
- [Social Scheduler](./social_scheduler.md) - Schedule to platforms

