---
name: granola-context
description: Look up meeting discussions, decisions, or scheduled meetings. Use when the user asks about a meeting or explicitly connects their current task to something discussed or agreed in a meeting. Do not use for routine implementation, debugging, or design work without a meeting reference.
---

# granola-context

Use this skill when meeting context is relevant to the user's request — for example, "what did we decide in the planning meeting?", "implement the approach we agreed on in yesterday's call", or "what did Alex say about this in the review?" Retrieve the relevant context rather than asking the user to recall it from memory.

A feature request, bug fix, design choice, person's name, or reference to the current chat is not by itself a reason to search meetings. If the needed meeting context is already in the conversation, use it without another lookup unless the user asks for verification or newer information, or relevant details are missing.

Use `query_granola_meetings` with the meeting question or the specific context needed for the task. For requests about upcoming meetings or future calls, use `list_meetings` with the requested date range, or the next week or two if none is specified.

Return a concise answer — the decision or information, which meeting it came from (title and date), and who was involved. If the answer came up across multiple meetings, note whether the thinking evolved or stayed consistent.

If the answer feels incomplete — like context clearly moved to async channels between meetings — briefly note that and offer to check Slack or other connected tools.

Keep it brief. The person asking is in the middle of something and wants a quick, citable answer — not a report.
