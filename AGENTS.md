# AGENTS.md — 给 AI Agent 的工作指引

本文件面向自动化 AI Agent（编码助手、技能加载器、知识库机器人）。人类读者请看 [README.md](README.md)。

## 这个仓库是什么

`brain-design-benchmark` 是一个 **research 类 Agent Skill 发布包**，不是可运行的 SDK/服务。核心资产是 `SKILL.md`（遵循 Agent Skills 规范，带 YAML frontmatter）。把本目录放入 Agent 的技能目录，即可获得「类人 AI 大脑设计三向对标评估」能力。仓内无可执行后端逻辑，资产为文档 + 方法参考表。

## 可用的工作命令

```bash
# 查看技能元数据
cat manifest.json

# 查看技能主文件（触发词、方法、边界、frontmatter）
cat SKILL.md

# 查看 12 维度对标明细与神经科学参照
cat references/维度与对标.md
```

前置依赖：无运行时依赖；一个能加载 Agent Skill 的 AI 运行时即可。

## 约定（Do）

- 修改前先读 `SKILL.md` 的 YAML frontmatter，**保持字段兼容**（`name` / `slug` / `version` / `license` 等）。
- 新增评估维度或参考证据写进 `references/维度与对标.md`，并注明来源与「as of」日期。
- 沿用真实参照法：每条判断挂外部参照，无来源不主张。

## 禁止（Don't）

- 不要改动 `SKILL.md` / `manifest.json` 的 `copyright` / `author` 字段，也不要改 `LICENSE.md` 的版权主体——**权属字段只由维护者变更**。
- 不要在评估中使用「最 / 全球首创」等绝对词。
- 不要把本技能表述为医疗器械 / 医疗软件，不要加任何疗效或临床声明。
- 不要在仓库内提交任何密钥、令牌或真实客户数据。

## 边界

本技能专注「方法论层面的对标评估」；不覆盖具体模型训练、部署运维、医疗临床决策。它给的是差距分诊与路线图，不是保证结论。
