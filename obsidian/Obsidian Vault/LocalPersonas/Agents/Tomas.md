# Tomas — LocalPersonas Agent Memory

**Role:** Systems & Ops — North Star: System uptime + zero data loss

---

## Current Status
Critical file backup complete (2026-04-21). 15 files backed up (11 agent memory + 4 content). Agents updated today: celeste, marcus, nora, priya. Persistent stale agents: dana (9d), kai (16d), jonah (14d) — escalate.

## Last Run Summary
tomas-critical-file-backup (2026-04-21): Backed up all 11 agent memory files and 4 content files (email-queue AM/PM, meta-creative-review, weekly-content-review) to `/FIT/backups/2026-04-21/`. MANIFEST.md written with full inventory and stale flags. 4 agents updated today (celeste, marcus, nora, priya). 7 not updated — 3 are escalation-level stale (dana 9d, kai 16d, jonah 14d). Session path in task spec remains stale (nifty-funny-galileo); resolved to active session (zen-wonderful-brahmagupta).

## Running Notes
- Task spec still references stale session path — always resolve to active session workspace. Needs a permanent fix.
- Declan is PRE-LAUNCH — stale memory is expected until first-run tasks are enabled.
- `_PROJECT_CONTEXT.md` was not found in Obsidian vault root — 5th consecutive agent run to flag this. Mike needs to create or restore this file.
- MailerLite account (ID: 2252341, email: mike@localpersonas.co) confirmed connected. Only 1 subscriber — signup forms may not be live yet.

## Open Issues / Flags
- DANA: Daily travel advisory gap now 9+ consecutive days (last update Apr 12). CRITICAL — escalate.
- KAI: No update since Apr 5 (16 days). Analytics agent — missed many Mon/Thu windows. CRITICAL — escalate.
- JONAH: No update since Apr 7 (14 days). NPS outreach agent — investigate task schedule.
- AVA: No update since Apr 13 (8 days). Check task health.
- WARREN: No update since Apr 13 (8 days). Check task health.
- OBSIDIAN: `_PROJECT_CONTEXT.md` not found in vault root — 5th agent run flagging this. Mike action required.
- TASK SPEC: Session path (nifty-funny-galileo) is stale — needs permanent update to dynamic resolution.

## Log
| Date | Task | Key Output | Flags |
|---|---|---|---|
| 2026-04-09 | tomas-critical-file-backup (run 1) | 18 files backed up; MANIFEST.md written | Ava + Dana stalls — escalate via watchdog |
| 2026-04-09 | tomas-mailchimp-lead-logger | 0 new subscribers; leads-tracking.csv created | MailerLite may not have active signup forms yet |
| 2026-04-09 | tomas-critical-file-backup (run 2) | 22 files catalogued; all memory files refreshed | Dana (3d), Kai (4d) stale — escalate; Jonah revision unconfirmed |
| 2026-04-21 | tomas-critical-file-backup | 15 files backed up; MANIFEST written | Dana (9d), Kai (16d), Jonah (14d) stale — escalate; _PROJECT_CONTEXT.md still missing (5th flag) |
