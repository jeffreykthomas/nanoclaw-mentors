# TOOLS.md - NanoClaw Workspace Notes

Keep practical local runbooks and non-secret repo notes here.

Only add entries that are genuinely useful and not already documented better elsewhere.

## Core Commands
- `npm run dev` - run NanoClaw with hot reload
- `npm run build` - compile TypeScript
- `./container/build.sh` - rebuild the agent container image

## Service Management
- macOS:
  `launchctl load ~/Library/LaunchAgents/com.nanoclaw.plist`
  `launchctl unload ~/Library/LaunchAgents/com.nanoclaw.plist`
  `launchctl kickstart -k gui/$(id -u)/com.nanoclaw`
- Linux:
  `systemctl --user start nanoclaw`
  `systemctl --user stop nanoclaw`
  `systemctl --user restart nanoclaw`

## Important Paths
- `src/index.ts` - orchestrator and main loop
- `src/ipc.ts` - IPC watcher and task processing
- `src/container-runner.ts` - container execution
- `src/config.ts` - core runtime configuration
- `store/messages.db` - SQLite state
- `groups/global/CLAUDE.md` - shared runtime memory
- `groups/main/CLAUDE.md` - main/admin runtime instructions

## Working Notes
- Prefer skills for adding channels or major capabilities.
- Favor code changes over config sprawl.
- Check docs and code together before copying patterns from another repo.
