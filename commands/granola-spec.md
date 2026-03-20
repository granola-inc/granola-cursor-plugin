---
name: granola-spec
description: Build a structured spec from meeting discussions about a feature or project.
---

# granola-spec

Someone needs to turn meeting conversations into a spec they can build from. They've discussed a feature or project across one or more meetings, and now they need it written down properly — requirements, constraints, decisions, and open questions, all traced back to where they came from.

Ask what feature or topic to spec, or infer it from the current project context. Use `list_meetings` and `get_meetings` to find all relevant discussions. For ambiguous points, use `get_meeting_transcript` to pull exact wording.

From the meetings, extract:
- Requirements that were stated or agreed on
- Constraints or limitations that were mentioned
- Decisions that were made, and who made them
- Open questions that weren't resolved
- Dependencies on other work or teams

If different meetings said different things about the same topic, surface the contradiction clearly — "the March 3 meeting decided X, but the March 7 discussion leaned toward Y." Don't silently resolve these; the person needs to know they exist.

Produce a SPEC.md with everything traced to specific meetings (title and date). This should be something the team can review, reference during implementation, and use to verify the work when it's done.
