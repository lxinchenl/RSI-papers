# 2026 RSI Spotlight 阅读名单

基于当前两个文集的摘要、既有分类依据与精读价值筛选；优先考虑改进机制本身的更新、独立验证、长期演化和泛化。文集清理后重新控制比例，两个文集各自及合计均不超过 10%。未入选 Spotlight 的保留论文仍可在文集中查阅。

| 来源 | 总数 | Spotlight | 比例 |
| --- | --- | --- | --- |
| 核心 | 47 | 4 | 8.51% |
| 拓展 | 59 | 5 | 8.47% |
| 合计 | 106 | 9 | 8.49% |

建议先读：Hyperagents → MetaSkill-Evolve → VERSE → Red Queen Gödel Machine → SkillOS → OPD-Evolver。

## 2026 RSI 核心

### 1. MetaSkill-Evolve: Recursive Self-Improvement of LLM Agents via Two-Timescale Meta-Skill Evolution

[原文位置：核心版第 45 篇](2026RSI核心.md) · [arXiv：2607.05297](https://arxiv.org/abs/2607.05297)

**入选理由：** 把任务技能与改进流程的元技能放进快慢双循环，是理解“改进器也能进化”的直接样例。

**精读核查：** 固定元技能的对照是否在相同总预算下比较；元技能增益能否跨任务继承？

### 2. The Red Queen Gödel Machine: Co-Evolving Agents and Their Evaluators

[原文位置：核心版第 46 篇](2026RSI核心.md) · [arXiv：2606.26294](https://arxiv.org/abs/2606.26294)

**入选理由：** 让执行者、评估器与元智能体的改进循环共同进化，触及开放任务中固定裁判能力不足的关键瓶颈。

**精读核查：** 人类锚点和独立评估如何防止裁判漂移、互相迎合与自偏好？

### 3. COEVO: Co-Evolving Context and Parameters for Recursive Self-Improvement

[原文位置：核心版第 33 篇](2026RSI核心.md) · [arXiv：2609.33398](https://arxiv.org/abs/2609.33398)

**入选理由：** 把上下文与参数放入同一反馈循环，说明外部脚手架会影响模型学到什么。

**精读核查：** 协同更新相对单独更新的收益是否在相同训练预算下仍成立？

### 4. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses

[原文位置：核心版第 35 篇](2026RSI核心.md) · [arXiv：2609.24972](https://arxiv.org/abs/2609.24972)

**入选理由：** 直接处理递归优化对开发任务过拟合，并同时关注分布外泛化与执行成本。

**精读核查：** 分布外任务是否真正隔离；正则化各组件分别贡献多少？

## 2026 RSI 拓展

### 1. Hyperagents

[原文位置：拓展版第 55 篇](2026RSI拓展.md) · [arXiv：2603.19461](https://arxiv.org/abs/2603.19461)

**入选理由：** 将任务智能体与可自修改的元智能体合成可编辑程序，是研究元层自修改的关键框架。

**精读核查：** 元层修改是否确实提高后续改进效率；跨领域迁移能否排除单纯增加搜索预算？

### 2. VERSE: Verified Self-Evolving Optimizer for Agent Harnesses

[原文位置：拓展版第 12 篇](2026RSI拓展.md) · [arXiv：2610.02616](https://arxiv.org/abs/2610.02616)

**入选理由：** 以执行验证支持优化器自进化，并提供无验证时失效的对照，紧扣递归增益的证据问题。

**精读核查：** 验证反馈、优化器自改与额外计算的独立贡献分别是什么？

### 3. Evo$^2$: Evolving the Evolver through Weight-Harness Co-Evolution

[原文位置：拓展版第 9 篇](2026RSI拓展.md) · [arXiv：2610.13025](https://arxiv.org/abs/2610.13025)

**入选理由：** 同时训练提出修改与反思修改效果的能力，将 harness 演化经验反馈进改进者权重。

**精读核查：** 提出者与反思者训练是否各有增益；跨基准迁移与成本如何？

### 4. OPD-Evolver: Cultivating Holistic Agent Evolver via On-Policy Distillation

[原文位置：拓展版第 40 篇](2026RSI拓展.md) · [arXiv：2606.17628](https://arxiv.org/abs/2606.17628)

**入选理由：** 联合学习经验的读、用、写、维护，把“有记忆”推进到“会管理演化过程”。

**精读核查：** 慢循环训练带来的收益能否迁移到新任务与新记忆分布？

### 5. SkillOS: Learning Skill Curation for Self-Evolving Agents

[原文位置：拓展版第 49 篇](2026RSI拓展.md) · [arXiv：2605.06614](https://arxiv.org/abs/2605.06614)

**入选理由：** 用后续相关任务的反馈训练技能策展者，使技能库维护成为长期决策问题。

**精读核查：** 长期奖励如何归因到具体技能操作；策展策略能否跨执行模型泛化？

