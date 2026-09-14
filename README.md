<h1 align="center">ZWork</h1>
<p align="center">A desktop agent workbench for Yunxiao DevOps, built on goose</p>

<p align="center">
  <a href="../../releases/latest">Download the latest release</a> · <a href="README.zh-CN.md">简体中文</a>
</p>

ZWork is an independent distribution of [goose](https://github.com/aaif-goose/goose). It keeps the goose agent and adds a Yunxiao personal workbench, more model providers and a reworked desktop experience. This repository hosts the macOS releases, the changelog and the license notices.

## Features

- **Yunxiao workbench**: work items on a board or list, repositories with local clones, code and diffs, merge requests, pipelines and packages, with a one-click hand-off to the agent.
- **Providers**: Qoder CLI, QwenWork, Claude Code, Codex and the providers that ship with goose. New conversations switch provider and model on the chat page, and started conversations can switch models.
- **Workspace tabs**: tabs grouped by working directory that come back after a restart, with session search and status filters.
- **Command palette and quick session jump**: `⌘⇧P` or `⌘K` for commands, `⌘P` for sessions.
- **Dracula PRO themes**: Dracula Pro, Alucard, Blade, Buffy, Lincoln, Morbius, Van Helsing and Aura.
- **XiYang**: a desktop companion that follows your conversations.
- **Desktop control**: drive the running app from the `zwork desktop` CLI or the `zwork-desktop` skill.
- **Updates**: ZWork checks this repository for new releases, downloads them in the background and installs them when you choose Restart to Update in Settings > App.

## Install

1. Download `ZWork-<version>-arm64.dmg` from the [latest release](../../releases/latest).
2. Open the DMG and drag ZWork to Applications.

The app is signed with a Developer ID certificate and notarized by Apple. This release requires an Apple Silicon Mac running macOS 12 or later.

ZWork 1.52.0 and later update from Settings. If you run 1.51.0, install the latest release manually once.

To verify the download, place the `.sha256` file next to the DMG and run:

```bash
shasum -a 256 -c --ignore-missing ZWork-<version>-arm64.sha256
```

## Before you start

- **Workbench**: open Settings, then Workbench, and enter the Yunxiao API base URL and a personal access token.
- **Qoder CLI, Claude Code and Codex**: install and sign in to the matching CLI on this Mac.
- **QwenWork**: install and sign in to the QwenWorkCN desktop app. The first QwenWork session downloads a Node.js runtime through Hermit, which takes a minute or two and needs access to GitHub.

## Feedback

Please report problems and ideas in [Issues](../../issues).

## License

ZWork is a modified version of goose and is distributed under the Apache License 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
