# LocalPersonas — Project Context

> **Read this at the start of every session.** This file is the single source of truth for project state, agent roster, active campaigns, blockers, and open action items.
> Last updated: 2026-04-29 by Declan (keyword tracker run 1 — reconstructed from agent memory files after file went missing)

---

## Product Overview

**LocalPersonas** is a SaaS tool that lets roofing contractors simulate how real local customers will react to their ads — before spending money on them. AI-powered personas provide honest feedback in ~30 seconds.

- **Tagline:** "Test Your Ads Before You Spend"
- **Site:** [localpersonas.com](https://www.localpersonas.com)
- **Owner:** Mike Volkin — mike@mikevolkin.com
- **LP business email:** mike@localpersonas.co
- **Stage:** Pre-launch / early traction (site indexed ~2026-04-07)
- **MailerLite account:** ID 2252341, email mike@localpersonas.co — 1 subscriber (owner seed only; signup forms not yet live)
- **GA4 property:** 523184396 (localpersonas.com) — NOT confirmed live/firing as of 2026-04-11

---

## Agent Roster

| Agent | Role | North Star Metric | Status |
|---|---|---|---|
| **Hunter** | Growth & RevOps | Free-to-paid conversion rate | Not yet run |
| **Gage** | AI Persona Engineer | Simulation accuracy/usefulness score | Not yet run |
| **Riley** | Content & Conversion Architect | Landing page CVR + email performance | Not yet run |
| **Blake** | Programmatic SEO Lead | Organic signups/month | Not yet run |
| **Sloane** | Social Proof & Inbound | Inbound signups from Instagram | Not yet run |
| **Miller** | Outbound Acquisition & Ads | Cost per free trial signup | Active — C1 TX campaign loaded |
| **Chen** | Product Success & Retention | Month 2 paid retention rate | Not yet run |
| **Ava** | Oversight & Improvement | Agent performance scores + gap identification | Not yet run |
| **Nora** | Content Research | Blog topic pipeline quality | Not yet run |
| **Warren** | Finance & CAC | Revenue pipeline accuracy | On hold (pending paid acquisition) |
| **Kai** | Analytics | Funnel insight quality and actionability | Stale — last run 2026-04-11 |
| **Marcus** | Social Listening | Roofing contractor pain signal quality | Active — 3 runs complete |
| **Celeste** | Brand Voice | Copy compliance rate across all agents | Active — 1 audit complete |
| **Tomas** | Systems & Ops | System uptime + zero data loss | Active — last backup 2026-04-21 |
| **Declan** | SEO | Keyword rankings + programmatic pages indexed | Active — first run 2026-04-29 |

---

## Scheduled Tasks (lp-*)

| Task | Agent | Cadence | Status |
|---|---|---|---|
| lp-declan-keyword-tracker | Declan | Weekly | Active — first run 2026-04-29 |
| lp-miller-daily-campaign-monitor | Miller | Daily | Active (last run 2026-04-09) |
| tomas-mailchimp-lead-logger | Tomas | Daily | Active (last run 2026-04-09) |
| tomas-critical-file-backup | Tomas | Regular | Active (last run 2026-04-21) |
| kai-booking-funnel-analysis | Kai | Mon/Thu | STALE — missed multiple windows |
| marcus-social-listening | Marcus | Recurring | Active — 3 runs complete |

---

## Active Campaigns

### C1 — TX Roofing Contractors (Cold Email)
- **Platform:** Instantly
- **Sending domains:** 20 warm-up domains via zapmail.ai
- **Lead count:** 955 TX roofing contractor leads
- **Status:** All 955 show "Not yet contacted" (as of 2026-04-09) — **verify Instantly is actively sending**
- **Email sequence:** 3 emails written; **Email 4 (local social proof) + Email 5 (case study) not yet written** — Riley action needed
- **CTA goal:** Drive to free trial signup

---

## Current Metrics (as of 2026-04-29)

| Metric | Value | Notes |
|---|---|---|
| Real subscribers (MailerLite) | 0 | Only owner seed account |
| Cold email replies | 0 | Instantly campaign unverified |
| Organic keyword rankings | 0 non-brand | Brand (#1 for "localpersonas") |
| Site age | ~3 weeks | Indexed ~2026-04-07 |
| GA4 traffic data | None | Tracking not confirmed live |
| Programmatic pages indexed | Unknown | Not detected by DataForSEO yet |

---

## Pain Signal Intelligence (Marcus)

18 pain signal themes documented across 3 runs. Top HIGH-signal themes:
1. Attribution blindness — "I don't know what's actually working"
2. Google Ads waste — 91% of keywords useless, 90% of roofers say PPC doesn't work
3. Facebook lead quality collapse — volume with zero conversion
4. Angi/HomeAdvisor shared leads — FTC-flagged, scathing reviews
5. Agency trust collapse — "burned by marketing companies"
6. LSA cost explosion + dispute removal (Google, mid-2025) — active grievance window
7. Channel-level job quality blindness (Theme 18, HIGH) — "optimize for job size, not lead volume" — direct upgrade to LocalPersonas value prop framing

**Hook map:** 13 trigger/angle pairs, 7 rated HIGH. See `social-listening-log.md`.

---

## Active Blockers (MUST RESOLVE)

| # | Blocker | Owner | Priority |
|---|---|---|---|
| 1 | GA4 tracking not confirmed live on localpersonas.com | Mike/Hunter | CRITICAL — blocks all funnel analytics |
| 2 | MailerLite signup forms not live | Mike/Hunter | CRITICAL — cold email → free trial loop is broken |
| 3 | Instantly C1 campaign send status unverified | Mike/Miller | HIGH — 955 leads may be sitting unsent |
| 4 | Email 4 + Email 5 not written | Riley | HIGH — sequence cuts off at email 3 |
| 5 | Reddit scrape not executed | Marcus/system | MEDIUM — needs Apify actor or Chrome MCP |
| 6 | Kai task schedule unreliable | Mike/Tomas | MEDIUM — missed multiple windows |
| 7 | Tomas task spec session path stale (nifty-funny-galileo) | Tomas | LOW — workaround in place |

---

## Open Action Items for Mike

1. **Verify GA4 is firing** on localpersonas.com (check GA4 > Admin > Data Streams, then DebugView)
2. **Activate MailerLite signup forms** — until live, no cold email → free trial conversion is possible
3. **Check Instantly** — confirm C1 TX campaign is actively sending (not paused)
4. **Assign Riley** to write Email 4 (local social proof: "a roofer in [city] used this") and Email 5 (case study)
5. **Enable Apify or Chrome MCP** for Marcus's Reddit scrape (r/Roofing, r/Contracting)
6. **Investigate Kai schedule** — missed Apr 7, Apr 9, and multiple subsequent windows
7. **Review Declan's keyword list** in Declan.md — confirm or expand the 8 baseline keywords for weekly tracking

---

## Key File Locations

| File | Location |
|---|---|
| Agent memory files | `Obsidian Vault/LocalPersonas/Agents/[Name].md` |
| Daily logs | `Obsidian Vault/LocalPersonas/Daily Logs/YYYY-MM-DD.md` |
| Social listening log | `Obsidian Vault/LocalPersonas/social-listening-log.md` |
| Funnel analysis | `Obsidian Vault/LocalPersonas/funnel-analysis/` |
| Lead tracking | `Obsidian Vault/LocalPersonas/leads-tracking.csv` |

---

## Notes

- This file was reconstructed 2026-04-29 after the original went missing. Cross-referenced all agent memory files and daily logs (Apr 7 – Apr 29) to rebuild. If anything is wrong or missing, update directly.
- `_PROJECT_CONTEXT.md` should be updated any time project state changes materially: new campaign launch, blocker resolved, agent status change, or metric movement.
