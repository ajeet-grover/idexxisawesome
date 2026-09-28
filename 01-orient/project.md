# Streakly — Comeback Experience Project

> Starting point for alignment before Thursday's meeting. Not a finished document.

## Overview

**What Streakly is:** A consumer habit + micro-learning app. Users pick a track and do a 5-minute daily lesson; the streak is the core habit loop. Launched 4 years ago, Series B funded ($42M), 2.1M registered users, 340K MAU, growing 28% YoY on MAU.

**Squad:** Engagement squad.

**Current phase:** Discovery — validating root cause of the Day-7 retention drop (data + user feedback) before designing solutions. See [4strategy.md](4strategy.md) and [change_log.md](change_log.md).

**Key stakeholders:** Marcus, Raj, Lena (from the originating Slack thread; specific roles/titles not yet confirmed).

## Problem Statement

Day-7 retention has dropped from 48% to 39% since the streak redesign shipped. The drop is sharpest among users who break their streak in week 1 — once someone misses two days in a row, churn is almost double.

Working hypothesis: users go passive after breaking a streak because it feels like failure, and there's no graceful way back. Today, when a user breaks a streak:
- The app resets the counter to zero with no acknowledgment of what happened — same home screen as if nothing occurred.
- The "you lost your streak" push notification has a harsh tone.
- Tapping through the notification drops the user back at day zero with nothing else offered.

It's unclear how much of the retention drop is driven by the reset/reaction itself vs. notification timing/tone — likely both, but the post-break experience (no acknowledgment, no path back) is believed to be the bigger issue.

## Goals

Give users a specific, personalized reason to come back after breaking a streak — not a generic "keep going!" message. Replace the cold reset with a "Comeback" experience at the moment a streak breaks, built from the three elements Lena sketched:

- **Best-streak stat** — show the user's personal best instead of just the reset counter, so progress isn't erased from view.
- **60-second comeback lesson** — a short lesson to rebuild momentum immediately, rather than dropping the user back at day zero with nothing to do.
- **One-tap streak-freeze** — lets a user protect a rebuilt streak going forward.

Per Raj, this is technically doable with existing data sources — no new data infrastructure is required. The main open engineering work is the targeting/eligibility logic and the freeze rules (see Non-Goals).

## Non-Goals

Explicitly out of scope for this PRD — flagged as open questions for follow-up, not resolved here:

- **Targeting/eligibility logic** — the rules for who sees the Comeback screen (e.g., which streak-break scenarios trigger it) are not yet defined.
- **Streak-freeze rules** — limits, cooldowns, or eligibility for the one-tap freeze are not yet defined.
- **Notification tone/timing** — Lena flagged the "you lost your streak" push as having a harsh tone, and Marcus raised whether notification timing itself contributes to churn. Both are real, related problems, but this PRD scopes the in-app Comeback experience, not a notification redesign.

## Success Metrics

No target metrics were set in the thread — these are candidates proposed to seed discussion, not agreed targets:

- **Day-7 retention rate** — the headline metric already in play (39%, down from 48%); track recovery against this baseline.
- **Return rate after a streak break in week 1** — directly tied to Raj's observation that churn roughly doubles once a user misses two days in a row; this is the population the Comeback experience targets.
- **Comeback screen engagement** — % of users who see the screen and complete the comeback lesson, and % who use the streak-freeze, as leading indicators before retention impact is measurable.
- **Streak-break push performance** — tap-through and opt-out rate on the "you lost your streak" notification, as a proxy for whether the harsh tone is actually driving disengagement (per Lena's research).

These need validation with the team (and likely a baseline pull from analytics) before Thursday.

---
*Source: Slack thread (Marcus, Raj, Lena) — captured 2026-09-28. To be discussed further at Thursday's meeting.*
