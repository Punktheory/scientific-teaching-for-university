# 🎓 scientific-teaching-for-university

<p align="center">
  <img src="./assets/readme/hero.svg" alt="Scientific Teaching for University hero" width="100%">
</p>

<p align="center">
  <strong>Turn AI from “answer generator” into a professor who actually teaches.</strong><br>
  <strong>让 AI 不只是回答你，而是真正把知识点教会你。</strong>
</p>

<p align="center">
  <a href="#-english-guide">English Guide</a> ·
  <a href="#-中文指南">中文指南</a> ·
  <a href="#-repository-structure">Structure</a>
</p>

---

# 🇬🇧 English Guide

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

## 🧠 Introduction

`scientific-teaching-for-university` is an educational-psychology-based AI teaching skill for university students. It is designed for lecture notes, slides, formulas, abstract concepts, and hard technical courses.

The goal is simple: make AI teach like a good professor.

That means the AI should:

- give the big picture before details;
- explain intuition before formal definitions;
- use examples before abstraction becomes too heavy;
- break math formulas down symbol by symbol;
- explain why the instructor placed this slide, concept, example, or table here;
- teach slide by slide instead of rushing through the whole deck.

## 🌍 Versions

| Version | Folder | Best for |
|---|---|---|
| 🌏 Default bilingual | `scientific-teaching-for-university` | Chinese explanations with English technical terms |
| 🇨🇳 Chinese version | `scientific-teaching-for-university-chinversion` | Full Chinese teaching for Chinese students |
| 🇬🇧 English version | `scientific-teaching-for-university-englishversion` | Full English teaching for public / international users |

## 🧩 Four Teaching Modes

<p align="center">
  <img src="./assets/readme/modes.svg" alt="Four teaching modes" width="100%">
</p>

| Mode | When to use | Teaching style |
|---|---|---|
| Mode 1 Easy | Descriptive / memory-heavy slides | Sentence-by-sentence explanation + light examples |
| Mode 2 Medium | Some harder concepts appear | Sentence-by-sentence explanation + higher-level concept teaching when needed |
| Mode 3 Hard | Math, CS, abstract, or technical courses | Real teaching: context, intuition, definitions, examples, formula breakdown |
| Mode 4 Deep Dive | Still confused after Mode 3 | Rebuild one hard concept from a more basic foundation |

## 🚀 Quick Start

### 1. Choose a version

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

Do not rush into the formula first. This slide is trying to answer one learning problem:

> The model is not good enough yet. How do we adjust its parameters step by step so the loss becomes smaller?

Intuitively, imagine the loss as the height of a mountain. You are standing on a slope and want to move downward. The gradient is like the steepest uphill direction under your feet. Since it points toward the fastest increase, we move in the opposite direction to decrease the loss.

The formula is:

\[
\theta := \theta - \alpha \nabla J(\theta)
\]

Symbol by symbol:

- \(\theta\): the model parameters, like adjustable knobs inside the model.
- \(J(\theta)\): the loss / cost function, measuring how wrong the model currently is.
- \(\nabla J(\theta)\): the gradient, telling us which direction makes the loss increase fastest.
- \(\alpha\): the learning rate, controlling how large each update step is.
- The minus sign: because the gradient points uphill, we subtract it to go downhill.

Why did the instructor place this slide here?

Because once a course defines the loss function, the natural next question is: how do we make that loss smaller? Gradient descent is the bridge between "defining the training objective" and "actually training the model."

## 🌟 Why It Matters

Good teaching is not dumping knowledge.

Good teaching means building stairs:

```text
context → intuition → example → definition → formula → evaluation → practice
```

This skill packages that teaching method into reusable AI instructions, so more students can use AI for serious learning instead of shallow Q&A.

---

# 🇨🇳 中文指南

## ✨ 这个 Skill 有什么不一样？

普通 AI 解释经常不好用，不是因为它不会这个知识点，而是因为它默认站在“已经懂了的人”的角度讲。

这个 skill 强制 AI 从学习者的起点出发：

<p align="center">
  <img src="./assets/readme/workflow.svg" alt="Teaching workflow" width="100%">
</p>

| 普通 AI 回答 | 这个 skill |
|---|---|
| 一上来堆术语 | 先给上下文和直觉 |
| 直接甩公式 | 先解释公式到底想干什么 |
| 默认你懂前置知识 | 主动补前置背景 |
| 只回答一个问题 | 把这一页 slide 放回课程结构里教 |
| 听起来很专业 | 让学习者真的听懂 |

## 🧠 中文介绍

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

## 🌍 版本选择

| 版本 | 文件夹 | 适合谁 |
|---|---|---|
| 🌏 默认中英混合版 | `scientific-teaching-for-university` | 中文讲解 + 英文术语，适合学英文讲义的中文母语学生 |
| 🇨🇳 全中文版 | `scientific-teaching-for-university-chinversion` | 希望所有讲解尽量中文化的学生 |
| 🇬🇧 全英文版 | `scientific-teaching-for-university-englishversion` | 面向 public / international users |

## 🧩 四档教学模式

<p align="center">
  <img src="./assets/readme/modes.svg" alt="Four teaching modes" width="100%">
</p>

| Mode | 中文 | 适合内容 | 讲法 |
|---|---|---|---|
| Mode 1 Easy | 简单内容 | 偏记忆、描述性的课 | 逐句讲解 + 轻量例子 |
| Mode 2 Medium | 重点内容 | 开始出现有难度的概念 | 逐句讲解 + 少量高层概念解释 |
| Mode 3 Hard | 困难内容 | 数学、计算机、抽象概念、技术课 | 真正教学：背景、直觉、定义、例子、公式拆解 |
| Mode 4 Deep Dive | 追加深挖 | Mode 3 讲完还是不懂 | 从更基础处重新搭台阶，一步步推上去 |

## 🚀 使用方法

### 1. 选择版本

大多数“中文母语 + 英文 lecture notes”的学生，推荐先用：

```text
scientific-teaching-for-university
```

如果你希望讲解尽量全中文，用：

```text
scientific-teaching-for-university-chinversion
```

如果你想给英文用户使用，用：

```text
scientific-teaching-for-university-englishversion
```

### 2. 在 Codex 里使用

把你想用的 skill 文件夹复制到 Codex skills 目录。

Windows PowerShell：

```powershell
Copy-Item -Recurse .\scientific-teaching-for-university "$env:USERPROFILE\.codex\skills\scientific-teaching-for-university"
```

macOS / Linux：

```bash
cp -R ./scientific-teaching-for-university ~/.codex/skills/scientific-teaching-for-university
```

然后这样调用：

```text
启用 scientific-teaching-for-university，困难模式，教我这门课。我会一页一页贴 slide。
```

### 3. 在 Claude Code / 其他 AI 工具里使用

如果你的工具支持 custom skills、agents、memories 或 reusable instructions：

1. 把你选择的文件夹加入自定义 skill / instructions。
2. 让 AI 读取该文件夹里的 `SKILL.md`。
3. 告诉 AI 使用哪个 mode。

示例：

```text
请使用 scientific-teaching-for-university/SKILL.md 里的教学规则。
用困难模式教我这门课，我会一页一页贴 slide。
```

如果你的工具不支持 skill：

1. 打开对应版本的 `SKILL.md`。
2. 把内容粘贴到 system / project / custom instructions。
3. 上传 PPT，或一页一页粘贴 slide 内容。

这套方法可以用于 Codex、Claude Code、ChatGPT Projects、Cursor、Windsurf，或者任何能遵循长指令的 AI 系统。

## 📚 推荐学习流程

```text
1. 启用 skill + 选择难度
2. 如果可以，先上传整份讲义 / PPT
3. 让 AI 先理解课程整体结构
4. 一页一页贴 slide
5. 让 AI 解释上下文、直觉、例子和公式
6. 如果还是不懂，说“再基础一点”，触发 Mode 4
7. 继续下一页
```

最佳中文 prompt：

```text
启用 scientific-teaching-for-university，困难模式。
请先通读整份讲义，告诉我这门课的大框架。
然后我会一页一页贴 slide，请你按初学者视角真正教会我。
```

## 🔥 使用前后对比示例

<p align="center">
  <img src="./assets/readme/comparison.svg" alt="Before and after teaching example" width="100%">
</p>

### Slide 内容

```text
Gradient descent updates parameters in the opposite direction of the gradient:

θ := θ - α∇J(θ)
```

### ❌ 不使用这个 skill

Gradient descent is an optimization algorithm that updates parameters by subtracting the learning rate times the gradient of the cost function. The gradient points in the direction of steepest ascent, so subtracting it minimizes the function.

### ✅ 使用这个 skill

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

## 🌟 为什么这件事重要？

好的教学不是把知识倒出来。

好的教学是在给学习者搭台阶：

```text
上下文 → 直觉 → 例子 → 定义 → 公式 → 评价 → 练习
```

这个 skill 把这套教学方法封装成可复用的 AI 指令，让更多学生能用 AI 进行真正有效的学习，而不是停留在浅层问答。

希望它能帮助更多大学生更快、更系统地用 AI 学会知识点。

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
