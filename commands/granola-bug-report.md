---
name: granola-bug-report
description: Turn a bug walkthrough call into a structured bug report.
---

# granola-bug-report

Someone just got off a call where a user or teammate walked them through a bug. The conversation is in Granola — now they need a structured write-up they can hand to the engineering team or drop into a ticket.

Ask which meeting or look for the most recent one that sounds like a bug walkthrough. Use `get_meetings` and `get_meeting_transcript` to pull the discussion and exact quotes.

From the conversation, extract:
- What the person reported happening, in their own words
- Steps to reproduce, pieced together from the walkthrough ("they clicked X, then Y, then it broke")
- Expected behaviour vs what actually happened
- Any environment details mentioned — browser, OS, account type, plan tier, specific page or feature
- Who reported it and when

Use direct quotes from the transcript for anything ambiguous or subjective — "it just spins forever after I click save" is more useful than a paraphrase.

The output should be structured enough to paste straight into Linear, GitHub Issues, or whatever the team uses. Err on the side of including too much context from the call rather than too little — the engineer reading this wasn't on the call.
