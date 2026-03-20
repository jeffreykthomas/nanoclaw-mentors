# AGENTS.md - NanoClaw-Mentors Workspace

This repository is a customized `NanoClaw` fork. Use root docs only when they add something useful beyond the repo's actual runtime memory and code.

## First Run

If `BOOTSTRAP.md` exists:
1. Read it.
2. Follow it.
3. Delete it when complete.

## Session Startup

At the start of a direct session:
1. Read `SOUL.md`.
2. Read `USER.md`, if present.
3. Read `memory/YYYY-MM-DD.md` for today and yesterday, if present.
4. Read `MEMORY.md` only if it contains durable context that is not already captured better elsewhere.

Do this automatically. Missing optional files are fine.

## Canonical Project Context

When you need the repo's actual behavior, trust these first:
1. `README.md`
2. `CLAUDE.md`
3. `docs/REQUIREMENTS.md`
4. `docs/SPEC.md`
5. `groups/main/CLAUDE.md` and `groups/global/CLAUDE.md`

If a root scaffold doc conflicts with these, the repo docs and code win.

## Additive Docs Only

Root docs should be additive, not duplicative.

Good uses:
- local runbooks
- durable coding workflow notes
- temporary investigation context
- repo-specific guidance for future direct sessions

Bad uses:
- mirroring NanoClaw runtime memory already stored under `groups/`
- restating behavior already documented more accurately in code or specs
- keeping parallel sources of truth that drift

## Runtime Memory Distinction

These root files support local coding sessions.

NanoClaw's runtime memory is separate:
- shared runtime memory: `groups/global/CLAUDE.md`
- shared runtime soul: `groups/global/SOUL.md`
- per-group runtime memory: `groups/*/CLAUDE.md`
- per-group runtime experience logs: `groups/*/REFLECTIONS.md`

Do not treat root `MEMORY.md` as the product's main memory system.
Do not treat root `SOUL.md` as the live runtime soul for group chats.

## Write It Down

If something should persist, write it to the narrowest useful place.

- `memory/YYYY-MM-DD.md` for active work and short-lived findings
- `TOOLS.md` for local commands, paths, and runbooks
- `AGENTS.md` for future-session workflow guidance
- `MEMORY.md` only for durable context that is not redundant with runtime memory

## Red Lines

- Never exfiltrate private data.
- Never read `.env`, `.env.*`, or other secret-bearing local config files unless the user explicitly asks, or there is no safer way to complete a requested task.
- Never run destructive commands without explicit approval.
- Prefer recoverable operations over irreversible ones.
- Ask before external actions or third-party side effects.
- Never claim a tool succeeded when it failed.

## NanoClaw Rules

1. Respect group isolation.
   Runtime boundaries are real; do not leak context across chats.
2. Skills are the preferred extension path.
   When a request maps to a skill, read the relevant `SKILL.md` first.
3. Prefer durable fixes over brittle UI workarounds.
4. Keep the repo aligned with NanoClaw's small, understandable philosophy.
5. Stream progress on longer work instead of going silent.

## External vs Internal Actions

Safe without asking:
- read/search files
- inspect logs and configuration
- run local builds, tests, and diagnostics
- edit internal docs and code

Ask first:
- sending messages or emails
- posting to external services
- actions that leave the machine or change shared third-party state

## Heartbeats

When a heartbeat prompt arrives:
1. Read `HEARTBEAT.md`.
2. Execute only that checklist.
3. Reply `HEARTBEAT_OK` if no action is needed.

## Practical Default

Be useful, concise, and accurate.
Keep the scaffold lean and only as opinionated as it is helpful.
