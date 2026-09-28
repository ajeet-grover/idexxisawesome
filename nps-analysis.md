# NPS Feedback Analysis — Findings Report

> For: Marcus. Source: 10 raw NPS responses, captured 2026-09-28. Method: manual theme extraction across all 10 responses; frequency = number of distinct responses touching a theme.

## 1–2. Themes Mentioned More Than Once, Ranked by Frequency

| Rank | Theme | Type | Frequency |
|---|---|---|---|
| 1 (tie) | Losing the streak kills motivation and drives users to quit/uninstall | Complaint | 3 |
| 1 (tie) | No way to recover a broken streak; users want a "coach," not a "scorekeeper" | Complaint / request | 3 |
| 3 (tie) | Notifications feel nagging or random, leading to opt-out | Complaint | 2 |
| 3 (tie) | Lesson content itself is enjoyable | Praise | 2 |

Two additional points were each mentioned once, not enough to rank as a repeated theme, but worth noting: (a) the home screen gives no acknowledgment of a user's actual state (2-day streak vs. returning after two weeks look identical), and (b) some users disengage by simply forgetting the app exists, and say a *useful* pull-back would bring them back.

## 3. Praise vs. Complaints

**Praise (2 mentions)**
> "The first week was genuinely fun."
> "Love the lessons."

**Complaints (8 mentions across the other themes)**
- Streak reset causes disengagement/churn (3): "felt pointless to start over," "the moment I lost my streak the whole thing lost its meaning," "the second I lost it, I was done."
- No recovery/forgiveness mechanism (3): "no way to recover it, other apps let you freeze a streak," "coach... not a scorekeeper," "make coming back easier instead of making me feel like I failed."
- Notifications nagging/random (2): "daily reminder just started to feel like nagging," "notifications feel random... turned them all off."
- Single mentions: no acknowledgment of user state on home screen; forgets app exists and wants a useful pull-back rather than a generic reminder.

## 4. Top 3 Actionable Issues

1. **No recovery path after a streak breaks.** Users explicitly want a forgiveness mechanism and name a competitor (streak freeze) that already has one. This is the most directly actionable and most repeated request in the data (3 mentions), and it lines up with the Comeback screen already sketched in [4strategy.md](../01-orient/4strategy.md).
2. **The reset itself reads as total, meaningless loss.** Three users describe quitting outright once the streak hit zero — the fix isn't just adding a recovery option, but changing what the user sees at the moment of the break (e.g., acknowledging progress/state instead of a blank reset), which also addresses the single mention about the home screen looking the same regardless of streak state.
3. **Notification volume/relevance is causing opt-out, not re-engagement.** Two complaints about nagging/random notifications, plus one user who'd respond to a "useful" pull-back instead of a generic reminder — suggests fixing frequency and personalization, not just tone.

## 5. Summary for Marcus

The two loudest complaints (streak reset = churn, and no recovery path) point to the same root cause the team already flagged from the Slack thread and user interviews: the all-or-nothing streak mechanic. This NPS data adds two things not yet in our existing docs: notification complaints are about volume/randomness (not just tone), and a subset of disengaged users aren't reacting to a broken streak at all — they're drifting away and want a relevant nudge back. Recommend treating the recovery-mechanism build as the top priority, with notification relevance as a fast, lower-lift follow-on.
