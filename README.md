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
### v0.0.50 — 2026-03-29

- chore(release): bump version to 0.0.50
- style(ui): update styles for AI chat and scripts
- chore(state): add debugging and improve persistence
- refactor(ai-chat): update components for model handling
- feat(ai): enhance provider configuration and APIs
- feat(ai): add chat tool loop and tool execution
- fix(terminal): conditionally update terminal actions
- feat(terminal): improve terminal transfer and connection
- feat(terminal): add transfer and attach functionality
- style(ui): update header styles for draggable project
- feat(desktop): add cross-window project transfer
- feat(ui): revamp welcome screen layout and styles
- feat(window): identify fresh new windows
- refactor(ui): use flexible grid and flexbox for settings
- chore: AI chat checkpoint
- style(layout): remove unused status bar model styles
- refactor(status-bar): remove unused currentView prop
- refactor(ui): remove AI model indicators from StatusBar
- style(ui): update modal width and button whitespace
- refactor(git): simplify commit amendments logic
- style(git): enhance CSS for git components
- feat(desktop): remove dashboard feature
- refactor(ui): reorder pull requests button in sidebar
- chore(shortcuts): update default shortcuts
- feat(ui): improve persistent state handling

### v0.0.49 — 2026-03-26

- chore(release): bump version to 0.0.49
- docs(ui): update layout and page metadata
- style(ui): revamp global styles
- style(ui): update HeroVisual component styles
- refactor(ui): improve animation logic in AnimateIn
- feat(desktop): add clipboard image handling
- refactor(ai-chat): remove restore confirmation dialog
- feat(ai-chat): handle restored content after truncation
- chore: AI chat checkpoint
- feat(ai-chat): handle message truncation for checkpoints
- feat(git): add auto-commit checkpoint for AI chat
- feat(ipc): add stashCreate channel
- feat(ai-chat): add message truncation to checkpoint
- feat(ai-chat): add context chip display to input bar
- feat(ai-chat): add git checkpoint restore functionality
- feat(ai-chat): enhance UI and functionality
- feat(ai): add streaming support for AI chat
- refactor(ai-chat): simplify TypewriterBubble logic
- refactor(ai-chat): remove working indicator
- refactor(ai-chat): simplify AgentLogs component
- fix(app): refine slash command detection
- fix(ai-chat): improve markdown handling
- style(ai-chat): update diff block styles

### v0.0.48 — 2026-03-24

- chore(package): bump version to 0.0.48
- style(ai-chat): adjust CSS styles
- feat(ai-chat): add image resizing for attachments
- fix(ai-chat): escape HTML in markdown
- style(ai-chat): update placeholder text
- feat(ai-chat): add resend message and error boundary

### v0.0.47 — 2026-03-24

- chore(package): bump version to 0.0.47
- style(ui): add CSS for left-positioned file panel
- feat(ui): add file panel position setting

### v0.0.45 — 2026-03-24

- chore: update version

### v0.0.44 — 2026-03-24

- chore(release): bump version to 0.0.44
- feat(ui): sort files by directory depth in QuickOpen

### v0.0.43 — 2026-03-24

- chore(package): bump version to 0.0.43
- test(board): update task payload creation test
- style(ui): adjust CSS for select container in settings
- fix(mobile): update default AI chat model
- test(ai): update tests for model selection and routing
- refactor(ai): replace models.dev with static registry
- chore(settings): remove .codraft from default ignored
- docs(settings): update ignored paths description
- feat(board): filter file changes in board components
- feat(main): add built-in ignored entries
- refactor(logs): remove useIncrementalList from logs tab
- style(ui): update sidebar icon for scripts
- feat(settings): update default ignored entries
- feat(board): add incremental list loading
- feat(board): limit files in DescriptionEditor
- refactor(terminal): improve reconnection logic
- style(ui): add custom select container styles
- refactor(terminal): improve key event handling
- docs(memory): update theme system and decisions documentation
- fix(chat-api): improve provider to agent type mapping
- fix(project-runner): correct bun lockfile detection
- feat(process-manager): add process manager feature
- fix(agent-pipeline): improve session memory handling
- feat(ai-chat): improve agent-powered chat experience
- fix(agent-pipeline): improve session memory handling

### v0.0.42 — 2026-03-14

- chore(release): bump version to 0.0.42
- feat(ui): handle async approve in board card
- feat(pipeline): add taskId support to reapply
- fix(terminal): use onMouseDownCapture for activation
- feat(ui): add rate limits update listener
- feat(ai): add rate limits polling
- feat(ui): integrate create project feature
- feat(filesystem): add create project folder functionality
- docs(decisions): update decisions documentation
- docs(memory): update terminal and chat context documentation
- feat(terminal): improve performance with buffering and throttling

### v0.0.41 — 2026-03-13

- chore(release): bump version to 0.0.41
- feat(pipeline): include resumeDiff in task status
- feat(pipeline): add projectPath support in approval
- style(ui): add flex styling to tab panels

### v0.0.40 — 2026-03-12

- chore(release): bump version to 0.0.40
- feat(desktop): add clone repository feature
- refactor(hooks): use const for currentTask
- style(comments): distinguish user and agent comments
- style(board): add loading skeleton styles
- fix(subtasks): add error handling for subtask approval
- fix(pipeline): improve cleanup error logging
- fix(board): enhance task reset and error handling
- fix(logs): fix log presentation key stability
- feat(overview): improve comments rendering
- refactor(logs): optimize log entries merging
- feat(board): add loading state and clear confirmation
- feat(board): enhance caching and shutdown handling
- refactor(hooks): optimize task selection in useBoard
- refactor(ui): improve multi-agent plan task handling
- feat(board): add rolling backups on save
- refactor(runtime): optimize emission and status handling
- feat(ui): lazy keep-alive for tabs
- fix(hooks): enhance error handling in usePipelineSubtasks
- fix(hooks): enhance error handling in usePipelineApproval
- fix(hooks): correct log count reference in usePipeline
- fix(hooks): improve task reset and creation in useBoard
- fix(ui): improve log handling in LogsTab
- fix(ui): improve file loading logic in ChangesTab
- feat(ui): prevent duplicate approvals in SubtaskPlanModal

### v0.0.39 — 2026-03-12

- chore(release): bump version to 0.0.39
- feat(editor): configure monaco workers
- feat(lsp): enhance Vue LSP setup
- feat(editor): improve monaco config and library loading
- feat(editor): enhance language support and remove CDN config
- feat(lsp): add configuration and capability handling
- feat(agent-core): support image paths in pipeline
- refactor(terminal): improve drag and drop handling
- feat(ai-chat): add drag and drop image support
- refactor(ui): update settings update downloading styles

### v0.0.38 — 2026-03-11

- chore(release): bump version to 0.0.38
- feat(terminal): handle buffer change for screen resizing
- refactor(ui): remove project runner functionality
- feat(state): improve terminal panes state saving
- feat(terminal): optimize git status polling
- refactor(terminal): use ResizeObserver for resize handling
- feat(terminal): enhance drag-and-drop support

### v0.0.37 — 2026-03-11

- chore(release): bump version to 0.0.37
- feat(shortcuts): update terminal navigation keys
- fix(terminal): improve resizing and navigation

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
