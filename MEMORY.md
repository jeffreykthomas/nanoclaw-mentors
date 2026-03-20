# MEMORY.md - Long-Term Memory

Curated, durable memory for direct development sessions in this repo.

## User
- Name: Jeffrey

## Workspace Context
- This repo is a customized `NanoClaw` fork.
- Root scaffold docs should stay aligned with the repo's real architecture and philosophy.
- Runtime/group memory lives under `groups/`, not in root `MEMORY.md`.

## Stable Preferences
- Prefers concise, practical answers.
- Values consistency between docs, code, and actual behavior.
- Favors building on an agent scaffold, but wants it adapted to the repo rather than copied blindly.

## Current Priorities
- Keep the root agent scaffold useful for local coding sessions.
- Preserve NanoClaw's small, understandable architecture.
- Avoid introducing guidance that conflicts with runtime behavior.

## Known Lessons
- Copied scaffolds can be structurally fine but semantically wrong for the target repo.
- For NanoClaw questions, trust `README.md`, `CLAUDE.md`, `docs/REQUIREMENTS.md`, and `docs/SPEC.md` over generic workspace docs.

## Update Policy
- Keep this file concise and high-signal.
- Put short-lived work in `memory/YYYY-MM-DD.md`.
- Do not store secrets here.
