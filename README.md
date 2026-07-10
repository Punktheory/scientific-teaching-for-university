# 🎓 scientific-teaching-for-university

<p align="center">
  <img src="./assets/readme/hero.svg" alt="Scientific Teaching for University hero" width="100%">
</p>

<p align="center">
  <strong>Turn AI from “answer generator” into a professor who actually teaches.</strong><br>
  <strong>让 AI 不只是回答你，而是真正把知识点教会你。</strong>
</p>

<p align="center">
  <a href="#-english-introduction">English</a> ·
  <a href="#-中文介绍">中文</a> ·
  <a href="#-quick-start--使用方法">Quick Start</a> ·
  <a href="#-before--after-example">Before / After</a>
</p>

---

## ✨ What Makes This Different?

Most AI explanations fail because they teach from the perspective of someone who already understands the topic.

This skill forces the AI to teach from the learner's starting point:

<p align="center">
  <img src="./assets/readme/workflow.svg" alt="Teaching workflow" width="100%">
</p>

| Normal AI answer | This skill |
|---|---|
| Dumps terminology | Starts with context and intuition |
| Gives the final formula | Explains what the formula is trying to do |
| Assumes prerequisites | Fills in missing background |
| Answers one question | Teaches the slide as part of a course |
| Sounds professional | Makes the learner understand |

---

## 🇬🇧 English Introduction

`scientific-teaching-for-university` is an educational-psychology-based AI teaching skill for university students. It is designed for lecture notes, slides, formulas, abstract concepts, and hard technical courses.

The goal is simple: make AI teach like a good professor.

That means the AI should:

- give the big picture before details;
- explain intuition before formal definitions;
- use examples before abstraction becomes too heavy;
- break math formulas down symbol by symbol;
- explain why the instructor placed this slide, concept, example, or table here;
- teach slide by slide instead of rushing through the whole deck.

This repository provides three versions:

| Version | Folder | Best for |
|---|---|---|
| 🌏 Default bilingual | `scientific-teaching-for-university` | Chinese explanations with English technical terms |
| 🇨🇳 Chinese version | `scientific-teaching-for-university-chinversion` | Full Chinese teaching for Chinese students |
| 🇬🇧 English version | `scientific-teaching-for-university-englishversion` | Full English teaching for public / international users |

---

## 🇨🇳 中文介绍

读大学最崩溃的瞬间之一：打开讲义，满屏公式和术语，问 AI 之后它又甩你一脸“专业黑话”，越问越懵。

这个项目就是为了解决这个问题。

它把一套基于教育心理学和真实学习经验的教学方法做成 AI skill，让 AI 按一个真正会教学的教授那样讲：

- 先讲大框架和上下文，再进入细节；
- 难概念先给生活化直觉 / 类比，再给正式定义；
- 每个概念配“概念评价 + 例子”；
- 数学公式逐个符号拆开；
- 解释“老师为什么把这页放在这里”；
- 讲义一页一页讲，讲完一页停下来等你消化。

核心目的只有一个：通过这个 skill，让 AI **真正教会你**。

---

## 🧠 Four Teaching Modes / 四档教学模式

<p align="center">
  <img src="./assets/readme/modes.svg" alt="Four teaching modes" width="100%">
</p>

| Mode | 中文 | When to use | 讲法 |
|---|---|---|---|
| Mode 1 Easy | 简单内容 | Descriptive / memory-heavy slides | 逐句讲解 + 轻量例子 |
| Mode 2 Medium | 重点内容 | Some harder concepts appear | 逐句讲解 + 少量高层概念解释 |
| Mode 3 Hard | 困难内容 | Math, CS, abstract or technical courses | 真正教学：背景、直觉、定义、例子、公式拆解 |
| Mode 4 Deep Dive | 追加深挖 | Still confused after Mode 3 | 从更基础处重新搭台阶，一步步推上去 |

---

## 🚀 Quick Start / 使用方法

### 1. Choose a version / 选择版本

Most Chinese-native students studying English lecture notes should start with:

```text
scientific-teaching-for-university
```

Use the full Chinese version if you want every explanation in Chinese:

```text
scientific-teaching-for-university-chinversion
```

Use the English version for public / international use:

```text
scientific-teaching-for-university-englishversion
```

### 2. Use with Codex

Copy the skill folder into your Codex skills directory.

Windows PowerShell:

```powershell
Copy-Item -Recurse .\scientific-teaching-for-university "$env:USERPROFILE\.codex\skills\scientific-teaching-for-university"
```

macOS / Linux:

```bash
cp -R ./scientific-teaching-for-university ~/.codex/skills/scientific-teaching-for-university
```

Then invoke it like this:

```text
Use scientific-teaching-for-university in hard mode to teach me this machine learning lecture.
```

中文：

```text
启用 scientific-teaching-for-university，困难模式，教我这门课。我会一页一页贴 slide。
```

### 3. Use with Claude Code / Other AI Tools

If your tool supports custom skills, agents, memories, or reusable instructions:

1. Add the chosen folder as a custom skill / instruction resource.
2. Point the AI to that folder's `SKILL.md`.
3. Ask it to follow the mode you want.

Example:

```text
Use the instructions in scientific-teaching-for-university-englishversion/SKILL.md.
Teach this lecture in hard mode, slide by slide.
```

If your tool does not support skills:

1. Open the version's `SKILL.md`.
2. Paste it into the AI as system / project / custom instructions.
3. Upload your PPT or paste slides one by one.

This works with Codex, Claude Code, ChatGPT Projects, Cursor, Windsurf, or any AI system that can follow long custom instructions.

---

## 📚 Recommended Learning Workflow

```text
1. Enable the skill + choose difficulty
2. Upload the whole lecture deck if possible
3. Ask AI to understand the course structure first
4. Paste one slide at a time
5. Let AI explain context, intuition, examples, and formulas
6. Say "more basic please" to trigger Mode 4
7. Continue to the next slide
```

Best prompt:

```text
Use scientific-teaching-for-university in hard mode.
First read the whole lecture note and summarize the course structure.
Then I will paste slides one by one. Teach each slide from a beginner's perspective.
```

最佳中文 prompt：

```text
启用 scientific-teaching-for-university，困难模式。
请先通读整份讲义，告诉我这门课的大框架。
然后我会一页一页贴 slide，请你按初学者视角真正教会我。
```

---

## 🔥 Before / After Example

<p align="center">
  <img src="./assets/readme/comparison.svg" alt="Before and after teaching example" width="100%">
</p>

### Slide content

```text
Gradient descent updates parameters in the opposite direction of the gradient:

θ := θ - α∇J(θ)
```

### ❌ Without this skill

Gradient descent is an optimization algorithm that updates parameters by subtracting the learning rate times the gradient of the cost function. The gradient points in the direction of steepest ascent, so subtracting it minimizes the function.

### ✅ With this skill

先不要急着看公式。这个 slide 想解决的问题是：

> 模型现在表现不好，我们怎么一点点调整参数，让 loss 变小？

直觉上，你可以把 loss 想象成一座山的高度。你站在山坡上，想往低处走。gradient 就像脚下坡度最陡的上坡方向；既然它指向“上坡最快”，那我们要让 loss 下降，就往反方向走。

公式是：

\[
\theta := \theta - \alpha \nabla J(\theta)
\]

逐个符号拆：

- \(\theta\)：模型参数，可以理解成模型里需要调整的旋钮。
- \(J(\theta)\)：loss / cost function，用来衡量模型现在错得有多厉害。
- \(\nabla J(\theta)\)：gradient，告诉我们“往哪里调会让 loss 上升最快”。
- \(\alpha\)：learning rate，表示每一步走多大。
- 减号：因为 gradient 指向上升方向，所以我们要反着走，才能下降。

老师为什么把这页放这里？

因为在学训练模型时，前面通常已经定义了 loss。下一步自然就是问：有了 loss 以后，怎么把它变小？Gradient descent 就是连接“定义目标”和“训练模型”的桥。

---

## 🧩 Repository Structure

```text
.
├── assets/readme/
│   ├── hero.svg
│   ├── workflow.svg
│   ├── modes.svg
│   └── comparison.svg
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

---

## 🌟 Why It Matters

Good teaching is not dumping knowledge.

Good teaching means building stairs:

```text
context → intuition → example → definition → formula → evaluation → practice
```

This skill packages that teaching method into reusable AI instructions, so more students can use AI for serious learning instead of shallow Q&A.

希望它能帮助更多大学生更快、更系统地用 AI 学会知识点。
