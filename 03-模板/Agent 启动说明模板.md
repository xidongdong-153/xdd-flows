---
title: Agent 启动说明模板
tags:
  - xdd/template
  - xdd/agent
note_type: template
template_name: Agent 启动说明模板
template_version: v1
---

# Agent 启动说明模板

这份内容可以放进项目卡片，也可以整理到项目仓库 `AGENTS.md`。

## 可直接改的版本

```markdown
请先按下面顺序阅读当前项目，再开始处理任务：

1. 仓库根目录 `AGENTS.md`
2. `README.md`
3. `docs/architecture.md`
4. `docs/development.md`
5. 个人开发偏好说明
6. 开发技能调用规则
7. 项目里的文案规则说明
8. 当前任务直接相关的模块文档或目录

执行要求：

- 先理解当前目录和已有实现，再动代码
- 默认沿用已有命名、结构和文案风格
- 技术选型默认先按个人开发偏好判断
- React / Next.js 任务先按开发技能调用规则使用 `vercel-react-best-practices`
- ElysiaJS 后端任务先按开发技能调用规则使用 `elysiajs`
- 涉及说明性文案时，只写当前实现，不写历史过程
- 涉及 README、`docs/`、JSDoc、注释、错误提示、提示词或脚本说明时，先按文案规范整理
- 输出先给结论和修补方案，简单问题不做汇报式拆解
- 多项内容优先用 Markdown 表格，不显示 `P0`、`P1` 这类等级
- 结束时明确说明这次用到的 skill
- 涉及目录、流程、接口变化时，同步更新文档
- 输出以可直接使用为目标，不只给方向

当前项目补充规则：

- 项目名称：
- 仓库路径：
- 是否沿用个人开发偏好：
- 当前技术栈：
- 关键目录：
- 常用命令：
- 当前阶段：
- 当前任务重点：
```

## 使用建议

- 如果项目规则已经稳定，优先写进仓库 `AGENTS.md`。
- 如果项目还在搭架子，先放进项目卡片，后面再整理进仓库。
