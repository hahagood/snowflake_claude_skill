# 雪花写作法 Claude Skill

基于兰迪·英格曼森（Randy Ingermanson）所著《雪花写作法：10步写出一篇好小说》编制的 Claude Code 技能。通过10个渐进步骤，从一句话概括逐步扩展为完整的小说大纲。

## 安装

将本项目中的 `.claude/` 目录复制到你的小说创作项目中：

```bash
cp -r .claude/ /path/to/your-novel-project/
```

## 使用

在小说项目目录下启动 Claude Code，告诉它你想用雪花写作法创作小说即可。例如：

```
我想用雪花写作法写一部科幻小说
```

Claude 会自动识别技能，按步骤引导你完成创作。

## 十个步骤

| 步骤 | 名称 | 产出 |
|------|------|------|
| 1 | 一句话概括 | 不超过25字的故事核心 |
| 2 | 一段式概括 | 五句话构建三幕结构 |
| 3 | 人物简介 | 每个角色的动机、目标、冲突、顿悟 |
| 4 | 故事梗概 | 一页版故事大纲 |
| 5 | 人物小传 | 从角色视角写的一页人物传记 |
| 6 | 完整大纲 | 四页版详细大纲 |
| 7 | 人物宝典 | 角色完整档案 |
| 8 | 场景清单 | 全部场景的结构化列表 |
| 9 | 场景描写 | 每个场景的叙事描写 |
| 10 | 写小说 | 基于以上准备写第一稿 |

每个步骤都建立在前一步的基础上，随时可以回退修改——就像雪花分形一样，从简单到复杂，逐层生长。

## 文件结构

```
.claude/skills/snowflake-method/
├── SKILL.md                    # 技能定义与完整流程
├── templates/                  # 各步骤输出模板
│   ├── step1-one-sentence.md
│   ├── step2-one-paragraph.md
│   ├── step3-character-summary.md
│   ├── step4-synopsis.md
│   ├── step5-character-synopsis.md
│   ├── step6-full-outline.md
│   ├── step7-character-bible.md
│   ├── step8-scene-list.md
│   ├── step9-scene.md
│   ├── step10-first-draft.md
│   └── project-status.md
└── references/
    └── method-guide.md         # 雪花法理论参考
```
