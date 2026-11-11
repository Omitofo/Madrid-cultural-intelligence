# Instructions for LLMs working in this repository

## Mission

Help the user discover interesting public activities in Madrid by maintaining a small, useful reference list of entities and collecting current findings from their official channels.

This repository is a **working context and research workspace**. It is not expected to contain every institution, every event, or a complete copy of external websites.

## The five areas

- `01_system/`: how this workspace works.
- `02_entities/`: the entities worth checking and the practical information needed to revisit them.
- `03_findings/`: sourced research collected during checks, especially event listings and changes to entity information.
- `04_ai_outputs/`: curated answers and reports made from findings.
- `05_working_notes/`: leads, questions and unfinished work.

Do not mix these concerns. An entity record describes a source to monitor; a finding records what was discovered at a particular time; an AI output is a curated response for a particular request.

## Before starting a task

1. Read this file and `01_system/data_standards.md`.
2. Inspect the relevant entity records and recent findings.
3. Understand the requested scope and date range.
4. Identify what needs fresh verification.

Do not ask the user to repeat information already present in the repository.

## Entity records

Create or update a record when the user asks to add an entity, investigate a new source, or maintain the list of sources.

An entity can be an institution, foundation, association, university, cultural centre, venue, event organizer, newsletter, events directory or other useful discovery source.

Use `02_entities/TEMPLATE.md` as the starting point. Store records in the most suitable subfolder:

- `institutions/`
- `organizations/`
- `venues/`
- `discovery_sources/`

If an entity fits more than one type, choose one primary location and mention its other roles in the record. Avoid duplicate records.

Keep entity records concise and operational. Prioritize:
- what the entity is and why it may be relevant;
- location and official website;
- official calendar/programme page;
- subjects and event formats;
- how to register or attend;
- whether activities are free, paid or mixed, if verified;
- what to check when revisiting;
- sources and last verification date.

Do not try to copy the entity's entire website or maintain a full institutional encyclopedia.

## Checking schedules and collecting events

When asked to check entities, update their schedules, or find events for a period:

1. Use the entity records as a checklist and starting context.
2. Visit the official calendar or event page for each relevant entity.
3. Search the requested date range. Check additional official channels only when useful (for example, an official newsletter or ticketing page).
4. Record event details only when supported by a source.
5. Verify the event date, start time, venue, price and registration requirements from the event's own page where possible.
6. Distinguish confirmed information from tentative or incomplete announcements.
7. Save useful results in `03_findings/events/`. For a batch check, also create or update a dated check note in `03_findings/schedule_checks/`.
8. Update an entity's `Last checked` field when its schedule was actually reviewed.

A search result snippet or an old agenda is not enough to confirm a current event. If a page is unavailable or information cannot be verified, say so and record the limitation. Do not interpret missing information as evidence that no events exist.

Do not claim that an event is free unless the event page or an authoritative access page supports that claim. Distinguish free admission, free registration, invitation-only access, ticket lotteries and paid admission.

## Findings versus outputs

- `03_findings/` is the evidence-oriented record of what was found. Keep event entries factual, sourced and reusable.
- `04_ai_outputs/` is where curated agendas, recommendations, comparisons and research reports go. These can select and interpret findings, but should link back to them and to original sources.

Do not save every conversational answer. Save outputs when they are useful as a durable reference, when the user asks, or when they represent a meaningful research deliverable.

Preserve dated outputs rather than silently replacing old reports. If correcting a report, make the correction clear or create a new dated version.

## Discovering new entities

When asked to find more places or organizations:

1. Search beyond the current list; the repository is a starting point, not a boundary.
2. Prefer entities with a recurring public programme or a useful event-discovery channel.
3. Check whether the entity already exists before adding it.
4. Create a concise entity record when there is enough evidence that it is worth following.
5. Put promising but insufficiently researched leads in `05_working_notes/research_backlog.md`.

## Using findings to answer the user

For weekly/monthly agendas:
- use the requested local date range in Madrid;
- prioritize relevance, quality, practical accessibility and free/affordable entry;
- include date, time, venue, price/access, registration and direct event URL;
- group events by date or theme when useful;
- explain briefly why an event may be interesting;
- identify missing or unverified details;
- link each event to its finding and organizing entity where possible.

Do not rank events as objectively "best" without explaining the criteria. Do not invent availability, ticket status or event details.

## External actions

The repository itself does not book, register, email or create calendar events.

If the user asks to use connected tools (for example, Gmail or Google Calendar), first produce or identify the verified event shortlist, then use the relevant connected tool and follow its permission and confirmation requirements. Never imply that an event was added, booked or emailed unless the tool confirms success.

## Editing discipline

- Keep the folder structure shallow.
- Prefer Markdown and ordinary links.
- Avoid adding dependencies, databases, scripts or elaborate schemas unless the user explicitly asks or scale clearly requires them.
- Do not delete useful historical findings or outputs.
- Avoid duplicating the same event or entity.
- Make focused edits; do not rewrite unrelated records.
- When uncertain, preserve the uncertainty and add an open item.
