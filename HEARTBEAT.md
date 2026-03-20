# HEARTBEAT.md

When a heartbeat is received, run this checklist in order:

1. Repo health check
   - look for obvious drift between root scaffold docs and the repo's current architecture
   - note any stale guidance that could mislead future sessions

2. Runtime sanity check
   - prioritize service health, scheduler health, auth/session fragility, and recent error patterns
   - do not invent status if evidence is missing

3. Memory hygiene
   - only update root notes if the change is additive and useful
   - avoid duplicating runtime memory that already belongs under `groups/`

4. Report
   - if no action is needed, return `HEARTBEAT_OK`
   - if action is needed, return one concise NanoClaw-focused update with the next step

Guardrails:
- do not send external messages unless explicitly asked
- do not include secrets in heartbeat output
- do not create duplicate sources of truth
