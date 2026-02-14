# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

本项目是一个 **雪花写作法 Claude Code Skill**，基于兰迪·英格曼森（Randy Ingermanson）所著《雪花写作法：10步写出一篇好小说》编制而成。

## Skill 结构

```
.claude/skills/snowflake-method/
├── SKILL.md                              # 主技能定义（含10步完整流程）
├── templates/                            # 各步骤输出模板
│   ├── step1-one-sentence.md             # 一句话概括模板
│   ├── step2-one-paragraph.md            # 一段式概括模板
│   ├── step3-character-summary.md        # 人物简介模板
│   ├── step4-synopsis.md                 # 故事梗概模板
│   ├── step5-character-synopsis.md       # 人物小传模板
│   ├── step6-full-outline.md             # 完整大纲模板
│   ├── step7-character-bible.md          # 人物宝典模板
│   ├── step8-scene-list.md               # 场景清单模板
│   ├── step9-scene.md                    # 单个场景描写模板
│   ├── step10-first-draft.md             # 第一稿写作指南
│   └── project-status.md                # 项目状态追踪模板
└── references/
    └── method-guide.md                   # 雪花写作法理论参考
```

## 使用方式

将 `.claude/` 目录复制到任意项目中，即可在该项目中使用"雪花写作法"技能。Claude Code 会自动识别 `.claude/skills/` 下的技能定义。

## 关键设计决策

- **语言**：所有内容为中文，匹配原书中译本
- **模板驱动**：每个步骤都有对应的输出模板，确保结构化输出
- **交互式引导**：Skill 设计为与用户协作式推进，每步确认后再继续
- **可回溯**：支持随时回到前面的步骤修改，符合雪花法的迭代理念
