---
name: granola-context
description: Look up what was discussed or decided in meetings. Use when someone asks about a past discussion, needs to recall a decision, or references something that was talked about in a meeting.
---

# granola-context

Someone is mid-work and needs to check what was discussed or agreed. Maybe they're implementing something and want to confirm the approach. Maybe they're writing a doc and need to recall who said what. Maybe they just can't remember whether a decision was actually made or only floated. Or maybe they want to know what's coming up — upcoming calls, scheduled check-ins, future meetings on a topic.

Use `query_granola_meetings` with their question. If the question is about upcoming meetings or future calls, also use `list_meetings` with a custom range extending into the next week or two — Granola knows about scheduled meetings, so don't ask the user to paste their calendar.

Return a concise answer — the decision or information, which meeting it came from (title and date), and who was involved. If the answer came up across multiple meetings, note whether the thinking evolved or stayed consistent. If there are upcoming meetings related to the topic, mention them.

If the answer feels incomplete — like context clearly moved to async channels between meetings — briefly note that and offer to check Slack or other connected tools.

Keep it brief. The person asking is in the middle of something and wants a quick, citable answer — not a report.
