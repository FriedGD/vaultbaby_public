# 👶 VaultBaby

> **Search your baby's memories with natural language.**

[![Download App](https://img.shields.io/badge/Download-Release-blue)](#-download--install)
[![Demo Video](https://img.shields.io/badge/Watch-Demo-red)](#-demo)

VaultBaby is a **private, AI-powered family album** built around one core promise: you should be able to find your baby's memories by simply describing them. Instead of scrolling through thousands of photos, just ask — *"Find the photo where grandma is holding the baby"* — and VaultBaby does the rest.

---

## 📸 Screenshots & Demo

> *(Insert key screenshots here — main album view, SmartSearch in action, D+day calendar, etc.)*

![SmartSearch Demo](./assets/demo_video.gif)

---

## 🚨 Problem

Families capture a baby's growth every single day, but those memories quickly become scattered across phones, messaging apps, cloud albums, and family group chats. As the library grows, finding a specific moment becomes increasingly difficult.

Common pain points include:

- Parents must upload or forward the same media multiple times across different channels.
- Grandparents struggle to locate older photos buried in chat history.
- Paternal and maternal family groups often require separate sharing spaces.
- Photos are organized by file date, not by meaningful events or milestones.
- Videos are especially hard to search because their contents are invisible from filenames or thumbnails alone.

---

## 💡 Solution

VaultBaby solves this by turning a family's baby media into a **searchable, AI-indexed memory archive**.

When photos and videos are uploaded, VaultBaby automatically prepares searchable context for each memory. Photos are indexed through **VaultSage**, while videos — which VaultSage cannot process directly — are first analyzed by **Gemini**, which interprets scenes, actions, emotions, and milestones from the video content before passing the resulting metadata into the search pipeline.

The result is a family album that understands human questions.

---

## ✨ Key Features

### 🔍 SmartSearch — Natural Language Memory Search

SmartSearch is the core differentiator of VaultBaby. Family members can find baby memories using everyday language instead of manual filters or exact dates.

- Search by people, places, actions, emotions, events, and milestones.
- Works for both photos and videos.
- Example queries: *"Dad feeding the baby"*, *"smiling in the stroller"*, *"first birthday cake"*, *"beach last summer"*.

### 📅 D+day Calendar — Growth Timeline View

The D+day calendar organizes memories around the baby's growth timeline rather than acting as a conventional scheduling calendar.

- Displays uploaded memories by the baby's age in days (e.g., D+100, D+365).
- Helps families revisit growth milestones, daily records, and special events from the child's point of view.

### 👨‍👩‍👧‍👦 Separated Family Groups — Flexible Sharing Boundaries

VaultBaby supports multiple independent family groups, such as paternal family, maternal family, and custom groups.

- Each group has its own access boundary, so media and members can be managed independently.
- No need to create separate albums manually for different sides of the family.

### 🔗 Family Invitations — Simple Onboarding for Relatives

Parents can invite grandparents and relatives through shareable invite links. After signing in, invited members join the correct family group and view the child's album based on their permission level.

### 🛡️ Role-based Permissions — Admin & Viewer

| Role | Capabilities |
|---|---|
| **Admin (Parent)** | Upload media, manage family groups, register children, edit album information |
| **Viewer (Relative)** | Browse memories, use SmartSearch, leave comments and reactions |

---

## 🛠️ Tech Stack & Architecture

### AI & Search Pipeline

VaultBaby's intelligent search is powered by a two-stage AI pipeline designed to handle both photos and videos.

| Component | Role |
|---|---|
| **VaultSage** | Core search engine. Indexes photo metadata and AI-generated context to enable natural-language queries across the family album. |
| **Gemini API** | Video intelligence layer. Because VaultSage does not natively process video content, Gemini analyzes each uploaded video to extract scene descriptions, detected actions, emotions, and milestone events. The resulting text metadata is then fed into VaultSage for indexing, making videos fully searchable alongside photos. |

**Data Flow (Video Search):**

```
Video Upload → Gemini API (scene/action/emotion analysis)
             → Text Metadata → VaultSage Index
             → SmartSearch Query → Matching Results
```

**Data Flow (Photo Search):**

```
Photo Upload → VaultSage (AI metadata indexing)
             → SmartSearch Query → Matching Results
```

### Application Stack

> *(Fill in the technologies used in your implementation.)*

| Layer | Technology |
|---|---|
| **Frontend** | — |
| **Backend** | — |
| **Database** | — |
| **Storage** | — |
| **AI / Search** | VaultSage, Gemini API |
| **Auth** | — |

---

## 📥 Download & Install

| Platform | Link |
|---|---|
| **Android** | [Download APK from Releases](../../releases) |
| **iOS** | *(TestFlight or App Store link)* |
| **Web Demo** | *(Demo link, if available)* |

---

## 🔭 Future Directions

- Monthly and age-based growth recap pages.
- AI-detected milestone suggestions.
- Parenting document search (e.g., vaccination records, daycare notes).
- Family viewing insights and activity summaries.
- Personalized parenting assistance based on accumulated child records.

---

## 📧 Contact

| | |
|---|---|
| **Team** | *(Team name)* |
| **Email** | *(Contact email)* |
