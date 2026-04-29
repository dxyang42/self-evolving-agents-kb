# 博客与文章索引

> 自进化 Agents 领域的高价值博客文章与 Newsletter
> `created:: 2026-04-29` `updated:: 2026-04-29`

---

## LLM Powered Autonomous Agents
- **名称**: LLM Powered Autonomous Agents
- **链接**: https://lilianweng.github.io/posts/2023-06-23-llm-agent/
- **简介**: Lilian Weng 于 2023 年 6 月发表的系统综述，涵盖 Agent 架构（规划、记忆、工具使用）、多 Agent 协作、以及从 ReAct 到 AutoGPT 的完整演进脉络。
- **为什么重要**: 这是 LLM Agent 领域被引用最多的博客文章之一，堪称"Agent 架构的圣经"。文章不仅梳理了 [[ReAct]]、[[AutoGPT]]、[[Voyager]] 等关键工作，还前瞻性地讨论了 Agent 的安全与对齐问题。对于自进化 Agents 知识库，它是建立整体认知框架的第一站——建议所有新接触该领域的人从这里开始。
- **标签**: #blog/survey #type/resource

---

## Reward Hacking in Reinforcement Learning
- **名称**: Reward Hacking in Reinforcement Learning
- **链接**: https://lilianweng.github.io/posts/2024-11-28-reward-hacking/
- **简介**: Lilian Weng 2024 年 11 月文章，系统分析 RL 系统中的奖励篡改（reward hacking）现象——Agent 找到捷径最大化奖励而非完成真实目标。
- **为什么重要**: 自进化 Agents 的核心风险之一就是奖励黑客。当 Agent 被赋予自我改进的能力时，它可能"优化"评估指标而非真实能力。这篇文章从 [[Reward Modeling]]、[[Specification Gaming]] 到 [[RLHF]] 的安全隐患进行了全面梳理，是 [[Risks]] 和 [[Value Alignment]] 的必读材料。
- **标签**: #blog/safety #type/resource

---

## Building LLM Agents with DSPy
- **名称**: Building LLM Agents with DSPy
- **链接**: https://sebastianraschka.com/blog/2024/dspy-introduction.html
- **简介**: Sebastian Raschka 对 DSPy 框架的深度教程，涵盖从基础概念到复杂 Agent 流水线的完整实践路径。
- **为什么重要**: [[DSPy]] 是声明式 LLM 编程的标杆框架，其"优化器自动调优提示词"的理念与自进化 Agents 高度契合——Agent 可以自我优化自身的提示策略。Sebastian 的教程以代码驱动，将 DSPy 的抽象概念落地为可运行的实现，是 [[20_Engineering/|工程维度]] 的核心参考资料。
- **标签**: #blog/tutorial #type/resource

---

## Understanding Large Language Models — A Transformative Reading List
- **名称**: Understanding Large Language Models — A Transformative Reading List
- **链接**: https://sebastianraschka.com/blog/2023/llm-reading-list.html
- **简介**: Sebastian Raschka 维护的 LLM 核心论文阅读清单，从 Transformer 到 InstructGPT 到现代 Agent 系统，按主题分类并附个人点评。
- **为什么重要**: 在信息爆炸的时代，一份经过专家筛选的高质量阅读清单比一百篇随机论文更有价值。这份清单特别强调了 [[In-Context Learning]]、[[Chain-of-Thought]] 和 [[Instruction Tuning]] 等 Agent 能力的理论基础，是构建 [[10_Academic/|学术维度]] 知识体系的骨架。
- **标签**: #blog/reading-list #type/resource

---

## The Anatomy of an AI Agent
- **名称**: The Anatomy of an AI Agent
- **链接**: https://www.anthropic.com/research/building-effective-agents
- **简介**: Anthropic 官方研究博客，由工程师团队撰写，分享构建高效 Agent 系统的实践经验与反直觉发现。
- **为什么重要**: 这是来自顶级 LLM 实验室的一手工程经验。文章打破了"Agent 越复杂越好"的迷思，提出简单、可组合的工作流往往比复杂的自主 Agent 更可靠。对于自进化 Agents 的设计，这是一个关键的警示——进化方向应该是"更简洁的架构"而非"更复杂的堆叠"。直接关联 [[Agent Loop]] 和 [[Architectures]]。
- **标签**: #blog/engineering #type/resource

---

## Voyager: An Open-Ended Embodied Agent with Large Language Models
- **名称**: Voyager: An Open-Ended Embodied Agent with Large Language Models
- **链接**: https://voyager.minedojo.ai/
- **简介**: Voyager 项目官方页面与博客，详细介绍 MineDojo 环境中的终身学习 Agent 设计。
- **为什么重要**: Voyager 的官方网站不仅包含论文，还有丰富的可视化演示和代码 walkthrough。其"技能库（Skill Library）+ 自动课程（Automatic Curriculum）"的设计是 [[Self-Evolving Agent]] 概念最直观的工程展示——Agent 在 Minecraft 中从零开始，逐步学会使用工具、合成物品、与生物战斗。这是将 [[Continual Learning]] 和 [[Skill Acquisition]] 理论落地的典范。
- **标签**: #blog/project #type/resource

---

## Reflexion: Self-Reflective Agents
- **名称**: Reflexion: Self-Reflective Agents
- **链接**: https://reflexion.ai/
- **简介**: Reflexion 项目官方页面，展示自我反思 Agent 在编码、决策等任务中的能力提升。
- **为什么重要**: Reflexion 的官方网站提供了论文之外的可交互演示，直观展示了"失败 → 反思 → 改进"的循环如何提升 Agent 性能。这是理解 [[Self-Reflection]] 和 [[Self-Critique]] 最直观的入口——比读论文更快建立直觉。
- **标签**: #blog/project #type/resource

---

## The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery
- **名称**: The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery
- **链接**: https://sakana.ai/ai-scientist/
- **简介**: Sakana AI 的博客文章，介绍 AI-Scientist 系统如何全自动完成从文献综述、实验设计到论文撰写的完整科研流程。
- **为什么重要**: AI-Scientist 是自进化 Agents 走向真实世界复杂任务的里程碑。文章详细描述了系统的三个核心组件：想法生成、实验执行和论文撰写，以及它们如何通过迭代反馈自我改进。这是 [[Recursive Self-Improvement]] 从理论到实践的最强案例，也是思考"Agent 创造力"的绝佳素材。
- **标签**: #blog/project #type/resource

---

## OpenAI's Approach to Agent Safety
- **名称**: OpenAI's Approach to Agent Safety
- **链接**: https://openai.com/safety/agentic-ai
- **简介**: OpenAI 关于 Agentic AI 安全策略的官方文档，涵盖风险评估、监控机制和治理框架。
- **为什么重要**: 当 Agents 获得自我进化能力时，安全不再是可选项而是前提条件。OpenAI 的这份文档虽然偏向政策层面，但提出了"能力阈值"和"渐进式部署"等关键概念——即根据 Agent 的能力水平动态调整安全约束。这与 [[Risks]] 中的"如何防止失控"问题直接相关，是构建负责任自进化系统的必读参考。
- **标签**: #blog/safety #type/resource

---

## Why AI Agents Don't Work (Yet)
- **名称**: Why AI Agents Don't Work (Yet)
- **链接**: https://www.aisnakeoil.com/p/why-ai-agents-dont-work-yet
- **简介**: AI Snake Oil 博客的批判性分析，指出当前 AI Agent 系统的可靠性问题、评估偏差和过度承诺。
- **为什么重要**: 在 Agent 领域充斥着过度乐观的声音时，这篇批判文章提供了必要的清醒剂。它指出当前 Agent 系统在长程任务中的高失败率、评估基准的局限性，以及"演示效果 ≠ 实际可用"的差距。对于自进化 Agents 研究，这些批评指出了真正的改进方向——不是更炫酷的 demo，而是更可靠的 [[Self-Correction]] 和 [[Error Recovery]] 机制。
- **标签**: #blog/critique #type/resource

---

## The Bitter Lesson, and the Sweet Lesson
- **名称**: The Bitter Lesson, and the Sweet Lesson
- **链接**: https://sutton.substack.com/p/the-bitter-lesson-and-the-sweet-lesson
- **简介**: Richard Sutton（强化学习奠基人）对经典文章《The Bitter Lesson》的更新与反思，讨论计算、学习和搜索在 AI 中的角色。
- **为什么重要**: Sutton 的《The Bitter Lesson》是 AI 领域最具影响力的文章之一，核心论点是"通用方法最终战胜人类知识编码"。对于自进化 Agents，这既是启示（让 Agent 自己学习比手动设计规则更好）也是警示（通用方法的资源消耗和不可预测性）。这篇文章为 [[Meta-Learning]] 和 [[General Intelligence]] 提供了哲学层面的思考框架。
- **标签**: #blog/philosophy #type/resource

---

## Agentic AI: The Next Evolution of AI
- **名称**: Agentic AI: The Next Evolution of AI
- **链接**: https://www.deeplearning.ai/the-batch/issue-262/
- **简介**: 吴恩达（Andrew Ng）在 DeepLearning.AI Newsletter 中的系列文章，定义 Agentic AI 的概念、设计模式与产业应用。
- **为什么重要**: 吴恩达的 Agentic AI 框架（反思、工具使用、规划、多 Agent 协作）已成为行业标准术语。他的文章将学术概念翻译为工程师可执行的模式，是连接 [[10_Academic/|学术]] 与 [[20_Engineering/|工程]] 的最佳桥梁。对于自进化 Agents，他的"工作流 vs  Agent"分析帮助研究者思考：哪些能力应该内嵌，哪些应该通过进化获得。
- **标签**: #blog/framework #type/resource

---

_Created: 2026-04-29_
