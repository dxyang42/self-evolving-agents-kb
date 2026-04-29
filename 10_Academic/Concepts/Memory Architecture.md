# Memory Architecture

> `created:: 2026-04-29` `updated:: 2026-04-29`
> #type/concept #status/seedling

---

## 📖 定义

**Memory Architecture** in agent systems refers to the structured organization of information storage, retrieval, and updating mechanisms that enable an agent to maintain continuity across time, learn from experience, and ground its decisions in context beyond the immediate input. It is not merely "having a database" but the *epistemic scaffolding* that determines what the agent remembers, forgets, rehearses, and integrates.

For self-evolving agents, memory architecture is particularly critical because the agent's "self" — its capabilities, identity, and accumulated wisdom — is largely constituted by what it remembers and how it organizes that memory. A poor memory architecture leads to catastrophic forgetting, context window exhaustion, or inability to generalize across episodes.

---

## 🏛️ 起源/背景

The tripartite memory model (Episodic / Semantic / Procedural) originates from cognitive psychology, particularly Tulving's distinction between episodic and semantic memory, and the later inclusion of procedural memory in the declarative/non-declarative framework.

In AI, memory architectures have evolved through:
- **RNN hidden states**: Implicit, compressed memory in recurrent connections.
- **External memory networks** (Graves et al., 2014; Weston et al., 2014): Differentiable attention over memory slots.
- **Retrieval-Augmented Generation (RAG)**: Separating parametric memory (model weights) from non-parametric memory (external knowledge bases).
- **Agent memory systems** (e.g., Generative Agents, Voyager, MemGPT): Explicitly structured memory with read/write/update operations, often inspired by cognitive architectures (ACT-R, SOAR).

---

## 🔗 相关概念

- [[Self-Evolving Agent]]
- [[Self-Reflection]]
- [[Recursive Self-Improvement]]
- [[Meta-Learning]]
- [[Episodic Memory]]
- [[Semantic Memory]]
- [[Procedural Memory]]
- [[Catastrophic Forgetting]]
- [[Retrieval-Augmented Generation]]
- [[Working Memory]]

---

## 🧠 我的理解

Memory architecture is the *body* of a self-evolving agent. Without it, the agent is a ghost — each interaction starts from a blank slate. But simply adding a vector database is not enough. The architecture must answer: What deserves to be remembered? How is memory organized for efficient retrieval? How are conflicting memories reconciled? How does memory decay or consolidate?

I see three memory types as essential for any serious self-evolving agent:

**Episodic Memory**: Raw experience — what happened, in what context, with what outcome. This is the agent's autobiography. Without it, there is no self-narrative, no sense of history, no ability to learn from specific failures. Current agents often compress episodes into summaries, losing nuance. The challenge is episodic memory at scale: a year of an agent's life generates enormous trace data.

**Semantic Memory**: Generalized knowledge — facts, concepts, relationships, distilled from episodes. This is the agent's worldview. It must be editable (knowledge updates) and queryable (fast retrieval). The risk is ossification: semantic memory can become a prison of outdated assumptions that the agent never revisits.

**Procedural Memory**: How to do things — skills, strategies, habits, code. This is the agent's muscle memory. In LLM agents, procedural memory is often externalized as generated code or prompt templates. It is the most directly actionable memory type and the closest to "self-modification." The danger is procedural entrenchment: old skills block the acquisition of better ones.

The interplay between these three types is where the real intelligence lies. Episodes inform semantics; semantics guide procedure; procedure generates new episodes. A self-evolving agent needs not just storage but *memory dynamics* — consolidation, replay, reconsolidation, forgetting.

---

## ⚠️ 我的批判/疑问

1. **The compression-loss tradeoff**: We cannot store everything. Every compression of episodic memory into semantic or procedural form is a lossy transformation. What gets lost? Usually: context, uncertainty, counterfactuals. The agent remembers "what works" but forgets "why it might not work in different conditions." This creates overgeneralization. How do we preserve epistemic humility in compressed memory?

2. **Memory as ideology**: Semantic memory, once formed, resists change. An agent's "beliefs" become embedded in its retrieval and reasoning infrastructure. This is a form of computational ideology. How does an agent revise its semantic memory when new evidence contradicts old generalizations? Most current systems don't — they just append, leading to contradiction bloat.

3. **The ownership problem**: In multi-agent or human-agent systems, whose memory is it? If an agent's episodic memory includes interactions with humans, there are privacy and consent issues. If agents share a semantic memory pool, individual agency blurs. Memory architecture is not just technical; it is ethical and political.

4. **Forgetting is underrated**: Biological brains forget strategically — to reduce interference, to prioritize, to heal. AI memory systems almost never forget. They accumulate. This leads to retrieval noise, outdated information dominance, and inability to adapt to paradigm shifts. We need *active forgetting* mechanisms, but nobody knows how to design them for LLM-based agents.

5. **Grounding in the substrate**: LLM agents have two memory substrates: the model weights (parametric, slow to change) and external stores (non-parametric, fast). The relationship between these is poorly understood. When should knowledge be "compiled" into weights versus kept external? This is the cognitive architecture equivalent of the register-vs-memory problem in computer design, and we have no good theory.

---

## 📌 实例

- **Generative Agents** (Park et al., 2023): Episodic memory stream with reflection → semantic memory (observations → higher-level thoughts). Procedural memory implicit in behavior patterns.
- **Voyager**: Procedural memory as executable skill library (code). Episodic memory as task execution history. Semantic memory minimal — mostly implicit in the LLM's pretraining.
- **MemGPT**: Explicit memory hierarchy with OS-like memory management (paging between context window and external storage).
- **Human memory**: Episodic (your first day of school), Semantic (knowing Paris is the capital of France), Procedural (riding a bicycle). The dissociation between these is visible in amnesia patients who retain procedural skills while losing episodic memory.
- **Catastrophic forgetting in neural nets**: When training on new tasks destroys old task performance — a failure of memory architecture to segregate or consolidate properly.

---
_Created: 2026-04-29_
