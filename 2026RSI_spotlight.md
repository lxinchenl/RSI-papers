# 2026 RSI Spotlight 阅读名单

基于当前两个文集的摘要、既有分类依据与精读价值筛选；优先考虑改进机制本身的更新、独立验证、长期演化、泛化及不同路线的代表性。本轮按用户确认的新规则，Spotlight 总数最多 20 篇，替代此前的 10% 比例限制。 未入选 Spotlight 的保留论文仍可在文集中查阅；本轮没有把所有入选论文宣称为重新全文精读。

| 来源 | 总数 | Spotlight | 比例 |
| --- | --- | --- | --- |
| 核心 | 42 | 8 | 19.05% |
| 拓展 | 60 | 12 | 20.00% |
| 合计 | 102 | 20 | 19.61% |

建议先读：Hyperagents → MetaSkill-Evolve → VERSE → Red Queen Gödel Machine → SkillOS → OPD-Evolver。

## 2026 RSI 核心

### 1. MetaSkill-Evolve: Recursive Self-Improvement of LLM Agents via Two-Timescale Meta-Skill Evolution

[原文位置：核心版第 38 篇](2026RSI核心.md) · [arXiv：2607.05297](https://arxiv.org/abs/2607.05297)

**入选理由：** 用快慢双循环分别演化任务技能与元技能，明确区分执行能力和提出改进的能力。

**精读核查：** 元技能更新相对固定元技能的收益，能否在相同预算和新任务上保持？

### 2. The Red Queen Gödel Machine: Co-Evolving Agents and Their Evaluators

[原文位置：核心版第 39 篇](2026RSI核心.md) · [arXiv：2606.26294](https://arxiv.org/abs/2606.26294)

**入选理由：** 执行 Agent、裁判与元层代码共同演化，是评价机制进入递归闭环的代表。

**精读核查：** 独立锚点如何限制裁判漂移、互相迎合和自偏好？

### 3. Harness^2: Recursive Agent Harnessing for an Open World

[原文位置：核心版第 11 篇](2026RSI核心.md) · [arXiv：2610.14224](https://arxiv.org/abs/2610.14224)

**入选理由：** 同时改进执行 Harness 和跨任务的改进经验，面向没有真实答案验证器的开放世界。

**精读核查：** 对比探测的反馈有多可靠；经验库更新是否提升未来任务的改进效率？

### 4. Mixture of Self-Improving Branches For Agent Harness Optimization

[原文位置：核心版第 21 篇](2026RSI核心.md) · [arXiv：2609.37834](https://arxiv.org/abs/2609.37834)

**入选理由：** 分支分别更新开发任务子集和提案指导，使诊断目标与改进方向共同变化。

**精读核查：** 任务子集变化是否只造成选优偏差；测试隔离与分支路由贡献是否充分控制？

### 5. Dream-RSI: Recursive Self-Improvement through Evolving Worlds

[原文位置：核心版第 31 篇](2026RSI核心.md) · [arXiv：2609.14858](https://arxiv.org/abs/2609.14858)

**入选理由：** 用历史发现树构建回放世界，优化可执行探索策略，再部署到后续在线发现。

**精读核查：** 回放模拟的离策略偏差有多大；策略收益能否迁移到未探索区域？

### 6. COEVO: Co-Evolving Context and Parameters for Recursive Self-Improvement

[原文位置：核心版第 26 篇](2026RSI核心.md) · [arXiv：2609.33398](https://arxiv.org/abs/2609.33398)

**入选理由：** 把上下文与模型参数纳入同一反馈循环，研究外部经验如何影响后续训练。

**精读核查：** 协同更新相对单独更新的收益是否在相同训练预算下仍成立？

### 7. iCoder-27B: Recursive AI-Led Development of Frontier Industrial Coding Model

[原文位置：核心版第 33 篇](2026RSI核心.md) · [arXiv：2609.29626](https://arxiv.org/abs/2609.29626)

**入选理由：** 在人类给定 Research Skills 与阶段边界内，自主诊断实验并修订后训练和奖励使用规则。

**精读核查：** 人类先验与 Agent 自主发现各贡献多少；是否确有可复用训练策略更新？

### 8. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses

[原文位置：核心版第 28 篇](2026RSI核心.md) · [arXiv：2609.24972](https://arxiv.org/abs/2609.24972)

**入选理由：** 直接约束 Harness 递归优化的过拟合，同时关注留出泛化和执行成本。

**精读核查：** 正则化收益能否与额外验证预算区分；分布外任务是否真正隔离？

## 2026 RSI 拓展

### 1. Hyperagents

[原文位置：拓展版第 52 篇](2026RSI拓展.md) · [arXiv：2603.19461](https://arxiv.org/abs/2603.19461)

**入选理由：** 将任务 Agent 与元 Agent 放入同一可编辑程序，直接展示改进流程自身的持久修改。

**精读核查：** 元层修改是否提升后续改进效率；跨领域收益能否排除额外搜索预算？

### 2. VERSE: Verified Self-Evolving Optimizer for Agent Harnesses

[原文位置：拓展版第 11 篇](2026RSI拓展.md) · [arXiv：2610.02616](https://arxiv.org/abs/2610.02616)

**入选理由：** 让优化器的提示、技能、工具和钩子成为可修改对象，并以执行验证约束递归更新。

**精读核查：** 验证、优化器自改与额外计算的贡献是否分别得到控制？

### 3. Evo$^2$: Evolving the Evolver through Weight-Harness Co-Evolution

[原文位置：拓展版第 8 篇](2026RSI拓展.md) · [arXiv：2610.13025](https://arxiv.org/abs/2610.13025)

**入选理由：** 将提出修改、反思与跨分支整合经验反馈到演化器权重，研究会改进的改进器。

**精读核查：** Proposer 与 Reflector 的独立贡献、跨任务迁移和训练成本分别是多少？

### 4. ClawLoop: Self-Improving Agents via Harness-Native Training Loop

[原文位置：拓展版第 7 篇](2026RSI拓展.md) · [arXiv：2610.14118](https://arxiv.org/abs/2610.14118)

**入选理由：** 明确区分训练任务池和留出诊断任务池，并联合更新出题、验证代码与求解策略。

**精读核查：** 训练与诊断隔离是否完整；新验证器是否通过独立正确性审查？

### 5. SkillMentor: LLM Agent Self-Evolution via Learning Blind-Spot Diagnosis

[原文位置：拓展版第 31 篇](2026RSI拓展.md) · [arXiv：2607.27360](https://arxiv.org/abs/2607.27360)

**入选理由：** 直接学习生成盲区诊断任务，再将失败整理为纠正技能，突出可学习的诊断能力。

**精读核查：** 诊断策略学习的收益能否与技能编写和额外测量预算分开？

### 6. CoEvoSkills: Self-Evolving Agent Skills via Co-Evolutionary Verification

[原文位置：拓展版第 51 篇](2026RSI拓展.md) · [arXiv：2604.01687](https://arxiv.org/abs/2604.01687)

**入选理由：** 技能包与代理验证器交替修订，同时保留隐藏真实测试作为外部锚点。

**精读核查：** 代理验证器是否只是迎合当前技能；跨执行模型泛化是否稳健？

### 7. OPD-Evolver: Cultivating Holistic Agent Evolver via On-Policy Distillation

[原文位置：拓展版第 38 篇](2026RSI拓展.md) · [arXiv：2606.17628](https://arxiv.org/abs/2606.17628)

**入选理由：** 联合训练经验的读取、使用、写入与维护，把经验库更新能力内化到策略。

**精读核查：** 慢循环蒸馏是否提升新任务和新记忆分布下的长期演化能力？

### 8. SkillOS: Learning Skill Curation for Self-Evolving Agents

[原文位置：拓展版第 46 篇](2026RSI拓展.md) · [arXiv：2605.06614](https://arxiv.org/abs/2605.06614)

**入选理由：** 用后续相关任务的延迟反馈训练技能策展器，学习新增、修订和删除技能。

**精读核查：** 长期奖励如何归因到具体编辑；策展策略能否跨执行器迁移？

### 9. Learning to Build the Environment: Self-Evolving Reasoning RL via Verifiable Environment Synthesis

[原文位置：拓展版第 44 篇](2026RSI拓展.md) · [arXiv：2605.14392](https://arxiv.org/abs/2605.14392)

**入选理由：** 学习生成可执行训练环境，借助 oracle/scorer 与解决—验证不对称性维持学习信号。

**精读核查：** 环境有效性和新颖性如何保证；生成环境能否持续超过当前模型的能力边界？

### 10. SAGE: A Statistical Acceptance Gate for Self-Evolving Agents

[原文位置：拓展版第 13 篇](2026RSI拓展.md) · [arXiv：2609.36043](https://arxiv.org/abs/2609.36043)

**入选理由：** 为持久技能修改提供统计验收门，正面处理回退和含噪选优。

**精读核查：** 多轮自适应选优的统计误差是否受控；保守验收是否阻碍长期进步？

### 11. Self-Authored Verification Is Unreliable in Heuristic Self-Improving Agents

[原文位置：拓展版第 33 篇](2026RSI拓展.md) · [arXiv：2607.24300](https://arxiv.org/abs/2607.24300)

**入选理由：** 揭示自行编写验证器与真实部署表现的偏差，并提出封闭外部验收循环 SEAL。

**精读核查：** 外部审计需要多少信号；完整状态回滚能否阻断验证器与策略共同退化？

### 12. False Frontiers: Diagnosing and Mitigating Co-Cheating in Self-Evolving Search Agents

[原文位置：拓展版第 12 篇](2026RSI拓展.md) · [arXiv：2609.39102](https://arxiv.org/abs/2609.39102)

**入选理由：** 用 CrossFit 隔离出题与反馈来源，缓解自博弈中提问者和求解者共同犯错。

**精读核查：** 去除同源反馈后收益能否持续；独立审计能否覆盖多轮累积错误？

