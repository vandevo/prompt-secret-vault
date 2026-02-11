---
title: "Stack Audit & Ecosystem Map"
version: "1.0"
tags: ["knowledge", "tech-stack", "ops", "audit"]
author: "Van"
description: "Current operational snapshot of the Worktugal/HireSignal ecosystem. Defines the transition from Legacy WP to AI-Native/Cloudflare stack."
model: "gemini-3-pro"
last_updated: "2026-02-08"
---

# Operational Philosophy: "Headless & Hybrid"
We are in a **Transition Phase** (Legacy Cashflow → AI-Native Future).
- **Rule 1**: Do not break the legacy flywheel (WordPress/SEO) while building the new engine.
- **Rule 2**: All new builds are **AI-First** (Cursor + Vibe Coding) and **Serverless** (Cloudflare/Supabase).
- **Rule 3**: Data sovereignty is priority (Own the list, own the code, own the domain).

# 1. The Core Engines (Daily Drivers)

| Category | Tool | Role/Status | Cost/Credits |
| :--- | :--- | :--- | :--- |
| **IDE / Brain** | **Cursor Pro** | **Primary OS.** Code, Prompts, Knowledge. | Paid |
| **Model (Fast)** | **Gemini 3 Flash** | Daily driver. Default model in Gemini app. | Free/API |
| **Model (Smart)** | **Gemini 3 Pro** | Deep logic, architecture, complex refactors. | Free/API |
| **Model (Senior)** | **Claude Opus 4.6** | Senior Engineer. Agentic coding, complex refactors. | Paid |
| **Search/Research** | **Perplexity Pro** | Deep research, fact-checking, market scans. | Paid |
| **Agentic Search** | **Parallel AI** | Batch processing, deep data enrichment. | API |
| **Research Task** | **Deep Research (GPT-5.3)** | Analyst-grade reports. | Paid |

# 2. The Cloud Infrastructure (New Stack)

| Component | Tool | Config/Notes |
| :--- | :--- | :--- |
| **Hosting** | **Cloudflare Pages** | All new web apps (Static/Vite/Next). Fast, free, secure. |
| **DNS/Security** | **Cloudflare** | Global CDN, WAF, DNS management. |
| **Database** | **Supabase** | Postgres, Auth, Realtime. Replaces Netlify/Firebase. |
| **Backend Logic** | **Edge Functions** | Cloudflare Workers / Supabase Edge Functions. |
| **Visual UI** | **Stitch (Google)** | New AI UI prototyping & design system. |
| **Dev Repo** | **GitHub** | Source of truth. CI/CD actions to Cloudflare. |

# 3. The Legacy Cashflow Engine (Do Not Break)

| Component | Tool | Status/Notes |
| :--- | :--- | :--- |
| **CMS** | **WordPress** | Content flywheel, SEO authority (5y domain age). |
| **Hosting** | **CPanel/WHM** | Legacy hosting. Keeps the lights on. |
| **Email Mktg** | **FluentCRM Pro** | **Critical.** Integrated WP CRM. Amazon SES backend. |
| **Email Sending** | **Amazon SES** | Dirt cheap delivery. High deliverability. |
| **Forms** | **FluentForms** | Data capture. |
| **SEO** | **RankMath** | On-page optimization. |
| **Speed** | **LiteSpeed Cache** | Essential for WP performance. |
| **Backup** | **UpdraftPlus** | Safety net. |

# 4. The SaaS / Ops Layer

| Category | Tool | Use Case |
| :--- | :--- | :--- |
| **Automation** | **Make.com** | Glue between WP, Stripe, and Email. |
| **Payments** | **Stripe** | The Merchant of Record. Global payments. |
| **Database (No-Code)** | **Airtable** | Operational data, applicant tracking, content calendar. |
| **Scheduling** | **Cal.com** | Booking API (superior to Calendly). Future integration. |
| **Social** | **Publer / Buffer** | Social scheduling (Transitioning to AI automation). |
| **Design** | **Adobe Express** | Quick visuals (moving to AI generation). |
| **Images** | **Google Imagen 4** | AI asset generation (Vertex AI). |

# 5. Legacy / Paused Projects

- **HireSignal**: Paused. Recognized but inactive.
- **Bolt.new**: Deprecated. Replaced by Cursor + Local Dev.
- **Netlify**: Deprecated. Replaced by Cloudflare Pages.
- **Zoom/Read.ai**: Paused. No active webinar funnel.
- **Luma**: Paused. No IRL events currently.
- **Facebook Group**: Dead channel.
- **Instagram**: Dormant. Potential revival.

# 6. Future Migration Path (The Roadmap)

1.  **Email Decoupling**: Move from FluentCRM (WP) → **EmailOctopus + AWS SES**.
    -   *Why*: Remove dependency on WordPress plugin ecosystem. Own the list in a dedicated platform.
2.  **Community Shift**: Move from FB/Telegram → **Reddit/Discord** (AI-Era relevance).
3.  **Affiliate Layer**: Investigate platforms for Worktugal Affiliate Program.

---

`VanStackAudit v1.0 Active`

## Operator Take
The stack is split: Old World (WordPress) pays the rent; New World (Cursor/Cloudflare) builds the empire. We maintain the Old to fund the New.
