---
name: weekly-status
description: Turn raw bullet-point notes into a formatted leadership status update with Shipped, In Progress, Blockers, and Next Week sections — max 3 bullets each, plain language, no jargon.
---

# Weekly Status Update

Turns raw, unstructured bullet notes into a concise, leadership-ready status update.

## Input

Raw bullet-point notes — whatever was jotted down during the week (tasks done, work in flight, issues, plans for next week). Notes may be messy, out of order, or mix multiple topics per line.

## Output format

**Shipped**
- (up to 3 bullets)

**In Progress**
- (up to 3 bullets)

**Blockers**
- (up to 3 bullets — write "None" if there are no blockers)

**Next Week**
- (up to 3 bullets)

## Rules

- Max 3 bullets per section. If more than 3 items belong in a section, keep the 3 most significant and drop or merge the rest — don't cram more in by shortening sentences.
- Plain, declarative language. No jargon, no buzzwords, no filler ("leveraging," "synergy," "circle back," "bandwidth"). Write each bullet as one clear sentence, the way you'd tell a colleague what happened.
- Don't invent shipped work, progress, or blockers that aren't in the input. If a section has nothing to report, write "None."
- Preserve the actual facts from the input — reformat and tighten wording, don't change the substance or add detail that wasn't there.
- Sort raw notes into the right section by what they actually describe (a note about something finished is Shipped, not In Progress; a note about something stuck is a Blocker, not In Progress), regardless of where it appeared in the input.

## Example

**Input notes:**
- finally got the streak-freeze API live in prod
- still working on eligibility logic, about 60% done
- waiting on design review for comeback screen mockups, blocking build
- also blocked bc analytics team hasn't given us the retention baseline query
- next week: finish eligibility logic, kick off comeback screen build once review lands

**Output:**

**Shipped**
- Streak-freeze API is live in production.

**In Progress**
- Eligibility logic for the Comeback screen — about 60% done.

**Blockers**
- Comeback screen build is blocked on design review of the mockups.
- Retention baseline query is blocked on the analytics team.

**Next Week**
- Finish eligibility logic.
- Kick off Comeback screen build once design review lands.
