<h1 align="center">ZWork</h1>
<p align="center">基于 goose 的云效桌面 Agent 工作台</p>

<p align="center">
  <a href="../../releases/latest">下载最新版本</a> · <a href="README.md">English</a>
</p>

ZWork 是 [goose](https://github.com/aaif-goose/goose) 的独立发行版。它保留了 goose 的 Agent 能力，新增云效个人工作台、更多模型 Provider，并重做了桌面端体验。本仓库发布 macOS 安装包、更新日志和许可声明。

## 功能

- **云效工作台**：工作项看板与列表、代码库与本地克隆、代码与差异、合并请求、流水线和制品库，可以一键交给 Agent 处理。
- **Provider**：Qoder CLI、千问办公、Claude Code、Codex，以及 goose 自带的各类 Provider。新对话可以在对话页直接切换 Provider 和模型，已开始的对话也可以切换模型。
- **workspace 标签**：按工作目录分组，重启后自动恢复，支持会话搜索和状态筛选。
- **命令面板与会话跳转**：`⌘⇧P` 或 `⌘K` 打开命令面板，`⌘P` 跳转会话。
- **Dracula PRO 主题**：Dracula Pro、Alucard、Blade、Buffy、Lincoln、Morbius、Van Helsing 和 Aura。
- **XiYang**：跟随对话状态的桌面伙伴。
- **桌面控制**：用 `zwork desktop` 命令行或 `zwork-desktop` skill 操作正在运行的应用。
- **自动更新**：ZWork 从本仓库检查新版本，在后台下载，并在设置 → App 点击“重启以更新”后完成安装。

## 安装

1. 从[最新版本](../../releases/latest)下载 `ZWork-<版本>-arm64.dmg`。
2. 打开 DMG，把 ZWork 拖到“应用程序”。

安装包已使用 Developer ID 签名并经过 Apple 公证。本版本需要 Apple Silicon Mac，系统为 macOS 12 或更高版本。

1.52.0 及以后的版本可以在设置里更新；正在使用 1.51.0 的话，需要手动安装一次最新版本。

校验下载文件：把 `.sha256` 文件放在 DMG 旁边，然后执行：

```bash
shasum -a 256 -c --ignore-missing ZWork-<版本>-arm64.sha256
```

## 使用前准备

- **云效工作台**：打开设置 → Workbench，填写云效 API 地址和个人访问令牌。
- **Qoder CLI、Claude Code、Codex**：在本机安装并登录对应的 CLI。
- **千问办公**：安装并登录 QwenWorkCN 桌面端。第一次使用时，应用会通过 Hermit 自动下载 Node.js 运行环境，大约需要一两分钟，并且要能访问 GitHub。

## 反馈

问题和建议请提交到 [Issues](../../issues)。

## 许可

ZWork 是 goose 的修改版，基于 Apache License 2.0 发布，详见 [LICENSE](LICENSE) 和 [NOTICE](NOTICE)。
