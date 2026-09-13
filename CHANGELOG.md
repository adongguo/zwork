# 更新日志

## 1.51.0 - 2026-09-13

ZWork 首个正式版，基于 goose 1.50.0，macOS 版支持 Apple Silicon。

### 新增

- 云效个人工作台：工作项看板与列表、代码库与本地克隆、代码与差异、合并请求、流水线和制品库。各模块可以在设置里关闭，工作项和合并请求可以直接交给 Agent 处理。
- Qoder CLI 与千问办公 Provider。千问办公通过内置 sidecar 复用 QwenWorkCN 桌面端的登录态。
- 新对话可以在对话页直接切换 Provider 和模型，只列出本机可用的 Provider，对话开始后锁定。
- 按工作目录分组的 workspace 标签，重启后自动恢复；侧栏支持会话搜索和状态筛选。
- 命令面板和会话快速跳转，快捷键可以自定义。
- Dracula PRO 主题：Dracula Pro、Alucard、Blade、Buffy、Lincoln、Morbius、Van Helsing，以及 Aura。
- 桌面伙伴 XiYang：跟随对话状态，支持视线跟随、单击、双击、长按和拖拽互动，空闲时会打盹。
- 通过 `zwork desktop` 命令行和 `zwork-desktop` skill 操作正在运行的应用。
- 合并请求参与人和工作项负责人显示 Codeup 头像，工作项卡片按阶段、类型和优先级着色。

### 变更

- 采用 ZWork 品牌、图标和字体，默认语言为英文。
- 更新源、遥测、文档站等上游在线服务改为按需开启，默认关闭。

### 修复

- 暗色主题下设置开关看不清。
