# Self-Reflection

> `created:: 2026-04-29` `updated:: 2026-04-29`
> #type/concept #status/seedling

---

## 📖 定义

**Self-Reflection** in agent systems refers to the capacity of an agent to examine its own cognitive traces — including thoughts, actions, outcomes, and internal states — and generate evaluative or corrective judgments about them. It is a meta-cognitive process where the agent steps back from task execution to ask: *What did I do? Why did it fail or succeed? What should I do differently?*

In LLM-based agents, self-reflection is typically operationalized through:
- **Outcome-based reflection**: Comparing achieved results against expected goals.
- **Process-based reflection**: Reviewing the reasoning chain (CoT) for logical errors, hallucinations, or suboptimal choices.
- **Epistemic reflection**: Assessing the agent's own confidence, uncertainty, or knowledge gaps.

It is distinct from simple error detection in that it involves *narrative reconstruction* of the agent's own behavior, often producing explicit "lessons" that feed into future behavior.

---

## 🏛️ 起源/背景

Self-reflection as a cognitive mechanism has roots in human psychology (metacognition, theory of mind) and philosophy (Hegelian self-consciousness, Dewey's reflective thinking). In AI, it appears in:
- **ReAct** (Yao et al., 2022): Interleaving reasoning and action, with implicit feedback loops.
- **Reflexion** (Shinn et al., 2023): Explicit verbal reinforcement through self-generated feedback.
- **Chain-of-Verification**: Agents checking their own outputs.
- **Critique-and-Revise paradigms**: Multi-turn self-correction in reasoning tasks.

The move from "reflection as human-provided feedback" to "reflection as self-generated feedback" is a key step toward agent autonomy.

---

## 🔗 相关概念

- [[Self-Evolving Agent]]
- [[Recursive Self-Improvement]]
- [[Meta-Learning]]
- [[Memory Architecture]]
- [[Reflexion]]
- [[Chain-of-Thought]]
- [[Metacognition]]

---

## 🧠 我的理解

Self-reflection is the *conscience* of an agent loop — but it's a conscience that can be hallucinated. When an LLM reflects on its own reasoning, it is not accessing a privileged internal state; it is generating a plausible narrative about what it *might* have done wrong, based on the same statistical patterns that produced the original error. This means reflection can be self-deceiving: the agent may construct a coherent but incorrect critique, leading to "corrections" that make things worse.

I view self-reflection as a compression mechanism. The agent distills a complex interaction history into a compact "lesson" that can be stored in memory and retrieved later. The quality of the agent's long-horizon behavior depends heavily on the signal-to-noise ratio of this compression. Bad reflections are toxic memory — they poison future decisions.

---

## ⚠️ 我的批判/疑问

1. **The Narcissus trap**: Can an agent truly reflect on itself, or is it merely reflecting on its outputs as if they belonged to another agent? The LLM has no persistent self-model; each reflection is a fresh generation conditioned on a transcript. Is this "reflection" or "simulated reflection"? And does the distinction matter functionally?

2. **Confirmation bias in silicon**: Reflection mechanisms often search for plausible explanations of failure that preserve the agent's existing strategy. There's no guarantee of cognitive diversity in critique. How do we engineer "adversarial self-reflection" where the agent genuinely considers that its core assumptions are wrong?

3. **Cost and latency**: Real self-reflection requires multiple passes (generate → evaluate → revise). In production systems, this is expensive. Most deployed agents use shallow or cached reflection. Is deep self-reflection only a luxury of research demos, fundamentally incompatible with real-time constraints?

4. **Grounding problem**: Reflection judgments need a ground truth to be meaningful. In open-ended tasks, there is no oracle. The agent evaluates itself against its own (possibly flawed) model of correctness. This seems epistemically fragile — how do we break the circularity?

---

## 📌 实例

- **Reflexion** (Shinn et al., 2023): Agent writes verbal reinforcement signals to itself after task failure, stored in episodic memory.
- **Self-Refine** (Madaan et al., 2023): Iterative generation-feedback-refinement loop for code and reasoning.
- **Voyager's skill validation**: Agent tests generated code and reflects on execution errors to revise skill implementations.
- **Human metacognition (analog)**: The feeling of "knowing that you don't know" — poorly replicated in current LLMs, which often express false confidence.

---
_Created: 2026-04-29_
