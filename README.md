# Granola

Your meetings in your workflow.

Granola gives Cursor's agent access to what your team discussed, decided, and committed to in meetings. Instead of context-switching to check your notes or asking teammates to repeat themselves, you get answers where you're already working.

## Setup

Install the plugin from the Cursor Marketplace. The first time you use a Granola tool, you'll be prompted to sign in via your browser. You need a [Granola](https://granola.ai) account with meeting data.

## What's included

### Skills

Skills are loaded autonomously — the agent decides when to use them based on what you're doing. You don't need to invoke them.

**granola-context** — Look up what was discussed or decided. The agent pulls this in when you're mid-work and a question touches on something from a meeting.

**granola-review** — Check your work against meeting decisions before submitting. The agent uses this to flag what's aligned, what's missing, and what you've added that wasn't discussed.

**granola-prep** — Prepare for an upcoming meeting. The agent pulls context from previous meetings with the same people or on the same topic.

### Commands

Commands are invoked manually with `/` and produce a document you keep — a spec, a plan, a report.

**`/granola-plan`** — Generate a prioritized build plan from recent meeting decisions and action items. Good for starting a work session.

**`/granola-spec`** — Build a structured spec from meeting discussions. Requirements, constraints, decisions, open questions — all traced to specific meetings.

**`/granola-brief`** — Get a briefing on any topic by synthesizing everything discussed across your meetings. Useful for onboarding, getting oriented, or preparing for a conversation.

**`/granola-bug-report`** — Turn a bug walkthrough call into a structured bug report, ready to drop into Linear or GitHub Issues.

**`/granola-pr`** — Write a PR description grounded in meeting decisions. Links your changes back to the discussions where the work was agreed on, and flags anything you've built that wasn't explicitly discussed.

**`/granola-gaps`** — Find what was discussed in meetings but hasn't shown up in code yet. Cross-references meeting decisions and action items against your git history to surface what's been done, what hasn't started, and what's only partially covered.

### Agent

**`/granola-engineer`** — A decisions-aware assistant that anchors implementation choices to meeting context. It cites meetings when justifying decisions, flags when you're building something that wasn't discussed, and surfaces contradictions between meetings.

### Rule

The plugin includes an always-on rule that nudges the agent to check Granola for meeting context when you're implementing features or making decisions — without you having to ask.

## Granola MCP tools

The plugin connects to Granola's MCP server. These are the tools available to the agent:

- `query_granola_meetings` — semantic search across your meetings
- `list_meetings` — browse meetings by date range or folder
- `list_meeting_folders` — discover folder IDs, titles, descriptions, and note counts
- `get_meetings` — retrieve detailed meeting info by ID (notes, summaries, attendees, metadata)
- `get_meeting_transcript` — full transcript with speakers and timestamps

## Feedback

We'd love to hear how you're using this. Reach out at hello@granola.ai or on [Twitter/X](https://x.com/granaborable).
