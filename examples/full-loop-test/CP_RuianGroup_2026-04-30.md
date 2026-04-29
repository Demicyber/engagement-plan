# Call Plan — 瑞安集团 数据平台现代化

> **Purpose:** 为明天（2026-04-30）拜访瑞安集团 CTO 和 Head of Data 做准备。
>
> ✅ *生成后请 BD 审阅并修改。*

---

## 1. Meeting Details

| Field | Value |
|---|---|
| **Date & Time** | 2026-04-30 [待确认具体时间] |
| **Duration** | 1 小时（建议） |
| **Format** | [待确认 — In-person / Virtual] |
| **Location / Link** | [待确认] |
| **Opportunity Name** | 数据平台现代化（Oracle 数仓迁移至 AWS） |
| **Current Sales Stage** | Prospect |

### Customer Attendees

| Name | Title | Role in Decision |
|---|---|---|
| 陈明 | CTO | Decision Maker / 潜在 Champion |
| 刘洋 | Head of Data | Evaluator / Influencer |

### AWS Attendees

| Name | Title | Role in Meeting |
|---|---|---|
| [BD 姓名] | BD / Account Manager | Lead |

---

## 2. Target Meeting Outcomes

| # | Customer Perspective | Our Perspective |
|---|---|---|
| 1 | 了解 AWS 在数据平台迁移方面的能力和方案成熟度 | 验证痛点真实性：Oracle 数仓迁移是真实需求还是探索性了解 |
| 2 | 获得初步的迁移路径建议和同行案例参考 | 了解决策流程：谁拍板、预算怎么批、时间线是什么 |
| 3 | 评估 AWS 是否值得进一步深入接触 | 识别 Champion：陈明是否可以成为内部推动者 |

**Target Stage Progression:** ( Prospect ) → ( Qualified )

> *Prospect 阶段退出标准：客户机会已识别、有效估值确认、首次会议完成。目标通过本次拜访获取足够信息推进到 Qualified。*

---

## 3. Success Criteria

| # | Customer Would Consider It Successful If… | We Would Consider It Successful If… |
|---|---|---|
| 1 | AWS 展示了可信的 Oracle 迁移路径，不是泛泛的 PPT | 陈明明确表达 AWS 是候选方案之一（或首选） |
| 2 | 获得了至少一个相关行业的迁移案例参考 | 了解完整的决策链：Decision Maker、预算审批人、时间线 |
| 3 | 下一步有明确的技术深潜安排（2 周内） | 刘洋的核心顾虑被识别并有初步应对思路 |
| 4 | — | 确认竞争态势：是否有其他云厂商在接触 |

---

## 4. Information Exchange

### Information to Gather

| # | Question | Category | Target Attendee | Purpose |
|---|---|---|---|---|
| 1 | 当前 Oracle 数仓的整体规模？（数据量、核心表数量、日均 ETL 任务数、并发查询峰值） | Technical | 刘洋 | 评估迁移复杂度，为技术深潜做准备 |
| 2 | 最需要实时分析的 top 3 业务场景是什么？（门店库存、全渠道营销、供应链、定价？） | I (Identify Pain) | 陈明 / 刘洋 | 定义迁移优先级和 POC 范围 |
| 3 | 这个项目的决策流程是怎样的？最终谁拍板？预算走什么审批流程？ | DP (Decision Process) | 陈明 | MEDDPICC: 识别 EB 和审批流程 |
| 4 | 有没有一个明确的时间节点必须完成迁移？（合同到期、业务需求驱动？） | M (Metrics) / Timeline | 陈明 | 判断紧迫性和可能的关单窗口 |
| 5 | 目前有在接触其他云厂商吗？有没有倾向性？ | CP (Competition) | 陈明 | 了解竞争态势，制定差异化策略 |
| 6 | 迁移最大的顾虑是什么？有什么不能妥协的硬性要求？ | DC (Decision Criteria) | 刘洋 | 识别技术 blocker 和必须满足的条件 |
| 7 | 你们内部有没有做过迁移的可行性评估？结论是什么？ | Ch (Champion) | 陈明 | 判断内部推动力度，评估 Champion 潜力 |

### Information to Deliver

| # | What to Share | Format | Purpose |
|---|---|---|---|
| 1 | 零售行业数据平台迁移案例：从传统数仓迁移到 AWS 后实现实时库存分析、全渠道数据融合的成功案例 | 案例故事（口头） | 建立可信度，证明 AWS 在零售行业有成熟经验 |
| 2 | Oracle → AWS 迁移路径概览：SCT（Schema Conversion Tool）+ DMS（Database Migration Service）+ Redshift/Aurora 的典型迁移架构 | 简要架构图（白板 / 1 页图） | 让 CTO 和 Head of Data 看到具体可行的迁移路径，不是空洞承诺 |
| 3 | 实时分析能力亮点：Amazon Kinesis + Redshift Streaming Ingestion + QuickSight 实时仪表盘 | 数据点 / 简要说明 | 回应客户对实时分析的核心需求，展示 AWS 在实时场景的能力 |
| 4 | AWS 零售行业趋势洞察：全渠道零售数据融合、实时库存优化、AI 驱动的个性化推荐 | 行业洞察（口头） | 拓展对话范围，展示 AWS 对零售行业的深度理解 |

---

## 5. Potential Objections & Responses

| # | Anticipated Objection | Our Response |
|---|---|---|
| 1 | **"迁移过程中业务不能停——300+ 门店的实时库存系统怎么保证？"** *(← CDO Persona: 业务连续性是 Head of Data 最大顾虑)* | AWS DMS 支持增量迁移（CDC），可以在源系统继续运行的同时将数据同步到 AWS。典型模式是「双跑验证」：新旧系统并行运行一段时间，数据一致性验证通过后再切换。我们有大型零售客户用这个模式完成了零停机迁移。具体方案可以在技术深潜中详细展开。 |
| 2 | **"Oracle 用了很多年了，迁移成本和风险太高"** *(← CTO Persona: 架构决策需要平衡风险与收益)* | 理解这个顾虑。我们建议分阶段迁移：先选一个非核心但有代表性的工作负载做试点（比如营销分析或报表），验证迁移路径和性能后再扩展。AWS SCT 可以自动评估和转换 90%+ 的 Schema，大幅降低迁移工作量。另外，Oracle 许可成本逐年增长也是一个不迁移的风险——我们可以帮你做一个 3 年 TCO 对比。 |
| 3 | **"为什么选 AWS 而不是阿里云/Azure？"** | 几个差异化点：(1) AWS 在数据分析领域最成熟——Redshift 是全球使用最广的云数仓之一；(2) 你们已经有 EC2 工作负载在 AWS 上，[待确认]减少多云复杂度；(3) AWS 在零售行业有最深的实践——全球头部零售企业大部分在用 AWS。具体的技术对比可以在深潜中展开。 |
| 4 | **"我们内部没有云迁移经验，谁来做？"** | AWS 有专门的 Migration 团队和合作伙伴生态。我们可以推荐有零售行业迁移经验的合作伙伴，同时 AWS Professional Services 也可以做前期评估和方案设计。技术深潜时可以一起讨论交付模式。 |

---

## 6. Meeting Agenda

> *建议 1 小时。时间为相对偏移量。*

| Time | Topic | Owner | Purpose |
|---|---|---|---|
| 00:00–00:05 | 开场 & 相互介绍 | BD | 破冰，建立融洽氛围 |
| 00:05–00:15 | 了解瑞安集团数据平台现状和痛点 | BD（引导提问） | 验证痛点，收集 Section 4 中的关键信息 |
| 00:15–00:25 | 深入探讨实时分析需求和业务场景 | 陈明 / 刘洋（分享）| 了解 top 业务场景，为迁移优先级做准备 |
| 00:25–00:40 | AWS 数据平台迁移方案概览 + 零售行业案例分享 | BD | 展示迁移路径可行性，建立可信度 |
| 00:40–00:50 | 讨论顾虑与关键要求（业务连续性、迁移风险等） | BD（引导）+ 刘洋 / 陈明 | 识别 blocker、DC，回应关键异议 |
| 00:50–00:55 | 总结 & 对齐下一步 | BD | 确认下一步行动和时间安排 |
| 00:55–01:00 | 结束 | BD | — |

> **注意 Prospect 阶段 70/30 原则：** 客户说 70%，我们说 30%。多提问、多倾听，赢得第二次见面的机会，而非急于推销方案。

---

## 7. Potential Next Steps

| # | Proposed Next Step | Timeline | Owner | Purpose |
|---|---|---|---|---|
| 1 | 安排技术深潜：AWS SA 讲解详细迁移方案 + 业务连续性保障 | 2 周内 | Joint（AWS 协调 SA，客户确认参会人） | 验证技术可行性，推进到 Technical Validation |
| 2 | AWS 提供初步的 3 年 TCO 对比（Oracle vs. AWS） | 1 周内 | AWS | 为内部预算讨论提供数据支撑 |
| 3 | 客户提供当前数据架构信息（数据量、核心表、ETL 清单） | 1 周内 | Customer（刘洋） | 为技术深潜做输入，评估迁移复杂度 |

---

*Call Plan | Created: 2026-04-29 | Related EP: EP_RuianGroup_Data-Platform.md*
