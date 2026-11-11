# Madrid Cultural Intelligence

A lightweight, LLM-friendly workspace for discovering institutions, checking their programmes, collecting event findings, and producing useful agendas and research notes.

## What this repository is

This is a **working place for research**, not a complete events platform or an automated event scraper.

The intended workflow is:

1. Keep a small, useful record of institutions, organizations, venues and other sources worth following.
2. Ask an LLM to revisit those sources and check their current schedules.
3. Save the verified findings (especially upcoming events) in this repository.
4. Ask the LLM to make weekly/monthly lists or other useful summaries from those findings.
5. Optionally use connected tools such as Gmail or Google Calendar to act on the selected events.

The repository provides persistent context. The LLM still needs to visit official websites for current schedules and verify time-sensitive details.

## Repository map

| Path | Purpose |
|---|---|
| `01_system/` | Project purpose, agent instructions and working conventions |
| `02_entities/` | Basic records for places and organizations worth checking |
| `03_findings/` | Research gathered from those entities: events, schedule checks and discoveries |
| `04_ai_outputs/` | Curated agendas, answers and reports generated from research |
| `05_working_notes/` | Backlog, open questions and ideas |

## Start here

1. Read `01_system/AGENTS.md`.
2. Browse `02_entities/` to see which sources are already known.
3. For current events, check official calendars directly; do not assume old findings are current.
4. Save sourced event details in `03_findings/events/`.
5. Save a curated answer or agenda in `04_ai_outputs/` when useful.

## Scope

Initial focus: Madrid, Spain.

Relevant activities include public lectures, conferences, debates, science communication, philosophy, history, literature, technology, exhibitions, cinema, music, workshops and other intellectually or culturally interesting activities.

Prefer free or affordable activities, but do not exclude paid events when they are particularly relevant. Record the actual price and access conditions rather than assuming all events from an entity are free.

## Important limitation

The initial entity records are **research starting points**, not claims that every detail has been freshly verified. Each record indicates what is known, what needs checking and where to look. Always verify current event dates, times, prices, registration and availability on the official event page.

## Naming conventions

- Entity files: `lowercase-hyphenated-name.md`
- Event findings: `YYYY-MM-DD-short-event-name.md` (use the event date when known)
- Weekly outputs: `YYYY-MM-DD_weekly-agenda.md`
- Monthly outputs: `YYYY-MM_monthly-agenda.md`
- Use ISO dates (`YYYY-MM-DD`) and include source URLs.
