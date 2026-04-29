# 课程与视频资源

> 自进化 Agents 领域的推荐课程、演讲与视频教程
> `created:: 2026-04-29` `updated:: 2026-04-29`

---

## DeepLearning.AI — AI Agentic Design Patterns
- **名称**: AI Agentic Design Patterns with AutoGen
- **链接**: https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/
- **简介**: 吴恩达与微软 AutoGen 团队合作的短课程，系统讲解反射（Reflection）、工具使用（Tool Use）、规划（Planning）和多 Agent 协作四大设计模式。
- **为什么重要**: 这是理解 Agent 设计模式最权威、最系统的入门课程。吴恩达的讲解风格将复杂概念拆解为可执行的代码块，而 AutoGen 框架提供了即插即用的实验环境。对于自进化 Agents，课程中的"反射模式"章节直接对应 [[Self-Reflection]] 概念，是理论与实践的最佳结合点。课程时长约 1 小时，适合快速建立整体认知。
- **标签**: #course/tutorial #type/resource

---

## CS 330: Deep Multi-Task and Meta Learning
- **名称**: Stanford CS 330 — Deep Multi-Task and Meta Learning
- **链接**: https://cs330.stanford.edu/
- **简介**: 斯坦福大学 Chelsea Finn 教授开设的元学习深度课程，涵盖 MAML、原型网络、贝叶斯元学习等核心方法。
- **为什么重要**: 元学习（Meta-Learning）是自进化 Agents 的理论基石之一——Agent 需要"学会学习"才能持续自我改进。这门课程从数学基础到前沿方法进行了系统梳理，特别是 [[MAML]]（Model-Agnostic Meta-Learning）和 [[Gradient-Based Meta-Learning]] 章节，为理解 Agent 如何快速适应新任务提供了形式化工具。课程视频、讲义和作业全部开源。
- **标签**: #course/academic #type/resource

---

## Jim Fan — Voyager 演讲与访谈
- **名称**: Jim Fan 关于 Voyager 和具身智能的系列演讲
- **链接**: https://www.youtube.com/results?search_query=jim+fan+voyager+agent
- **简介**: Jim Fan 在多个顶级会议（NeurIPS、CVPR、GTC）和播客中关于 Voyager、具身智能和终身学习的演讲与访谈合集。
- **为什么重要**: Jim Fan 的演讲不仅解释 Voyager 的技术细节，更重要的是分享设计哲学——为什么选择在 Minecraft 中测试、为什么技能库比端到端训练更好、为什么自动课程是关键。这些"为什么"在论文中往往被压缩，但在演讲中充分展开。对于理解 [[Voyager]] 的设计决策和 [[Self-Evolving Agent]] 的工程权衡，这些视频是不可替代的一手资料。
- **标签**: #video/talk #type/resource

---

## Lex Fridman Podcast — AI Agent 专题
- **名称**: Lex Fridman Podcast — AI Agents 系列访谈
- **链接**: https://lexfridman.com/
- **简介**: Lex Fridman 对 AI 领域顶级研究者的长格式深度访谈，涵盖 Agent 架构、安全、意识等主题。
- **为什么重要**: Lex Fridman 的访谈以深度和广度著称，单集时长常达 3-4 小时，允许受访者充分展开思路。推荐关注他与 [[Jim Fan]]、[[Yejin Choi]]、[[François Chollet]] 等 Agent 相关研究者的对话。这些访谈提供了论文之外的"研究动机"和"未发表想法"，对于理解 [[30_Philosophy/哲学维度 MOC|哲学维度]] 和 [[OpenProblems]] 特别有价值。
- **标签**: #video/podcast #type/resource

---

## Two Minute Papers — Agent 进化专题
- **名称**: Two Minute Papers — AI Agents and Self-Improvement
- **链接**: https://www.youtube.com/@TwoMinutePapers
- **简介**: 以 2-3 分钟短视频形式快速解读最新 AI 论文，涵盖 Voyager、Reflexion、FunSearch 等 Agent 相关研究。
- **为什么重要**: 在论文数量爆炸的时代，Two Minute Papers 提供了高效的"论文雷达"功能。其视频不仅总结核心贡献，还通过可视化演示帮助建立直觉。对于自进化 Agents 领域，它是跟踪 [[Voyager]]、[[Reflexion]]、[[FunSearch]]、[[AlphaEvolve]] 等关键工作最新进展的轻量渠道。适合作为深入阅读前的筛选工具。
- **标签**: #video/summary #type/resource

---

## Anthropic — Building Effective Agents (研讨会)
- **名称**: Anthropic — Building Effective Agents Workshop
- **链接**: https://www.anthropic.com/research/building-effective-agents
- **简介**: Anthropic 研究团队关于高效 Agent 构建的研讨会录像，分享从实际项目中提炼的工程最佳实践。
- **为什么重要**: 与博客文章相比，研讨会录像包含更多互动问答和案例讨论。Anthropic 工程师直接回答"何时该用简单工作流、何时该用复杂 Agent"等实践难题，这些判断对于自进化 Agents 的设计至关重要——进化不应该盲目增加复杂度，而应该找到"足够简单但足够强大"的架构。录像通常附带代码示例和架构图。
- **标签**: #video/workshop #type/resource

---

## Stanford CS 224N — Natural Language Processing with Deep Learning
- **名称**: Stanford CS 224N — NLP with Deep Learning
- **链接**: https://web.stanford.edu/class/cs224n/
- **简介**: 斯坦福大学经典 NLP 课程，涵盖 Transformer、预训练、微调、Prompting 等 LLM 基础。
- **为什么重要**: 自进化 Agents 建立在 LLM 能力之上，理解 LLM 的内部机制是必要前提。CS 224N 的 Transformer、[[Attention Mechanism]]、[[BERT]]、[[GPT]] 章节提供了这些基础。特别是近年更新的 [[In-Context Learning]] 和 [[Chain-of-Thought]] 内容，直接关联 Agent 的推理能力来源。课程作业包含实现 Transformer 等核心组件，是巩固理解的绝佳方式。
- **标签**: #course/academic #type/resource

---

## Andrej Karpathy — Let's build GPT: from scratch
- **名称**: Let's build GPT: from scratch, in code, spelled out
- **链接**: https://www.youtube.com/watch?v=kCc8FmEb1nY
- **简介**: Andrej Karpathy 的 2 小时直播编码视频，从零开始用 PyTorch 实现 GPT 训练。
- **为什么重要**: Karpathy 是 AI 教育领域最具影响力的讲师之一，这段视频以"从无到有"的方式揭示了 LLM 的内部工作原理。对于自进化 Agents 研究者，理解 LLM 的训练动态（梯度流动、注意力模式、token 预测）是设计有效进化策略的基础——你无法优化你不理解的东西。视频代码（nanogpt）也是轻量实验平台。
- **标签**: #video/tutorial #type/resource

---

## NeurIPS / ICML — Agent 相关 Tutorial
- **名称**: NeurIPS / ICML Agent 与 LLM 专题 Tutorial
- **链接**: https://nips.cc/virtual/2023/tutorials | https://icml.cc/virtual/2024/tutorials
- **简介**: 顶级机器学习会议上的 Agent 相关 Tutorial，通常由领域核心研究者主讲，涵盖最新进展和系统性综述。
- **为什么重要**: 会议 Tutorial 是获取领域"官方综述"的最高效方式。推荐关注 NeurIPS/ICML 上关于 [[LLM Agents]]、[[Reinforcement Learning from Human Feedback]]、[[Tool Learning]] 和 [[Multi-Agent Systems]] 的 Tutorial。这些材料通常在会议后 1-2 个月内公开视频和幻灯片，是建立前沿认知的权威来源。
- **标签**: #video/conference #type/resource

---

_Created: 2026-04-29_
