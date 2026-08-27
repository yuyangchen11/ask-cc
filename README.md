# Ask CC

Ask CC 是我为秋招面试准备搭建的个人 AI Skill。它不是简单把简历丢给模型生成答案，而是把简历经历、项目资料、岗位理解、常见追问和回答标准整理成结构化知识库，让 AI 按照统一的口语化标准生成可被追问的面试回答。

## Why I Built It

在准备互联网、运营、策略和数据相关岗位时，我发现真正难的不是“背一份答案”，而是要能解释清楚每段经历背后的业务背景、用户逻辑、执行动作、数据结果和复盘空间。Ask CC 的目标就是把这套准备过程标准化。

## What It Contains

- `SKILL.md`: Codex Skill 入口，定义 Ask CC 的使用场景、回答原则和输出边界。
- `references/answer-standard.md`: 面试回答标准，约束回答必须自然、具体、可追问。
- `references/resume-context-public.md`: 公开版个人经历上下文，保留可展示信息，不包含完整私密题库。
- `references/evaluation-rubric.md`: 回答质量检查表，用于判断答案是否过空、过假或过度 AI 化。
- `examples/sample-questions.md`: 示例问题和示例回答方向。

## How It Works

Ask CC 会先读取候选人的经历背景，再根据问题类型选择回答框架。对于简历深挖问题，它会优先使用业务背景、个人职责、执行动作、结果数据和复盘改进的结构；对于岗位理解问题，它会结合用户生命周期、增长漏斗、内容转化或数据分析框架；对于行为面问题，它会用真实经历解释能力，而不是直接堆能力标签。

## Public Portfolio Version

这个仓库是公开展示版本，主要展示 Skill 的设计思路、结构和部分示例。完整面试题库和内部准备材料不放入公开仓库，避免泄露个人秋招底稿和未公开业务细节。

## How To Install Locally

If this repository is used as a Codex Skill source, install the Skill folder from:

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo yuyangchen11/ask-cc \
  --path .agents/skills/ask-cc
```

After installation, Ask CC can be invoked in a Codex task when preparing interview answers based on the included public context and answer standards.

## Suggested Repo URL

`https://github.com/yuyangchen11/ask-cc`

## Official Reference

Codex Skills are organized around a `SKILL.md` file and optional supporting resources. Official OpenAI documentation: https://developers.openai.com/codex/build-skills
