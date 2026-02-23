# Codraft

> AI-powered development environment with multi-terminal support, Monaco editor, Git integration, and autonomous AI agents.

## Download

| Platform | File |
|----------|------|
| macOS (Apple Silicon) | `Codraft-x.x.x-arm64.dmg` |
| Windows | `Codraft-x.x.x-Setup.exe` |

Download the latest release from the [Releases](../../releases) page.

## Install via Homebrew

```bash
brew install --cask mehmetsagir/tap/codraft
```

## Features

- **AI Chat** — Conversational coding assistant with file context auto-detection and image attachments
- **Agent Mode** — Autonomous coding agent that reads/writes files and runs commands
- **AI Commit** — Group changes into logical conventional commits automatically
- **Multi-Terminal** — Multiple PTY terminals with split pane support
- **Monaco Editor** — VS Code-grade editor with syntax highlighting and LSP
- **Git Integration** — Full SourceTree-style UI (branches, history, stash, blame, cherry-pick, worktrees)
- **Task Board** — Kanban board with AI pipeline integration
- **GitHub PRs** — PR management, review, and merge inside the app
- **Project Search** — Project-wide search and replace

## Changelog

<!-- CHANGELOG_START -->
### v0.0.19 — 2026-02-23

- chore(package): bump version to 0.0.19
- feat(agent): enhance quota error handling
- fix(useBoard): exclude done and personal-review from taskCount
- feat(agent): add review model retry logic
- style(renderer): add CSS for model badges
- feat(renderer): enhance board with model display
- feat(main): add model caching and sorting
- refactor(agent): use git add -A and exclude node_modules
- style(ui): adjust components.css
- feat(theme): add ThemeContext
- style(theme): update midnight theme colors
- feat(agent): add shared clone path support
- style: minor formatting and whitespace adjustments
- feat(types): add free flag to model types
- feat(ui): add CLI installation warnings and options
- fix(ai): improve error handling in API calls
- feat(agent): add child process management to cleanup
- feat(hooks): enhance useAgentModels for models.dev
- feat(ui): update SettingsPage for models.dev
- feat(ipc): update preload and IPC for models.dev
- feat(models): add models.dev cache handling
- fix(pipeline): handle PM agent configuration
- fix(board): remove unnecessary log type
- refactor(agent): use worktree for merge operations
- style(ui): remove unused agent count styles

### v0.0.18 — 2026-02-22

- chore(release): bump version to 0.0.18
- feat(themes): add Monokai theme
- feat(renderer): add dracula theme
- docs(themes): add dracula theme
- feat(board): improve crash recovery and task management
- style(ui): update markdown editor and pipeline detail styles
- feat(board): add multi-agent task orchestration
- feat(themes): add nord theme and update color themes
- refactor(ui): enhance AppPullRequestsView rendering
- feat(ui): display open PR count in sidebar
- feat(renderer): add image file preview support
- chore(build): update application icon
- feat(board): add AI-enhanced description and advanced settings
- chore(workflow): update repo URL in release script
- refactor(ui): update settings page and styles
- fix(updater): disable auto download

### v0.0.17 — 2026-02-20

- chore(release): bump version to 0.0.17
- refactor(settings): update banners and styles
- feat(ai): remove AI code review feature

### v0.0.16 — 2026-02-20

- chore(package): bump version to 0.0.16
- fix(releases): check for README existence

<!-- CHANGELOG_END -->
