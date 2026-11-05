# PersonalAgent

A personal AI Chief of Staff built on Claude: one agent that knows you, instead of ten apps that don't.

Based on the framework in Sandeep Swadia's [This ONE AI Agent Will Make You So Productive It's Almost Unfair](https://www.youtube.com/watch?v=x9hrptrGGY0) (Nov 4, 2026). The agent has one mode for each of the four forces that drain productivity:

| Force | Mode | Call it with | What it does |
| --- | --- | --- | --- |
| Fragments | Glue | "cos, find or do X" | Routes to Drive, calendar, reminders or memory and acts |
| Flood | Gatekeeper | "triage" / morning brief | Sorts inbound into Act now, Decide, Read later, Ignore |
| Frequency | Trigger | "what's due" / weekly run | Checks the ledger, nudges early, preps the paperwork |
| Future | Compass | "weekly review" | Weighs time and requests against your purpose |

## Repo layout

| Path | What it is |
| --- | --- |
| `skills/chief-of-staff/SKILL.md` | The agent, as a Claude skill |
| `context/purpose.md` | Purpose, quarterly priorities, side projects (fill in the brackets) |
| `context/recurring-ledger.md` | Recurring obligations the Trigger mode tracks |
| `docs/concepts.md` | The concepts from the video, with the agent design |
| `deck/` | Source of the "Your AI Chief of Staff" slide deck (Claude Slides format: `deck.json` + one HTML file per slide) |

## Setup

1. Install the skill: save it from Claude, or copy `skills/chief-of-staff/` into your skills folder (`~/.claude/skills/` for Claude Code).
2. Fill in `context/purpose.md`. In claude.ai the agent reads `claude/purpose.md` and `claude/recurring-ledger.md` from the PersonalAgent project; keep those in sync with this repo.
3. Connect personal Gmail so the gatekeeper has an inbox to triage.
4. Turn on the weekday morning brief and weekly review as scheduled tasks.

## Guardrail

Personal use only. No JPMorgan systems, work email or firm data go into this agent or this repo.
