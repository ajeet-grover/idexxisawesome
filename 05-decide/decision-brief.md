# Decision Brief — Streakly Comeback Experience

> For: Marcus, Head of Product. Synthesized from [interview-synthesis.md](../02-research/interview-synthesis.md), [nps-analysis.md](../02-research/nps-analysis.md), and [competitive-matrix.md](../02-research/competitive-matrix.md). 2026-09-28.

## Situation

Streakly's Day-7 retention dropped from 48% to 39% since the v2 streak redesign shipped, driven mainly by users who break a streak in week 1 and don't come back. Three independent sources — user interviews, NPS feedback, and competitive research — now confirm the same root cause: the all-or-nothing streak reset, not just notification tone.

## Key Findings

- **All three sources converge on the same root cause.** User interviews (Tom: "there was no way to recover it... so I gave up"), NPS (3 of 10 responses cite the reset itself as the reason they quit), and competitive research (no competitor offers real post-break recovery either) all point to the zero-reset as the primary driver — not a secondary factor.
- **Streak anxiety starts before any break happens.** Amara, 4 days into the product with no break yet, already describes the streak as "a chore instead of a game" — a data point interviews surfaced that NPS and competitive research don't cover, suggesting the fix window may need to start earlier than the moment of the break.
- **Users already switch products for exactly this reason, and it's happening to Streakly today.** Tom left Streakly for Duolingo specifically because Duolingo's streak freeze "feels forgiving" — this matches the competitive finding that Duolingo's own move toward a harsher mechanic (the new Energy system) triggered a visible uninstall wave, with some users moving to gentler Babbel. The market rewards moving away from punitive mechanics, not toward them.
- **No competitor has solved this either — it's genuine white space.** Every freeze mechanic in the competitive set (Duolingo, Elevate) must be banked *before* a miss; none acknowledge a break after it happens or personalize the response to why it happened. Nothing in NPS or interviews contradicts this — users explicitly ask for something none of these apps currently offer.
- **Notification design is a real but secondary complaint.** NPS flags nagging/random notifications (2 of 10 responses), distinct from the reset problem — worth fixing, but not the primary lever on the data so far.

## Options Considered

1. **Build the Comeback experience** (best-streak stat, comeback lesson, one-tap streak-freeze) at the moment a streak breaks — directly targets the most-repeated finding across all three sources.
2. **Address anxiety upstream, before any break** — e.g., softer framing or a grace period for week-1 users — targets the Amara finding, but is based on one interview subject, not yet corroborated by NPS or competitive data.
3. **Fix notifications only** — lowest lift, but treats a secondary complaint as the whole fix and leaves the primary churn driver (the reset itself) unaddressed.

## Recommended Action

Build the post-break Comeback experience (Option 1) as the primary fix, since it's the most repeated finding across all three sources and claims white space no competitor currently owns; scope notification fixes as a fast follow, and treat upstream anxiety (Option 2) as an open question worth validating with more data before committing to it.

## Why Now

Retention has already dropped 9 points with no sign of stabilizing, a competitor's move toward a harsher mechanic is visibly costing them users right now — proof the market will reward the opposite move — and three independent sources have converged on the same root cause, which is as much validation as this problem is likely to get before committing engineering time.
