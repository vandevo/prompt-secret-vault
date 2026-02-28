---
title: "Stack Audit & Ecosystem Map"
version: "1.1"
tags: ["knowledge", "tech-stack", "ops", "audit"]
author: "Van"
description: "Current operational snapshot of the Worktugal ecosystem. Reflects the full migration to Cloudflare Pages static infra and EmailOctopus decoupling."
model: "gemini-3-pro"
last_updated: "2026-02-28"
---

# Operational Philosophy: "Headless & Sovereign"
We have successfully exited the Google Cloud VM/cPanel infrastructure to eliminate financial drag and manual dependency.
- **Rule 1**: The public frontend is **Static-First** (Cloudflare Pages) for speed and security.
- **Rule 2**: Database and Auth are **Supabase-First**.
- **Rule 3**: All marketing automation is **Decoupled** from WordPress.
- **Rule 4**: Data sovereignty is priority (Own the list, own the code, own the domain).

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

# 2. The Cloud Infrastructure (Active Stack)

| Component | Tool | Config/Notes |
| :--- | :--- | :--- |
| **Hosting (Static)** | **Cloudflare Pages** | worktugal.com served as static export (Simply Static). |
| **DNS/Security** | **Cloudflare** | Global CDN, WAF, full DNS management. |
| **Database** | **Supabase** | Postgres, Auth, Realtime. The **Canonical Data Source**. |
| **Email (Inbound)** | **Namecheap Private Email** | Detached from VM. Handles hello@worktugal.com. |
| **Email (Outbound)** | **Amazon SES** | High-volume transactional + campaign delivery. |
| **Automation** | **Make.com** | Glue between Supabase, SES, and EmailOctopus. |
| **Dev Repo** | **GitHub** | Source of truth. CI/CD to Cloudflare. |

# 3. Marketing & Distribution

| Component | Tool | Status/Notes |
| :--- | :--- | :--- |
| **Email Campaigns** | **EmailOctopus** | **Active.** Connected to Amazon SES. Owns the list. |
| **Payments** | **Stripe** | Merchant of Record. Connected to Supabase/Make. |
| **No-Code DB** | **Airtable** | Operational tracker for leads and partners. |
| **Social** | **Publer / Buffer** | Transitioning to AI-automated distribution. |
| **Visual UI** | **Stitch (Google)** | AI UI prototyping & design system. |

# 4. Legacy / Paused / Decommissioned

- **WordPress (Live VM)**: **Decommissioned.** Google VM stopped to save €37/mo.
- **FluentCRM Pro**: **Legacy.** Contacts migrated to EmailOctopus.
- **CPanel/WHM**: **Retired.**
- **HireSignal**: Paused. Recognized but inactive.
- **Bolt.new**: Deprecated. Replaced by Cursor + Local Dev.
- **Netlify**: Deprecated. Replaced by Cloudflare Pages.
- **Luma/Zoom/Read.ai**: Paused.

# 5. Future Migration Path (The Roadmap)

1.  **AI-Native CMS**: Rebuild the publishing pipeline inside `app.worktugal.com` using Supabase.
2.  **VM Final Delete**: Permanently delete stopped Google VM once dependencies are 100% verified.
3.  **Affiliate Program**: Launch Worktugal partner/affiliate portal inside the new app.
4.  **Community Shift**: Migrate legacy groups to Reddit/Discord for AI-era relevance.

---

`VanStackAudit v1.1 Active`

## Operator Take
The infrastructure debt is gone. We are now running a lean, static frontend with a sovereign backend. The next move is building the AI CMS to reclaim publishing velocity without the WordPress bloat.
