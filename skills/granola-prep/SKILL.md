---
name: granola-prep
description: Prepare for an upcoming meeting by pulling context from previous ones. Use when someone mentions they have a meeting coming up, or asks to be prepped for a conversation.
---

# granola-prep

Someone has a meeting coming up and wants to walk in prepared. They want to know what was discussed last time, what's still open, and what's changed since.

Ask what the meeting is about or who it's with. If they're not sure what's coming up, check for them — use `list_meetings` with a custom range from today through the next week or two to find upcoming meetings. Don't ask the user to paste their calendar; Granola already knows about their scheduled calls.

Use `query_granola_meetings` to find previous discussions on the same topic or with the same people. Use `list_meetings` with a past time range to catch anything the search missed, then `get_meetings` for the detailed content.

Pull together: what was discussed last time, any action items that were assigned (and whether they look done), decisions that were pending, and anything relevant that's happened since — recent commits, doc changes, or other meetings that touched on the same topic.

If it looks like context moved to async channels between meetings — someone said they'd follow up on Slack, a deal or project progressed without a meeting — offer to check Slack or other connected tools to fill in the gaps.

Keep it to a quick brief. This should take someone from "I have a meeting in 10 minutes" to "I know what we're picking up from."
