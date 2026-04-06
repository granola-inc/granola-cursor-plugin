---
name: granola-gaps
description: Find what was discussed in meetings but hasn't shown up in code yet.
---

# granola-gaps

A developer wants to know what they've missed. Meetings produced decisions, requirements, and action items — some of that has been built, some hasn't. This command finds the gaps.

Ask what project or feature to check, or infer it from the current repo. Establish a time range — default to the last two weeks, but ask if they want to go further back.

Use `query_granola_meetings` to find meetings where requirements, action items, or implementation details were discussed for this project. Use `list_meetings` with the time range to catch meetings the semantic search might miss. Use `get_meetings` for detailed content.

From the meetings, collect everything that sounds like it should result in a code change: features to build, bugs to fix, refactors to do, endpoints to add, behaviour to change, technical decisions to implement. Include who raised it and when.

Then look at the codebase: recent git history (`git log`), current diffs, file changes, and the state of the code. Try to match each meeting item against actual work — a commit that addresses it, a file that implements it, a PR that covers it.

Produce a report with three sections:
- **Done** — discussed in meetings and reflected in code, with the meeting reference and the commit/file that covers it
- **Not started** — discussed but no corresponding code changes found
- **Partially done** — work has started but doesn't fully cover what was discussed

For "not started" items, note when they were discussed and whether they were assigned to anyone specific. If something was discussed in multiple meetings without being actioned, flag that — it's either deprioritised or falling through the cracks, and the developer should know which.

Don't flag things that were clearly deferred or explicitly deprioritised in a later meeting. If a March 3 meeting said "build X" but a March 10 meeting said "actually, X is parked until Q3," that's not a gap.
