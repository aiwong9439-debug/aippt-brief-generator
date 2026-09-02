# AiPPT Brief Generator Skill

把模糊想法、零散资料或已有提纲整理成可直接复制到 AiPPT 的专业结构化 Brief，减少首次生成偏差和反复修改。

## 安装

### Codex

将 `aippt-brief-generator` 文件夹复制到个人 Skills 目录，然后重新打开 Codex。在对话中输入：

```text
使用 $aippt-brief-generator，把“2026 年品牌增长策略”整理成面向管理层的 AiPPT Brief。
```

### Claude / 其他兼容 Agent

将包含 `SKILL.md` 的 `aippt-brief-generator` 文件夹导入支持 Agent Skills 的客户端。不同客户端的入口名称可能不同。

### 小红书 RED Skill

上传发布包时，压缩包根目录应直接包含 `SKILL.md`，不要再套一层 GitHub 项目目录。若后台要求填写名称、简介与默认提示词，可使用：

- 名称：AiPPT Brief 生成器
- 简介：把模糊想法整理成可直接用于 AiPPT 的专业 Brief
- 默认提示词：帮我把这个主题整理成一份可直接生成的 AiPPT Brief

小红书功能仍处于迭代期；上传前请以发布后台当日显示的字段和审核要求为准。

## 文件结构

```text
aippt-brief-generator/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── narrative-library.md
    ├── output-contract.md
    └── style-library.md
```

## 产品边界

该 Skill 负责整理 Brief，不替代 AiPPT 生成或编辑最终幻灯片。完整资料、图片和文件应在进入 AiPPT 后上传。

官方入口：<https://www.aippt.cn/?utm_source=github&utm_medium=skill&utm_campaign=ppt_brief_generator>
