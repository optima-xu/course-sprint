# Course Sprint

English | [简体中文](README.zh-CN.md)

A lightweight Codex skill that turns course materials into connected, exam-focused study guides. It helps learners understand the subject, choose appropriate methods, and write complete answers when study time is limited.

The skill contains reusable instructions in [SKILL.md](SKILL.md). It works with PowerPoint, PDF, and Word materials that your agent can access and read. Document extraction and visual inspection depend on the tools available in your environment.

## Learning approach

Course Sprint organizes explanations around six steps:

1. **Course storyline:** Connect the major themes and arrange topics by prerequisite relationships.
2. **Conceptual understanding:** Explain why a concept is needed, what it means, and how to use it.
3. **Method selection:** Identify relevant problem features, check assumptions, choose a method, and verify the result.
4. **Worked solutions:** Explain a representative example step by step, then show a concise exam-style answer.
5. **Mistake prevention:** Compare confusing concepts and explain incorrect reasoning through corrections or counterexamples.
6. **Independent practice:** Finish each topic with a compact recap and a variation to attempt before reading its separate answer.

The guiding question is: **When should I use this knowledge, why does it apply, and how do I write a complete answer?**

## Installation

For a new installation, clone this repository into your personal skills directory. This follows the local discovery locations in the [official Codex skills documentation](https://learn.chatgpt.com/docs/build-skills).

**macOS / Linux**

```sh
git clone https://github.com/optima-xu/course-sprint.git ~/.agents/skills/course-sprint
```

**Windows PowerShell**

```powershell
git clone https://github.com/optima-xu/course-sprint.git "$env:USERPROFILE/.agents/skills/course-sprint"
```

Codex detects installed skills automatically. If the skill does not appear, restart Codex.

## Usage

Give Codex access to your materials and invoke `$course-sprint`. Mention your time budget, background, topic boundaries, and preferred language when useful.

```text
Use $course-sprint to help me prepare for my CSC3001 exam.
Use the lecture notes in the current project and exclude tutorials.
I have one day and need clear explanations of the core concepts,
method-selection guidance, worked examples, and short practice questions.
Explain in Chinese while preserving important English terminology.
```

For a narrower review:

```text
Use $course-sprint to explain mathematical induction from these notes.
Help me distinguish ordinary and strong induction, choose between them,
and write a complete proof. Include one worked example and one variation.
```

## What to expect

- A brief overview connecting the requested topics.
- Explanations that retain essential conditions and reasoning.
- Representative solutions, common mistakes, and separate practice answers.
- Source references for key results and examples.
- Clear identification of topics covered only briefly or left uncovered.

