# 代码仓库索引

> 自进化 Agents 领域的高价值开源项目与框架
> `created:: 2026-04-29` `updated:: 2026-04-29`

---

## Voyager
- **名称**: Voyager
- **链接**: https://github.com/MineDojo/Voyager
- **简介**: 基于 LLM 的开放式终身学习 Agent，在 Minecraft 中通过自动课程和技能库实现持续自我提升。
- **为什么重要**: Voyager 是自进化 Agents 领域最具影响力的开源实现之一。其核心创新——[[Skill Library]]（可复用技能库）和 [[Automatic Curriculum]]（自动课程生成）——定义了"终身学习 Agent"的工程范式。代码质量高，文档完善，是理解 [[Continual Learning]] 和 [[Tool Use Evolution]] 的最佳实践参考。MineDojo 环境也使其成为可复现的实验平台。
- **标签**: #repo/agent-framework #type/resource

---

## AutoGPT
- **名称**: AutoGPT
- **链接**: https://github.com/Significant-Gravitas/AutoGPT
- **简介**: 最早的自主 GPT Agent 之一，能够设定目标、分解任务、执行行动并迭代直至完成。
- **为什么重要**: AutoGPT 是 2023 年 Agent 浪潮的引爆点，虽然其原始版本在长程任务中的可靠性备受争议，但它定义了"自主 Agent"的公众认知和基础架构（目标 → 思考 → 行动 → 记忆）。项目后续演进（如 Forge 框架、Benchmark 系统）使其成为 Agent 生态的测试场。对于自进化 Agents 研究，AutoGPT 的兴衰史本身就是关于"自主边界"的宝贵教训。
- **标签**: #repo/agent-framework #type/resource

---

## MetaGPT
- **名称**: MetaGPT
- **链接**: https://github.com/geekan/MetaGPT
- **简介**: 多智能体协作框架，将软件公司的 SOP（产品经理、架构师、工程师、测试员）映射到多 Agent 协作中，实现端到端的软件开发。
- **为什么重要**: MetaGPT 是 [[Multi-Agent Co-evolution]] 的工程标杆。它证明了当多个 Agent 扮演不同角色并遵循标准化流程时，可以产生远超单 Agent 的涌现能力。其代码结构清晰，角色定义和消息传递机制易于扩展，是研究"社会进化"（agents 通过协作互相提升）的首选平台。Star 数超过 40k，社区活跃。
- **标签**: #repo/agent-framework #type/resource

---

## DSPy
- **名称**: DSPy
- **链接**: https://github.com/stanfordnlp/dspy
- **简介**: 斯坦福大学 NLP 组开发的声明式 LLM 编程框架，将提示工程转化为可优化的模块化程序。
- **为什么重要**: DSPy 的核心理念——"用优化器替代手动提示调优"——与自进化 Agents 高度契合。其 [[Bootstrap Few-Shot]]、[[Chain-of-Thought]] 自动优化等功能，本质上是让程序自我改进其提示策略。对于自进化 Agents 研究，DSPy 提供了一套形式化的"元优化"工具，是构建 [[Self-Refine]] 和 [[Meta-Learning]] 系统的理想基础框架。
- **标签**: #repo/agent-framework #type/resource

---

## Reflexion
- **名称**: Reflexion
- **链接**: https://github.com/noahshinn024/reflexion
- **简介**: 自我反思 Agent 框架，通过 verbal reinforcement learning 让 LLM 从失败中学习和改进。
- **为什么重要**: Reflexion 是 [[Self-Reflection]] 概念最简洁、最直接的代码实现。其核心逻辑（执行 → 评估 → 反思 → 重试）不到百行即可理解，却能在编码、决策等任务上带来显著性能提升。对于研究者，这是验证"语言层面自我批评"假设的最小可行实现；对于工程师，这是为现有 Agent 添加自我改进能力的最轻量方案。
- **标签**: #repo/agent-framework #type/resource

---

## LangChain
- **名称**: LangChain
- **链接**: https://github.com/langchain-ai/langchain
- **简介**: 最广泛使用的 LLM 应用开发框架，提供链式调用、工具集成、记忆管理和 Agent 编排等全套工具。
- **为什么重要**: 尽管 LangChain 因过度抽象而受到一些批评，但它仍是 Agent 工程的事实标准基础设施。其 [[AgentExecutor]]、[[Tool]] 接口和 [[Memory]] 系统被大量项目采用。对于自进化 Agents 研究，LangChain 的价值在于其生态——几乎所有新 Agent 技术都会提供 LangChain 集成，使其成为跟踪领域进展的枢纽。
- **标签**: #repo/infrastructure #type/resource

---

## FunSearch
- **名称**: FunSearch
- **链接**: https://github.com/google-deepmind/funsearch
- **简介**: Google DeepMind 开源的基于 LLM 的进化发现系统，结合进化算法和 LLM 代码生成来发现新的数学构造和算法。
- **为什么重要**: FunSearch 是"LLM + 进化计算"融合的最强工业实现。它不仅在数学上取得了新发现（上限集问题），更重要的是其架构设计——LLM 作为"变异算子"，评估器作为"选择压力"，程序数据库作为"种群"。这是理解 [[Evolutionary Computation]] 与 [[LLM]] 结合的经典案例，也是 [[Recursive Self-Improvement]] 的实证基础。
- **标签**: #repo/research #type/resource

---

## CrewAI
- **名称**: CrewAI
- **链接**: https://github.com/joaomdmoura/crewAI
- **简介**: 多 Agent 协作框架，以"船员（Crew）"隐喻设计角色分工、任务委派和协作流程。
- **为什么重要**: CrewAI 在 MetaGPT 之后进一步简化了多 Agent 协作的门槛，其声明式的角色定义和流程编排使其成为快速原型多 Agent 系统的首选。对于自进化 Agents，CrewAI 展示了"社会结构"如何影响群体智能——不同的角色配置和协作拓扑会产生不同的涌现行为。这是研究 [[Multi-Agent Co-evolution]] 的轻量实验平台。
- **标签**: #repo/agent-framework #type/resource

---

## AutoGen (Microsoft)
- **名称**: AutoGen
- **链接**: https://github.com/microsoft/autogen
- **简介**: 微软研究院开发的多 Agent 对话框架，支持可定制、可对话的 Agent 协作解决复杂任务。
- **为什么重要**: AutoGen 的独特之处在于其"对话驱动"的 Agent 协作模型——Agent 通过自然语言对话协商、规划和执行任务。这种设计天然支持 [[Self-Reflection]]（对话中的批评）和 [[Self-Correction]]（对话中的修正）。微软的持续投入使其成为企业级多 Agent 系统的首选框架，也是研究"通信协议进化"的有趣平台。
- **标签**: #repo/agent-framework #type/resource

---

## SWE-agent
- **名称**: SWE-agent
- **链接**: https://github.com/princeton-nlp/SWE-agent
- **简介**: 普林斯顿 NLP 组开发的软件工程 Agent，在真实 GitHub 问题上实现自动修复。
- **为什么重要**: SWE-agent 是 Agent 从"玩具任务"走向"真实世界复杂任务"的代表作。它在 [[SWE-bench]] 上的优异表现证明了 Agent 可以处理需要深度推理、工具使用和长期规划的软件工程任务。对于自进化 Agents，SWE-agent 的"计算机接口（ACI）"设计——让 Agent 以人类方式与计算机交互——是 [[Tool Use Evolution]] 的重要参考。
- **标签**: #repo/research #type/resource

---

## AgentBench
- **名称**: AgentBench
- **链接**: https://github.com/THUDM/AgentBench
- **简介**: 清华大学开发的全面 Agent 评估基准，涵盖操作系统、数据库、知识图谱、数字卡牌游戏等 8 个环境。
- **为什么重要**: 自进化 Agents 需要可靠的评估体系来衡量"进化"是否真实发生。AgentBench 是当前最全面的通用 Agent 评估框架，其多环境设计可以测试 Agent 的泛化能力——真正的进化应该体现在跨任务的能力提升上。对于研究者，这是验证 [[Self-Evolving Agent]] 效果的必要基础设施。
- **标签**: #repo/benchmark #type/resource

---

## OpenHands (原 OpenDevin)
- **名称**: OpenHands
- **链接**: https://github.com/All-Hands-AI/OpenHands
- **简介**: 社区驱动的开源 Agent 平台，旨在复现和超越 Devin（AI 软件工程师）的能力。
- **为什么重要**: OpenHands 代表了开源社区对顶级闭源 Agent 系统的追赶努力。其模块化架构（Agent、运行时、前端分离）和活跃的社区贡献使其成为观察 Agent 工程最佳实践的窗口。对于自进化 Agents，OpenHands 的"Agent 技能市场"概念——Agent 可以安装和学习新技能——是 [[Skill Library]] 的社区化实现。
- **标签**: #repo/agent-framework #type/resource

---

## EvoPrompt
- **名称**: EvoPrompt
- **链接**: https://github.com/evolute-ai/evoprompt
- **简介**: 基于进化算法的自动提示词优化框架，将提示工程转化为可进化的搜索问题。
- **为什么重要**: EvoPrompt 是"提示词进化"的专用工具，其核心思想——将提示词视为基因型、LLM 输出质量视为适应度——为 [[Self-Refine]] 提供了形式化框架。虽然项目规模较小，但其设计简洁，是理解"进化优化 + LLM"结合方式的理想教学案例。
- **标签**: #repo/research #type/resource

---

_Created: 2026-04-29_
