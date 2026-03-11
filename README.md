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
### v0.0.36 — 2026-03-11

- chore(release): bump version to 0.0.36
- refactor(ui): remove unused form setting
- refactor(agent-core): enhance review output parsing
- refactor(agent-core): unify personal review transition
- feat(board): enforce personal review in pipeline
- feat(reviewStage): implement personal review escalation
- feat(reviewEngine): add markdown stripping and verdict index finding
- refactor(settings): improve multi-agent handling
- chore(board): remove unused useBoardDrawerAnimation hook
- refactor(pipeline): improve modularity of pipeline hooks
- fix(board): reset PlanTab on task change
- feat(board): enhance ChangesTab and LogsTab
- test(board): add tests for boardViewUtils and logPresentation
- feat(board): add terminal actions set to boardCardUtils
- fix(board): handle task deletion errors in BoardView
- refactor(board): integrate BoardClearConfirmModal in BoardColumn
- feat(board): improve BoardClearConfirmModal accessibility
- feat(board): enhance board card components
- feat(board): add in-memory board cache
- chore(hooks): remove unused BoardCardStatus hook
- chore(styles): remove deprecated kanban board styles
- style(board): use CSS variables for colors
- refactor(pipeline): enhance hooks with updating refs
- refactor(board): add stable callbacks for plan approval
- refactor(board): remove redundant keydown handler

### v0.0.35 — 2026-03-09

- chore(package): bump version to 0.0.35
- feat(terminal): stable viewport and resize improvements
- style(ui): update styles for settings update

### v0.0.34 — 2026-03-09

- chore(package): bump version to 0.0.34
- docs(editor): update IntelliSense features
- feat(language-features): add new LSP providers
- docs(editor): update IntelliSense and RN support
- feat(editor): update Monaco config for TS/JS
- feat(lsp): add TypeScript LSP support
- feat(ui): add aria attributes to chat panel
- refactor(handlers): enhance file selection and settings handlers
- style(file-history): update overlay and modal styles
- feat(file-panel): remove refresh button
- feat(app): add lazy loading for file history view
- feat(landing): enhance page with new components
- style(ui): add new page orb styles
- docs(codraft): add comprehensive feature documentation
- style(css): remove unused file panel tree row styles
- feat(ui): enhance TabBar with pinned tab affordance
- feat(state): add filePanelWidth to global state
- style(landing): update landing page and hero visual
- style(ui): update component and terminal styles
- fix(filesystem): ignore internal project memory
- feat(shell): add shell operations
- feat(file-panel): enhance file panel features
- feat(editor): add editor tab management
- feat(board-types): add task spec and implementation plan
- docs(board): update documentation with new features

### v0.0.33 — 2026-03-04

- chore(release): bump version to 0.0.33
- feat(ui): add caching for usage limits
- style(ui): update create-task-modal styles
- refactor(board): adjust task title input section
- feat(board): add settings prop to modals
- style(ui): update branch selector styles
- feat(menu): implement menu actions and IPC communication
- feat(pipeline): add live file change tracking
- fix(types): make kind property in AgentPreset non-optional
- refactor(utils): remove unused functions in modelCatalog
- style(css): remove unused models panel styles
- refactor(hooks): simplify useAgentModels return values
- refactor(settings): remove unused prop and update model handling
- feat(settings): update ai provider settings
- refactor(model-parsing): use parseModelRef
- feat(ai-providers): add codex support
- refactor(ai-models): remove openai model fetching
- style(ui): add styles for settings models hero
- fix(ui): correct chat and feature model assignment
- feat(board): add agent preset support to task forms
- feat(ai): add model catalog and agent presets
- fix(agent): update GLM model argument handling

### v0.0.32 — 2026-03-03

- chore(package): bump version to 0.0.32
- feat(build): add beforePack script for file existence checks

### v0.0.30 — 2026-03-03

- chore(release): bump version to 0.0.30
- style(index): improve comment clarity for page reload prevention
- feat(index): add error logging for console messages and load failures
- refactor(index): remove DevTools shortcut handling

### v0.0.29 — 2026-03-03

- chore(release): bump version to 0.0.29
- feat(desktop): enhance error logging

### v0.0.28 — 2026-03-02

- chore(package): bump version to 0.0.28

### v0.0.27 — 2026-03-02

- chore(release): bump version to 0.0.27
- fix(build): remove committed tsbuildinfo files to fix CI build failures

### v0.0.24 — 2026-02-25

- chore(package): bump version to 0.0.24
- style(ui): add styles for CLI installation UI
- feat(cli): add CLI integration for opening projects

### v0.0.22 — 2026-02-25

- chore(package): bump version to 0.0.22
- chore(config): exclude test files in tsconfig

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
