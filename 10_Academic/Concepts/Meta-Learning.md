# Meta-Learning

> `created:: 2026-04-29` `updated:: 2026-04-29`
> #type/concept #status/seedling

---

## 📖 定义

**Meta-Learning** (literally "learning to learn") is the process of acquiring learning algorithms, priors, or inductive biases that enable rapid adaptation to new tasks from limited experience. While standard machine learning optimizes model parameters for a fixed task distribution, meta-learning optimizes over *task distributions* — seeking a meta-level configuration (initialization, architecture, or optimization rule) from which specific tasks can be learned in few steps.

In the context of agents, meta-learning can operate at multiple levels:
- **Task-level**: Learning how to solve new types of problems quickly (e.g., MAML, prompt tuning).
- **Strategy-level**: Learning which reasoning strategies (CoT, ReAct, tool use) work best for which task classes.
- **Architecture-level**: Learning how to modify one's own network structure or prompt templates to improve future learning efficiency.

It is a *capability* that enables *acquisition of capabilities*, a second-order competence.

---

## 🏛️ 起源/背景

Meta-learning has a long history in psychology (Harlow's "learning sets" in primates, 1949) and machine learning (Schmidhuber's "self-referential learning," 1987). Key ML developments include:
- **MAML** (Finn et al., 2017): Model-Agnostic Meta-Learning — finding model initializations that adapt quickly.
- **LSTM Meta-Learners**: Learning the update rule for another network.
- **In-context learning in LLMs**: Emergent meta-learning where pretraining induces a learning algorithm that operates during inference via prompt conditioning.
- **Neural Architecture Search (NAS)**: Meta-learning at the architecture level.

In agent research, meta-learning bridges the gap between "pretrained generalist" and "task-specific expert" without requiring retraining from scratch.

---

## 🔗 相关概念

- [[Self-Evolving Agent]]
- [[Self-Reflection]]
- [[Recursive Self-Improvement]]
- [[Memory Architecture]]
- [[Few-Shot Learning]]
- [[Transfer Learning]]
- [[Inductive Bias]]
- [[MAML]]

---

## 🧠 我的理解

Meta-learning is the "compressed wisdom of experience." An agent that meta-learns is not just remembering past tasks; it is distilling *patterns of successful adaptation* into reusable procedures. This is crucial for self-evolving agents because evolution is too slow if every new capability must be discovered from scratch. Meta-learning provides the "evolutionary memory" — a shortcut through the search space of possible agents.

However, I think the term is often conflated with mere transfer learning. True meta-learning requires the agent to *improve its learning speed* over time, not just apply old knowledge to new tasks. Most LLM "in-context learning" is powerful but static: the model does not become a better in-context learner as it encounters more tasks. It is meta-capable but not meta-improving.

The frontier question: Can an LLM-based agent meta-learn its own prompting strategy? That is, can it learn *how to write prompts that make itself learn faster*? This would close a critical loop in self-evolution.

---

## ⚠️ 我的批判/疑问

1. **The level confusion**: Meta-learning is defined relative to a base level, but in complex agents, there are many levels (parameters, prompts, tools, goals). Is "meta" a fixed designation or relative to whatever we call the "object level"? A system that learns to optimize prompts is meta-learning relative to task execution, but what if it then learns to optimize its prompt-optimization strategy? We need a theory of *meta-level collapse* — when does the tower of meta-levels become unstable or meaningless?

2. **Emergence vs. design**: In LLMs, meta-learning (in-context learning) emerged from scale, not from explicit meta-learning objectives. This suggests that meta-capabilities may be a natural consequence of sufficient model capacity and diverse training data. If so, is explicit meta-learning research chasing a phenomenon that will emerge automatically? Or are there meta-capabilities (e.g., self-modification) that require explicit architectural support?

3. **Meta-overfitting**: Just as models overfit to training tasks, meta-learners can overfit to the distribution of training tasks. An agent meta-trained on coding tasks may fail to meta-learn scientific reasoning. How do we ensure broad meta-generalization? The problem seems harder than standard generalization because the space of "possible learning problems" is vastly larger than the space of possible tasks.

4. **Meta-learning vs. Self-Evolution — what's the difference?**: This boundary is fuzzy. I would argue: meta-learning is about *acquiring capabilities efficiently*, while self-evolution is about *transforming the agent's identity* (its goals, its architecture, its operational boundaries). Meta-learning makes you better at what you do; self-evolution changes what you are. But in practice, these blend. A self-evolving agent must meta-learn to be efficient; a meta-learning agent that modifies its own meta-learning strategy is evolving. The distinction may be one of degree and risk, not kind.

---

## 📌 实例

- **MAML**: Finding neural network initializations that require only a few gradient steps to adapt to new tasks.
- **GPT-4 in-context learning**: Given a few examples in the prompt, the model adapts its output distribution without weight updates — a form of implicit meta-learning.
- **Voyager's automatic curriculum**: The agent learns which tasks to attempt next based on its current skill level — meta-learning of exploration strategy.
- **Hyperparameter optimization agents**: Systems like Optuna or learned optimizers that meta-learn the training process itself.
- **Human cognitive development**: Children meta-learn how to learn — their learning strategies become more sophisticated with age, independent of domain-specific knowledge growth.

---
_Created: 2026-04-29_
