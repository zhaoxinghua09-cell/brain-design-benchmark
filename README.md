# brain-design-benchmark · 类人 AI 大脑设计评估框架

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-blue.svg)](SKILL.md)
[![Category](https://img.shields.io/badge/category-research-8a2be2.svg)](#)
[![Version](https://img.shields.io/badge/version-1.0.0-informational.svg)](#)
[![Multilingual](https://img.shields.io/badge/i18n-8%20languages-brightgreen.svg)](#)
[![llms.txt](https://img.shields.io/badge/AI--friendly-llms.txt-101E2C.svg)](llms.txt)
[![Grounded Reference](https://img.shields.io/badge/method-grounded%20reference-2ea44f.svg)](#)

> 评估任何「类人 AI 大脑设计」（方法论 / 多智能体组织 / 自研架构）的框架，用于回答「我这套 AI 大脑设计到底行不行」「跟真人脑差在哪」「跟前沿架构比落后多少」这类问题。
> A framework for benchmarking any "human-like AI brain design" (methodology / multi-agent organisation / in-house architecture) against the real human brain and 2026 frontier AI.

SynomosAI 四支柱体系：**身份（Identity）· 溯源（Traceability）· 治理（Governance）· 共生（Symbiosis）**——当 AI 进入商业，可信是唯一的硬通货。

**关键词 / Keywords**：AI 大脑设计评估 · 类人架构对标 · 多智能体组织 · 认知架构 · 三向对标 · 差距分诊 · 真实参照法 · brain design benchmark · architecture review · cognitive architecture · neuroscience · agent evaluation

本仓库是一个 **Agent Skill 发布包**：核心文件 `SKILL.md` 遵循 Agent Skills 规范（带 YAML frontmatter），把「把你的 AI 大脑设计当作一个统一智能体，与真实人脑、脑科学既有证据、以及 2026 前沿 AI 架构做三向对标」的方法固化为可被 AI Agent 直接加载的技能。

---

## ✨ 特性 / Features

- **三向对标**：把「我们的设计 / 真实人脑 / 前沿 AI（2026 产品·框架）」放在同一张 12 维度表上打分（1–10），诚实给出差距。
- **真实参照法（Grounded Reference Method）**：每条判断都挂得出外部参照——脑科学既有证据、公开前沿架构；无来源不主张。
- **禁用绝对词**：全程禁用「最 / 全球首创」等不可证伪表述，输出可核验的差距三档分诊。
- **12 维度覆盖**：记忆分层、主动执行、工具交互、自我一致、反思自省、规划推理、遗忘巩固、持续进化、安全治理、评测标准化、能效可扩、具身感知。
- **差距三档分诊 + 改善路线图**：不只打分，还告诉你哪几维是代际领先、哪几维是短板、先补哪里。
- **多语种**：中文、英、日、韩、西、法、德、阿（核心 8 种），识别输入语言并同语言回复。
- **研究向（research）**：不夹带可执行后端，专注方法论与对标参考数据。

---

## 🚀 快速开始 / Quick Start

前置：一个能加载 Agent Skill 的 AI 编码助手 / 技能运行时；本包本身是**文档 + 方法论**，无需安装运行时依赖。

```bash
# 1. 克隆本仓库（浅克隆即可）
git clone https://github.com/zhaoxinghua09-cell/brain-design-benchmark.git
cd brain-design-benchmark

# 2. 把技能目录放进你的 Agent 技能目录（示例：WorkBuddy）
#    cp -r . ~/.workbuddy/skills/brain-design-benchmark/

# 3. 查看技能主文件（触发词、方法、边界）
cat SKILL.md
```

然后直接用自然语言发起评估，例如：

```text
「帮我评估这套多智能体组织到底行不行」
「我的架构跟真人脑差在哪」
「跟 2026 前沿架构比落后多少」
```

---

## 🧪 评估方法示例 / Examples

技能会引导你按 12 个维度逐项打分，并引用 `references/维度与对标.md` 中的神经科学 / 前沿 AI 参照。一次典型对话的骨架如下：

```text
你：我有一套自研记忆引擎 + 规划器，想对标真人脑和前沿 RAG。
Agent：按 12 维逐项打分（我们的设计 / 真实人脑 / 前沿 AI），
      每维挂外部参照；无来源不主张。
      → 输出差距三档分诊 + 改善路线图（先补哪几维）。
```

参考数据文件里已给出一套示例打分（均值：我们 ≈ 6.75 ｜ 真人脑 ≈ 8.9 ｜ 前沿 AI ≈ 8.1），可据此校准你的评估口径：

```bash
# 查看 12 维度对标明细与神经科学参照
cat references/维度与对标.md
```

---

## 📁 仓库结构 / Repository layout

```text
brain-design-benchmark/
├── README.md            # 本文件（双语）
├── README.en.md         # 英文版说明
├── SKILL.md             # 技能主文件（Agent Skills 规范 · YAML frontmatter）
├── manifest.json        # 技能元数据（名称 / 版本 / 许可 / 描述）
├── references/
│   └── 维度与对标.md     # 12 维度对标明细 + 神经科学 / 前沿 AI 参照
├── LICENSE.md           # MIT 许可全文
├── SECURITY.md          # 安全策略
├── CONTRIBUTING.md      # 贡献指南
├── AGENTS.md            # 给 AI Agent 的工作指引
├── llms.txt             # 给 AI 的最小索引（llms.txt 标准）
└── llms-full.txt        # 给 AI 的完整文本
```

---

## 🔬 它回答什么 / What it answers

把你的 AI 大脑设计当作一个**统一智能体**，与三个参照系对齐：①你自己的设计；②真实人脑（自由能原理、睡眠记忆巩固、智力网络、意识 IIT/GNWT 等既有证据）；③2026 前沿 AI 架构（function calling、ToT/MCTS、RAG、向量记忆等）。输出诚实结论、差距三档分诊与改善路线图。

---

## 许可说明 · License Notice

- **权利状态**：本仓库以 **MIT 许可** 许可发布，可依该许可证条款自由使用、修改与再分发。
- **引用建议**：引用时请标注仓库名与原文链接 `https://github.com/zhaoxinghua09-cell/brain-design-benchmark`
  与权利人「赵兴华 / Steven Zhao·China」。
- **品牌状态限定**：MedXpert、SynomosAI、LGD 等为相关项目标识，
  **均未申请实体注册、未申请商标注册**；出现仅作来源标识，
  不构成对法人实体或商标权的任何主张。
- **完整条款**：见仓库根目录 [LICENSE](LICENSE)。
- **联系**：zhaoxinghua06@126.com ｜ ORCID 0009-0001-0512-1237

---

## 🔒 安全 / Security

如发现技能内容存在误导性结论、参考数据失实或其它安全问题，请按 [`SECURITY.md`](SECURITY.md) 的方式私下报告，不要在公开 issue 中披露。

## 🤝 贡献 / Contributing

欢迎按 [`CONTRIBUTING.md`](CONTRIBUTING.md) 提交改进。本仓库为技能发布包，改动请保持 `SKILL.md` frontmatter 兼容，权属字段只由维护者变更。

---

## ⚠️ 免责声明

本仓库内容为**理论站位与工具化探索**，不代表任何已获认证、已商业化交付或已服务特定客户的声明；文中涉及的外部标准、认证与条款信息为公开资料转述，正式引用前请**独立核实**。本技能为通用方法论工具，非医疗器械 / 非医疗软件，无疗效或临床声明。API、授权码与形象大使等为路线图（roadmap）事项，尚未上线。
