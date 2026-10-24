# Course Sprint

[English](readme.md) | 简体中文

一个轻量级的 Codex skill，将课程材料整理为逻辑连贯、面向考试的学习指南，帮助你在有限时间内理解知识、选择解题方法，并写出完整的答案。

核心指令保存在 [SKILL.md](SKILL.md) 中，可用于 agent 能够访问和读取的 PowerPoint、PDF、Word 等课程材料。文档提取和图像检查能力取决于当前环境提供的工具。

## 学习逻辑

Course Sprint 按照六个步骤组织讲解：

1. **建立知识主线：** 串联课程的主要内容，按照前置知识关系安排学习顺序。
2. **理解核心概念：** 解释为什么需要这个概念、它是什么意思，以及如何使用。
3. **选择解题方法：** 识别题目特征，检查适用条件，选择方法并验证结果。
4. **学习完整例题：** 逐步讲解一道代表题，再给出简洁、规范的考场答案。
5. **避免典型错误：** 对比容易混淆的概念，通过纠错或反例解释问题所在。
6. **独立练习迁移：** 每个主题以简短回顾和一道变式题收尾，答案单独放置，方便先做后看。

始终围绕一个问题：**什么时候使用这个知识，为什么能够使用，以及如何写出完整答案？**

## 安装

首次安装时，将本仓库克隆到个人 skills 目录。以下路径遵循 [Codex 官方 skills 文档](https://learn.chatgpt.com/docs/build-skills) 中的本地发现规则。

**macOS / Linux**

```sh
git clone https://github.com/optima-xu/course-sprint.git ~/.agents/skills/course-sprint
```

**Windows PowerShell**

```powershell
git clone https://github.com/optima-xu/course-sprint.git "$env:USERPROFILE/.agents/skills/course-sprint"
```

Codex 会自动发现已安装的 skill。如果没有显示，请重启 Codex。

## 使用方法

让 Codex 能够访问你的学习材料，然后使用 `$course-sprint` 调用。可以同时说明可用时间、已有基础、学习范围和输出语言。

```text
使用 $course-sprint 帮我准备 CSC3001 考试。
请使用当前项目中的 Lecture Notes，不包含 Tutorial。
我只有一天时间，需要清晰的核心概念讲解、解题方法选择、
完整例题和简短自测。请用中文讲解，保留重要的英文术语。
```

也可以只复习一个主题：

```text
使用 $course-sprint 讲解这些讲义中的数学归纳法。
帮助我区分普通归纳法与强归纳法，判断什么时候使用哪一种，
并学会写出完整证明。请给出一道完整例题和一道变式题。
```

## 你会得到什么

- 串联所选主题的简短知识总览。
- 保留必要条件和关键推理的概念讲解。
- 代表题解答、常见错误，以及答案分开的练习题。
- 关键结论和例题的来源位置。
- 对仅作概述或尚未覆盖内容的明确说明。
