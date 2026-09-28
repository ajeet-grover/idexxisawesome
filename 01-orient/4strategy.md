# Strategy — Recovering the Day-7 Retention Drop

> Hypothesis document. Feeds off [project.md](project.md). To be validated during discovery, not treated as confirmed.

## The Gap

Day-7 retention dropped 9 points — from 48% to 39% — since the v2 streak redesign shipped.

## Hypothesis

Users go passive after breaking a streak because the break feels like failure and there's no graceful way back in. Specifically:

- The sharpest drop is among users who break their streak in week 1 — missing two days in a row roughly doubles churn (Raj's data).
- The app currently offers no acknowledgment of the break — same home screen, counter reset to zero (Lena's research).
- The "you lost your streak" push notification has a harsh tone, and tapping through it drops the user back at day zero with nothing else offered.

It's not yet confirmed how much of the 9-point drop is attributable to the reset/no-acknowledgment experience itself versus notification tone/timing — likely both contribute, but the post-break in-app experience is believed to be the larger driver.

## Approach

1. **Validate root cause first** — before designing a solution, confirm from data and user feedback whether the drop is driven by the streak-reset experience, notification tone/timing, or both, and how much each contributes. (This is the key discipline for this phase — see [CLAUDE.md](../CLAUDE.md) "Key tension.")
2. **If confirmed, intervene at the moment of the break** with a "Comeback" experience instead of a cold reset — the three elements already sketched: best-streak stat, 60-second comeback lesson, one-tap streak-freeze. (Full detail in [project.md](project.md).)

## Open Questions

- How much of the 9-point drop is reset/acknowledgment vs. notification-driven?
- Targeting/eligibility logic for who sees the Comeback screen.
- Streak-freeze rules (limits, cooldowns).
- Whether notification tone/timing needs its own workstream.

---
*Log entry: [change_log.md](change_log.md).*
