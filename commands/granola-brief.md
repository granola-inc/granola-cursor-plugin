---
name: granola-brief
description: Synthesize everything discussed about a topic across meetings into a briefing document.
---

# granola-brief

Someone needs to get oriented on a topic — a project, a client, a strategic question, a person. They want a single document that pulls together everything that's been discussed across their meetings, so they don't have to piece it together themselves.

This is useful for onboarding onto a project, preparing for a high-stakes conversation, getting back up to speed after time away, or just collecting scattered meeting discussions into one place.

Ask what they want a brief on. Use `query_granola_meetings` for a broad search, then `list_meetings` and `get_meetings` to find all relevant discussions chronologically.

Also check for upcoming meetings related to the topic. Use `list_meetings` with a custom range extending a week or two into the future. If there are upcoming calls with relevant people or on the relevant topic, include them at the end of the brief — "you have a call with [person/team] on [date]" — so the reader knows what's coming next, not just what's happened.

Build the brief as a narrative: how the topic first came up, how the thinking evolved, where it stands now. Include who was involved and what they said. Surface any unresolved tensions or open questions.

If the meetings suggest that important context may have moved to async channels — someone said "let's take this offline," a decision was deferred to Slack, or there's a gap between meetings where things clearly progressed — note that in the brief and offer to check Slack or other connected tools for what happened in between.

The goal is a document that would let someone who wasn't in any of those meetings understand the full picture — what happened, what was decided, what's still live, and what's coming up.
