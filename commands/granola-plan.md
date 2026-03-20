---
name: granola-plan
description: Generate a prioritized build plan from recent meeting decisions and action items.
---

# granola-plan

The person just sat down to work and wants to know what to focus on. They've had meetings — planning sessions, reviews, standups — and the decisions and action items from those meetings should drive what they build next.

Use `query_granola_meetings` to find action items and decisions from the last one to two weeks. Look for things assigned to the user or relevant to the current project. Use `list_meetings` to scan recent meetings if the semantic search needs broadening.

Cross-reference with the current state of the project — what files exist, what's been committed recently, what looks in progress. Some action items may already be done.

Produce a build plan: what to work on, in what order, and why (linked to specific meetings). Flag anything that's blocked or needs a conversation before starting. If there are competing priorities from different meetings, surface that — don't silently pick one.

The output should be something they can work from for the day or the week. Save it as a markdown file in the project if they want to keep it.
