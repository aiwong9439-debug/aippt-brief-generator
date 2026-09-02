# 更新记录

本项目的重要变化记录在此。版本号采用 `MAJOR.MINOR.PATCH` 形式。

## [0.2.0] - 2026-09-02

### Added

- 增加“快速对话生成 / 可视化工作台”双模式入口。
- 增加线上 AiPPT Brief 可视化工作台，可选择视觉风格、叙事结构和三色色盘。
- 为 RED Skill、GitHub 工作台与 AiPPT 跳转增加独立渠道参数。
- 增加 Codex 等具备浏览器能力环境中的直接打开体验。

### Changed

- 用户未提供明确主题时先选择使用模式，不再立即进入长问卷。
- 用户已经说明主题和目标时直接生成 Brief，不额外增加入口步骤。
- 明确不同 Agent 的网页打开差异：可能直接打开，也可能显示可点击链接。

### Compatibility

- Skill 名称、目录结构与输出契约保持不变，可从 `v0.1.0` 直接升级。
- 纯对话模式保持可用；不支持浏览器的 Agent 仍可正常生成 Brief。

## [0.1.0] - 2026-09-02

首个公开版本。

### Added

- 将模糊演示需求整理为结构化 AiPPT Brief 的核心工作流。
- 演示目标、受众、使用场景与页数策略的提取和确认。
- 30 种设计趋势方向，以及商务极简、科技未来、高级杂志和教育清晰等专业常用风格。
- 30 种叙事结构，覆盖决策提案、汇报复盘、产品用户、教学解释和故事表达。
- 主色、辅助色、点缀色三色配色控制。
- 逐页大纲、结论式标题、视觉形式与演讲提示输出。
- 缺失事实标记、禁止编造和逻辑一致性检查。
- Codex、Claude Code、OpenClaw 与小红书 RED Skill 的安装及发布说明。
- 完整的品牌增长策略 Brief 示例。

### Compatibility

- Skill 名称：`aippt-brief-generator`
- 入口文件：`aippt-brief-generator/SKILL.md`
- 核心输出顺序：策略判断 → Brief 代码块 → 关键假设 → AiPPT 入口

[0.2.0]: https://github.com/aiwong9439-debug/aippt-brief-generator/releases/tag/v0.2.0
[0.1.0]: https://github.com/aiwong9439-debug/aippt-brief-generator/releases/tag/v0.1.0
