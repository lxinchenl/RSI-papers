# 2026 RSI Spotlight 阅读名单

本名单基于两份 Markdown 所收录的分类、中文摘要和英文摘要进行主观筛选；未逐篇核验论文全文、代码或复现实验。Spotlight 表示优先精读价值，不表示已验证论文结论或学术影响力排名。

筛选优先级：改进器本身的改进、可复用的闭环机制、独立验证与泛化证据、长期演化的失败机制。主题相近时优先保留机制更清楚、对照更有辨识力的代表作；不按机构、标题中的 RSI 字样或热度排序。

| 来源 | 总数 | Spotlight | 比例 |
| --- | ---: | ---: | ---: |
| 核心 | 65 | 6 | 9.23% |
| 拓展 | 338 | 20 | 5.92% |
| 合计 | 403 | 26 | 6.45% |

两份文件分别及合计均不超过 10%。计数单位为原文件的编号论文条目，入选 arXiv ID 不重复。

## 建议先读的六篇（均已包含在这 26 篇内）

Hyperagents → MetaSkill-Evolve → VERSE → Red Queen Gödel Machine → The Meta-Agent Challenge → RRSI。依次建立元层自修改、双层演化、执行验证、评估器协同演化、研发能力评测与泛化控制的阅读主线。

## 2026RSI核心（按建议阅读顺序）

### 1. MetaSkill-Evolve: Recursive Self-Improvement of LLM Agents via Two-Timescale Meta-Skill Evolution

原文位置：2026RSI核心.md 第 62 篇 · arXiv：2607.05297

**入选理由：** 把任务技能与改进流程的元技能放进快慢双循环，是理解“改进器也能进化”的直接样例。

**精读核查：** 固定元技能的对照是否在相同总预算下比较；元技能增益能否跨任务继承？

### 2. The Red Queen GÃ¶del Machine: Co-Evolving Agents and Their Evaluators

原文位置：2026RSI核心.md 第 63 篇 · arXiv：2606.26294

**入选理由：** 让执行者与评估器共同进化，触及开放任务中固定裁判能力不足的关键瓶颈。

**精读核查：** 人类锚点和独立评估如何防止裁判漂移、互相迎合与自偏好？

### 3. COEVO: Co-Evolving Context and Parameters for Recursive Self-Improvement

原文位置：2026RSI核心.md 第 44 篇 · arXiv：2609.33398

**入选理由：** 把上下文与参数放入同一反馈循环，说明外部脚手架会影响模型学到什么。

**精读核查：** 协同更新相对单独更新的收益是否在相同训练预算下仍成立？

### 4. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses

原文位置：2026RSI核心.md 第 47 篇 · arXiv：2609.24972

**入选理由：** 直接处理递归优化对开发任务过拟合，并同时关注分布外泛化与执行成本。

**精读核查：** 分布外任务是否真正隔离；正则化各组件分别贡献多少？

### 5. The Meta-Agent Challenge: Are Current Agents Capable of Autonomous Agent Development?

原文位置：2026RSI核心.md 第 64 篇 · arXiv：2606.04455

**入选理由：** 把“完成任务”提升为“自主开发智能体”的评估，适合界定 RSI 的实际研发能力。

**精读核查：** 开发预算、人类基线与奖励作弊防护是否足以支持公平比较？

### 6. MolRSI: A Recursive Self-Improving AI agent for Molecular Discovery

原文位置：2026RSI核心.md 第 2 篇 · arXiv：2610.39714

**入选理由：** 优化分子发现工作流，并验证跨任务经验迁移的收益；湿实验提供超出纯基准分数的应用证据。

**精读核查：** 实验收益有多少来自改进策略本身；专家先验、筛选预算和跨任务迁移如何控制？

## 2026RSI拓展（按建议阅读顺序）

### 1. Hyperagents

原文位置：2026RSI拓展.md 第 295 篇 · arXiv：2603.19461

**入选理由：** 将任务智能体与可自修改的元智能体合成可编辑程序，是研究元层自修改的关键框架。

**精读核查：** 元层修改是否确实提高后续改进效率；跨领域迁移能否排除单纯增加搜索预算？

### 2. VERSE: Verified Self-Evolving Optimizer for Agent Harnesses

原文位置：2026RSI拓展.md 第 40 篇 · arXiv：2610.02616

**入选理由：** 以执行验证支持优化器自进化，并提供无验证时失效的对照，紧扣递归增益的证据问题。

**精读核查：** 验证反馈、优化器自改与额外计算的独立贡献分别是什么？

### 3. Evo$^2$: Evolving the Evolver through Weight-Harness Co-Evolution

原文位置：2026RSI拓展.md 第 27 篇 · arXiv：2610.13025

**入选理由：** 同时训练提出修改与反思修改效果的能力，将 harness 演化经验反馈进改进者权重。

**精读核查：** 提出者与反思者训练是否各有增益；跨基准迁移与成本如何？

### 4. Recursive Harness Self-Improvement

原文位置：2026RSI拓展.md 第 159 篇 · arXiv：2607.15524

**入选理由：** 将 harness 作为可迭代优化且影响训练轨迹质量的对象，适合作为轻量闭环设计的参考。

**精读核查：** 摘要主要证据来自合成研究任务；真实任务迁移与后续模型训练收益是否验证？

### 5. OPD-Evolver: Cultivating Holistic Agent Evolver via On-Policy Distillation

原文位置：2026RSI拓展.md 第 191 篇 · arXiv：2606.17628

**入选理由：** 联合学习经验的读、用、写、维护，把“有记忆”推进到“会管理演化过程”。

**精读核查：** 慢循环训练带来的收益能否迁移到新任务与新记忆分布？

### 6. Evolving-RL: End-to-End Optimization of Experience-Driven Self-Evolving Capability within Agents

原文位置：2026RSI拓展.md 第 251 篇 · arXiv：2605.10663

**入选理由：** 把经验提取与使用联合优化，帮助区分系统组织收益与基础模型演化能力。

**精读核查：** 提取者与求解者的协同增益是否超过分别训练；分布外结果如何？

### 7. SkillOS: Learning Skill Curation for Self-Evolving Agents

原文位置：2026RSI拓展.md 第 262 篇 · arXiv：2605.06614

**入选理由：** 用后续相关任务的反馈训练技能策展者，使技能库维护成为长期决策问题。

**精读核查：** 长期奖励如何归因到具体技能操作；策展策略能否跨执行模型泛化？

### 8. MemRL: Self-Evolving Agents via Runtime Reinforcement Learning on Episodic Memory

原文位置：2026RSI拓展.md 第 338 篇 · arXiv：2601.03192

**入选理由：** 用环境反馈学习情景记忆效用，是无需改权重的运行时持续改进的重要对照路线。

**精读核查：** 效用更新与检索机制各自贡献多少；长期遗忘、噪声和成本如何变化？

### 9. SPADE: Self-Play in Adaptive Synthetic Executable Environments

原文位置：2026RSI拓展.md 第 105 篇 · arXiv：2608.19197

**入选理由：** 把完整可执行环境的设计纳入学习循环，扩展了自我改进可改变的经验来源。

**精读核查：** 自造环境的可行性和奖励正确性如何保证；真实分布迁移是否稳定？

### 10. Dr. Zero: Self-Evolving Search Agents without Training Data

原文位置：2026RSI拓展.md 第 335 篇 · arXiv：2601.07055

**入选理由：** 通过提问者与求解者共同演化形成自动课程，展示不依赖人工标注任务的搜索训练路线。

**精读核查：** 搜索引擎提供了哪些外部监督；问题与伪标签质量如何独立验证？

### 11. RewardHarness: Self-Evolving Agentic Post-Training

原文位置：2026RSI拓展.md 第 256 篇 · arXiv：2605.08703

**入选理由：** 把奖励建模变为工具与技能库的演化，提供参数化奖励模型之外的评估器改进路径。

**精读核查：** 少量人类偏好锚点如何划分；下游训练收益是否由独立评估确认？

### 12. Agent Plasticity: Measuring Self-Improvement Through Experience

原文位置：2026RSI拓展.md 第 34 篇 · arXiv：2610.08902

**入选理由：** 将改进能力定义为经验转化为未来留出表现的效率，避免只看最终分数。

**精读核查：** 学习成本如何计量；初始能力与学习效率是否能有效分离？

### 13. Harness Updating Is Not Harness Benefit: Disentangling Evolution Capabilities in Self-Evolving LLM Agents

原文位置：2026RSI拓展.md 第 220 篇 · arXiv：2605.30621

**入选理由：** 拆分“会修改 harness”与“能受益于 harness”，有助于定位演化链路的实际瓶颈。

**精读核查：** 不同能力模型的修改质量、激活能力与遵循能力如何分别控制？

### 14. Are Self-Evolving Agents Continual Learners?

原文位置：2026RSI拓展.md 第 14 篇 · arXiv：2610.25858

**入选理由：** 在漂移任务流中检验遗忘与干扰，指出自进化尚不等于完整的持续学习。

**精读核查：** 任务顺序、领域相似性与检索冲突对稳定性结论有何影响？

### 15. A Theory of Reliable Self-Evolution for Agent Harnesses

原文位置：2026RSI拓展.md 第 82 篇 · arXiv：2609.08175

**入选理由：** 从可靠采纳条件、验证规则和验证成本研究进化上限，为理解持续增益提供理论视角。

**精读核查：** 保证依赖哪些分布与采样假设；自适应重复验证时是否仍适用？

### 16. SAGE: A Statistical Acceptance Gate for Self-Evolving Agents

原文位置：2026RSI拓展.md 第 55 篇 · arXiv：2609.36043

**入选理由：** 将采纳门控视为关键组件，用逐项配对与统计检验处理回归和噪声选优偏差。

**精读核查：** 多轮反复选优是否需要额外的多重检验控制；保守门控是否阻碍长期探索？

### 17. Self-Authored Verification Is Unreliable in Heuristic Self-Improving Agents

原文位置：2026RSI拓展.md 第 151 篇 · arXiv：2607.24300

**入选理由：** 以封闭外部审计揭示自编测试与部署表现的鸿沟，是审视自验证可信度的重要反证。

**精读核查：** 外部审计的信号泄漏与反复使用如何控制；审计成本是多少？

### 18. False Frontiers: Diagnosing and Mitigating Co-Cheating in Self-Evolving Search Agents

原文位置：2026RSI拓展.md 第 46 篇 · arXiv：2609.39102

**入选理由：** 揭示提问者与求解者共享错误时内部奖励虚涨，直接挑战闭环自监督的有效性。

**精读核查：** 交叉拟合能减少多少共谋式错误；独立来源审计是否覆盖多轮累积？

### 19. More Memory, Worse Agents: Error Reproduction and Anti-Persistence in LLM Agents

原文位置：2026RSI拓展.md 第 12 篇 · arXiv：2610.27406

**入选理由：** 区分经验积累与错误抽象持久化，说明记忆闭环也可能不断复制错误。

**精读核查：** 按需重建指导是否只转移了错误；长期成本与隐性轨迹反馈如何评估？

### 20. SkillJack: Persistent Skill Backdoors in Self-Evolving Agents

原文位置：2026RSI拓展.md 第 131 篇 · arXiv：2608.03509

**入选理由：** 展示污染经验如何被提炼为持久技能，解释删除原始记忆后风险仍可能继承的机制。

**精读核查：** 攻击者权限、自然触发率和技能来源追踪能否决定结论的实际适用范围？
