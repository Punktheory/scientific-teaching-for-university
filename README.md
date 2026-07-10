# scientific-teaching-for-university

An educational-psychology-based AI teaching skill for university students. It turns AI from a generic answer machine into a lecture tutor that explains course materials from the learner's point of view.

这个项目的目标很纯粹：让 AI 真正教会你，而不是站在"已经懂了的人"的角度甩术语、甩公式、甩专业黑话。

## Why This Skill Exists

很多大学生会用 AI 辅助学习 lecture notes、PPT 和课本知识点，但普通问答式使用经常效果不好。原因通常不是 AI 不会这个知识点，而是它默认从专家视角讲：

- 它知道结论，但不知道你卡在哪里。
- 它会解释术语，但不会先建立直觉。
- 它能写公式，但不一定逐个符号拆给你看。
- 它会回答问题，但不一定解释这页 slide 为什么放在这里。

一个好的教授真正厉害的地方，是能站在学习者的认知起点上教学：先给上下文，再给直觉，再上正式定义，再用例子和评价把概念固定住。

## What It Does

This skill asks the AI to teach with a structured pedagogy:

- Start with the big picture and context before details.
- Explain hard ideas with plain language and intuition first.
- Introduce formal definitions only after the learner has a mental model.
- Break formulas down symbol by symbol.
- Pair every key concept with evaluation and examples.
- Explain why the instructor placed this content, example, formula, or table on the current slide.
- Move slide by slide, pausing after each page so the learner can digest and ask questions.

## Versions

This repository provides three versions:

| Folder | Language style | Best for |
|---|---|---|
| `scientific-teaching-for-university` | Chinese explanation with English technical terms | Default version for Chinese-native students studying English lecture notes |
| `scientific-teaching-for-university-chinversion` | Full Chinese teaching | Chinese students who want the most fluent Chinese learning experience |
| `scientific-teaching-for-university-englishversion` | Full English teaching | Public / international users |

## Four Teaching Modes

| Mode | Use case | Teaching style |
|---|---|---|
| Mode 1 Easy | Simple or descriptive courses | Sentence-by-sentence explanation, light examples and concept evaluation |
| Mode 2 Medium | Courses with some harder concepts | Sentence-by-sentence explanation plus occasional higher-level concept teaching |
| Mode 3 Hard | Math, CS, technical, or abstract courses | Real teaching: context, intuition, step-by-step breakdown, examples, formula dissection |
| Mode 4 Deep Dive | When Mode 3 is still too hard | Rebuild one difficult concept from a more basic foundation |

## Installation

Copy the version you want into your Codex skills directory.

Windows PowerShell example:

```powershell
Copy-Item -Recurse .\scientific-teaching-for-university "$env:USERPROFILE\.codex\skills\scientific-teaching-for-university"
```

macOS / Linux example:

```bash
cp -R ./scientific-teaching-for-university ~/.codex/skills/scientific-teaching-for-university
```

To install the Chinese-only or English-only version, replace the folder name with:

- `scientific-teaching-for-university-chinversion`
- `scientific-teaching-for-university-englishversion`

## Usage

Enable the skill, choose a difficulty, and upload or paste your lecture material.

Example prompts:

```text
Use scientific-teaching-for-university in hard mode to teach me this machine learning course.
```

```text
启用讲义家教，中等难度，教我这门课。
```

```text
Use scientific-teaching-for-university-englishversion in easy mode. I will paste the slides one by one.
```

Recommended workflow:

1. Upload the full PPT / lecture notes first if possible, so the AI can understand the course structure.
2. Paste one slide at a time, preferably as text.
3. Let the AI explain the page.
4. Ask follow-up questions or say "more basic please" to trigger deeper scaffolding.
5. Continue with the next slide.

## Example Teaching Requirements

When a slide contains a formula, the AI should not only state what the formula is. It should:

1. Explain what the formula is trying to do intuitively.
2. Define every symbol.
3. Read the formula as a plain-language sentence.
4. Use a minimal numeric example if useful.
5. Only then treat the formula as a whole.

When a slide contains a hard concept, the AI should:

1. Explain where the concept sits in the course.
2. Give a simple but accurate intuition.
3. Use a small concrete example.
4. Introduce the formal definition.
5. Evaluate when the concept is useful, limited, or easily confused with nearby ideas.

## Repository Structure

```text
.
├── scientific-teaching-for-university/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/pedagogy.md
├── scientific-teaching-for-university-chinversion/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/pedagogy.md
└── scientific-teaching-for-university-englishversion/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/pedagogy.md
```

## Author's Note

这个 skill 来自作者长期使用 AI 学习、研究教育心理学、观察好教授和差教授教学差异后的总结。核心结论很简单：教得好不是把知识倒出来，而是给学习者搭台阶。

希望它能帮助更多大学生更快、更系统地用 AI 学会知识点。
