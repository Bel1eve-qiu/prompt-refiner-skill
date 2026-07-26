# Prompt Refiner Skill

A Claude Code skill that helps non-technical users refine their prompts into clear, structured instructions that AI agents can execute accurately.

## Problem

When using AI coding agents, many users write long, unstructured prompts that are hard to understand — even for themselves. This leads to inaccurate results and wasted iterations.

## Solution

This skill takes a user's raw prompt, restructures it following prompt engineering best practices, and presents an optimized version. The user then chooses whether to use the refined prompt, keep the original, or make further edits.

## Installation

Copy the skill file into your project:

```bash
mkdir -p .claude/skills
cp prompt-refiner.md .claude/skills/
```

Or clone this repo and copy the file:

```bash
git clone https://github.com/Bel1eve-qiu/prompt-refiner-skill.git
cp prompt-refiner-skill/.claude/skills/prompt-refiner.md YOUR_PROJECT/.claude/skills/
```

## Usage

In Claude Code, invoke the skill:

```
/prompt-refiner
```

Then paste your prompt. The skill will:

1. Analyze your original prompt
2. Output a refined, structured version
3. Explain what was changed and why
4. Ask you to choose: use refined / use original / edit refined

## Example

**Before:**
> 帮我把这个页面改好看一点 那个按钮太丑了 还有加载速度也慢 顺便把那个bug修了

**After:**
> 优化当前页面的视觉和性能：
> 1. 重新设计提交按钮的样式（圆角、配色、hover 状态）
> 2. 排查页面加载慢的原因，优化资源加载
> 3. 修复 [具体 bug 描述需补充] 的问题
>
> 约束：不改变现有页面布局结构

## License

MIT
