---
title: Agent技能目录规范
tags:
  - xdd/workflow
  - xdd/skill
  - xdd/standard
note_type: standard
---

# Agent 技能目录规范

这份规则用于统一管理当前工作流里的 Agent 技能目录，避免同一套技能在不同工具里各放一份。

## 固定目录

Agent 技能统一安装在用户目录下的 `~/.agents/skills`，后续新增、整理、迁移和删除技能时，都以这个目录为准。

`~/.codex/skills` 和 `~/.claude/skills` 作为兼容入口使用，统一软链接到 `~/.agents/skills`。

## 使用规则

- 安装新技能时，统一安装到 `~/.agents/skills`
- 给 Codex 或 Claude Code 接入技能目录时，使用软链接，不额外复制技能文件
- 检查技能是否已经安装、需要整理或需要删除时，先看 `~/.agents/skills`
- 如果切换电脑，继续按这套目录约定配置，就可以正常接入现有技能目录

## 目录说明

| 目录 | 用途 |
| --- | --- |
| `~/.agents/skills` | 技能实际维护目录 |
| `~/.codex/skills` | Codex 使用的技能入口，软链接到 `~/.agents/skills` |
| `~/.claude/skills` | Claude Code 使用的技能入口，软链接到 `~/.agents/skills` |

## 示例

```bash
ln -s ~/.agents/skills ~/.codex/skills
ln -s ~/.agents/skills ~/.claude/skills
```
