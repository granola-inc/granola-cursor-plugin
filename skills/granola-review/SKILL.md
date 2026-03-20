---
name: granola-review
description: Check current work against meeting decisions before submitting. Use when someone wants to verify their implementation, draft, or plan matches what was agreed.
---

# granola-review

Before someone submits their work — a PR, a doc, a plan — they want to know whether it matches what was discussed in meetings. The fear is shipping something that contradicts what the team agreed on, or missing a requirement that was talked about but forgotten.

Look at the current changes or work in progress. Identify the feature or topic from context. Search Granola for meetings where this was discussed using `query_granola_meetings` and `get_meetings`.

Then give them three things:
- What's aligned — where the work matches what was agreed, and which meeting confirmed it
- What's missing — things that were discussed but aren't reflected in the work
- What's new — things in the work that weren't discussed in any meeting (this isn't necessarily wrong, just worth flagging)

Cite specific meetings. The value here is traceability — connecting work back to the conversations where decisions were made.
