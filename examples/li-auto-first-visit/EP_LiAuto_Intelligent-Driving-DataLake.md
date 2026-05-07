# Engagement Plan: 理想汽车 (Li Auto) - Intelligent Driving Data Lake + OTA Platform

> **What is this?** A focused action plan for winning a specific opportunity. Answers: who do I need to win, what do I need from each person, and what's my engagement roadmap to get there?
>
> 🤖 *Automatically generated. Updated after each visit.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise.*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | 理想汽车 (Li Auto) — 智能驾驶事业部 |
| **Opportunity Name** | Intelligent Driving Data Lake + OTA Platform |
| **Deal Value** | $1.5M ARR |
| **Current Stage** | Prospect |
| **Target Close Date** | 2026-Q4 `[待确认 — 首次接触后验证 timeline]` |
| **Why Now** | 理想汽车 2026 年智驾全栈自研加速，路测数据量月增 300TB+，现有阿里云 OSS + MaxCompute 架构出现数据回灌延迟（路测数据从车端到训练集 >48h）和存储成本失控（月费用同比增 220%）。同时多云评估已列入技术委员会 Q2 议程。 |
| **Deal Objective** | 成为理想智驾数据湖主力平台（S3 + Lake Formation + SageMaker），同步拿下 OTA 数据分发场景（CloudFront + IoT Core），签署 $1.5M PPA by Q4 2026。 |

### Win Strategy

理想汽车的核心痛点是**智驾数据闭环的速度瓶颈** — 路测数据从车端回传到标注完成到模型训练，现有链路需要 48 小时以上，而竞争对手小鹏已经做到 6 小时（据行业交流）。这不是存储成本问题，而是研发效率问题 — 每多等一天，模型迭代就慢一轮，智驾功能 OTA 推送就晚一周。我们的 win theme 是 **"数据到模型 6 小时闭环"：S3 Intelligent-Tiering 解决存储成本 + Lake Formation 统一数据治理 + SageMaker 端到端训练 pipeline + IoT Greengrass 边缘预处理加速回传**。竞争格局：阿里云是存量供应商但 AI/ML 训练生态弱（PAI 平台成熟度不如 SageMaker），华为云在车企圈有影响力但数据湖方案碎片化。我们的差异化：AWS 全球汽车行业客户密度（BMW、Toyota、Rivian）+ SageMaker Ground Truth 自动标注 + 数据湖 + 训练一体化架构，且有蔚来在 AWS 上做智驾数据湖的参考案例可以调用。

---

## 2. Engagement Plan

> *Pull stance and relationship history from **Contact Profiling Skill**. For executive-level (C-suite/VP), also pull role-level priorities and pain points from **CXO Personas**. Do NOT include people who are not involved in this opportunity.*

### Key Stakeholders

**郎咸朋 (Lang Xianpeng)** — VP of Intelligent Driving R&D (智能驾驶研发副总裁)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Economic Buyer + Technical Decision Maker — 智驾事业部最高负责人，掌握部门预算（>$5M/年），技术路线最终拍板。直接向 CEO 李想汇报。 |
| **Current Stance** | Neutral-Curious — 同意见面说明有兴趣，但作为 VP 级别不会轻易表态。多云评估是技术委员会集体决策，他是主席但不会独断。 `[待确认 — 首次接触后验证]` |
| **What They Care About** | *← CXO Persona: VP Engineering (Automotive context)* — 智驾研发效率（数据闭环速度是核心 KPI）；模型迭代频率和 OTA 推送节奏；团队规模控制（用平台能力替代人力堆砌）；供应商生态多元化降低单一依赖风险；技术债务控制。Agent focus: 本次 opp 重点是**数据闭环速度 + 多云战略**，团队规模和技术债务是加分项但非决策核心。 |
| **Profiling** | *← Contact Profiling (initial, from public info + channel partner input)* — 中科院沈阳自动化所博士，曾任职方正集团和百度（前百度自动驾驶事业部技术骨干）。2018 年 1 月加入理想汽车，是智能驾驶部门首位员工，从 0 到 1 搭建了整个智驾团队。在百度时以 "数据驱动派" 著称（vs 规则派），相信 "数据规模决定智驾上限"。公开演讲风格偏学术，喜欢看 benchmark 数据和 A/B 实验结果，对纯商业 pitch 没耐心。LinkedIn 上活跃，经常转发 arXiv 论文。 `[待确认 — 首次接触后补充个人沟通风格和决策习惯]` |
| **What We Need From Them** | 确认多云评估的真实动机和 timeline；确认决策流程和其他参与者；agree to 技术 deep-dive as next step |
| **How to Win Them** | SA lead + Automotive Specialist 双打。用技术深度赢得尊重 — 准备一个 "智驾数据闭环 6h vs 48h" 的架构对比（whiteboard level）。带蔚来数据湖案例的技术细节（不只是 business outcome，要有架构图和性能数据）。不要在第一次就推 PPA — 这种技术型 VP 需要先被技术说服。预计需要 3-4 次 meeting 才能拿到明确支持。 |

**孙浩 (Sun Hao)** — Platform Architecture Director (平台架构总监)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Technical Evaluator / Potential Champion — 负责智驾平台底层架构选型，是郎咸朋的技术参谋。如果他认可 AWS 方案，会成为内部推动者。 |
| **Current Stance** | Unknown — 尚未直接接触。渠道伙伴提到他 "对现有架构有些不满"，但具体不满点不清楚。 `[待确认 — 首次会议重点观察对象]` |
| **What They Care About** | *← CXO Persona: Director of Engineering (Platform)* — 架构可扩展性和长期演进路径；多云/混合云互操作性；数据治理和血缘追踪；平台自服务能力（让算法团队自己跑 pipeline）；技术债务偿还路径。Agent focus: 本次 opp 重点是**架构可扩展性 + 数据治理**，如果他对现有阿里云架构不满，这是我们的切入点。 |
| **Profiling** | *← Contact Profiling (initial, from public info)* — 前字节跳动基础架构部 Tech Lead，2024 年初加入理想。在字节时负责过 PB 级数据湖建设（Iceberg on HDFS → cloud migration）。GitHub 上有开源贡献（Apache Iceberg committer）。技术社区活跃，InfoQ 上发表过 "车企数据平台演进" 文章。推测：对开放标准（Iceberg, Parquet）有强偏好，可能对 vendor lock-in 敏感。 `[待确认 — 需要在首次会议验证技术偏好和对 AWS 的态度]` |
| **What We Need From Them** | 当前技术栈全貌；现有架构的具体痛点；评估标准和权重；对 AWS 的先入印象 |
| **How to Win Them** | SA 李珊 lead 深度技术对话。强调开放架构：S3 + Iceberg (open table format) + Lake Formation — 不锁定，可以跟任何 compute engine 配合。如果确认他是 Iceberg committer，这是天然连接点。准备一个 "从阿里云 MaxCompute 到 S3+Iceberg 的渐进迁移路径" 话题 — 不是全量搬迁，而是增量场景先跑。 |

**周小林 (Zhou Xiaolin)** — Data Engineering Manager (数据工程经理)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Important |
| **Role in This Deal** | Influencer / Day-to-day Implementer — 带领 15 人数据工程团队，是智驾数据 pipeline 的实际构建者和运维者。他的配合度直接决定 POC 和迁移速度。 |
| **Current Stance** | Unknown — 可能对多云评估持实用主义态度（"哪个好用就用哪个"），但也可能对迁移工作量有顾虑。 `[待确认]` |
| **What They Care About** | 数据 pipeline 的稳定性和可观测性；工具链成熟度（Spark, Flink, Airflow 等）；迁移对团队的工作量影响；学习曲线和培训支持；on-call 负担是否减轻 |
| **Profiling** | `[待确认 — 尚无公开信息。建议在首次会议中观察其参与度和技术关注点，构建初步画像。推测：作为 manager 级别的实操者，会更关注 "我的团队要做什么" 而非战略层面。]` |
| **What We Need From Them** | 数据规模细节（日增量、存储量、查询模式）；现有 pipeline 的具体痛点；团队技能分布（熟悉哪些工具） |
| **How to Win Them** | 不要在第一次会议过度 engage — 他的级别决定了先观察再跟进。但如果他主动发问，SA 要充分回应。后续如果进入 POC，他是关键执行人，需要单独安排一次 hands-on workshop。降低他对迁移工作量的恐惧是关键 — 强调 "增量试点，不动存量" 的策略。 |

*Engagement sequence rationale: 郎咸朋是 Economic Buyer 且同意了首次会面 → 先通过技术深度赢得他的初步认可 → 同时重点发展孙浩为 Champion（技术选型他说了算，且可能对现有架构不满）→ 周小林在 POC 阶段深度参与。VP 级别需要 3-4 次 meeting，Director 级别 2-3 次。*
*建议顺序，请确认。*

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1 (May 13) | First meeting: validate pain, understand multi-cloud evaluation process, build rapport | VP 郎咸朋, Dir 孙浩, Mgr 周小林 | **Next** ↓ |
| 2 | Week 3 (May 27) | Technical deep-dive: current architecture review + target state design (data lake + training pipeline) | Dir 孙浩, Mgr 周小林, (+郎咸朋 optional) | Planned |
| 3 | Week 5 (Jun 10) | POC scope co-definition + success criteria alignment | Dir 孙浩, Mgr 周小林 | Planned |
| 4 | Week 6-9 (Jun 17 - Jul 8) | POC execution: 1 路测数据集 → S3 data lake → model training pipeline | Mgr 周小林 (execution), Dir 孙浩 (review) | Planned |
| 5 | Week 10 (Jul 15) | POC results review + business case for VP | VP 郎咸朋, Dir 孙浩 | Planned |
| 6 | Week 12 (Jul 29) | Commercial discussion: pricing, PPA structure, OTA scope expansion | VP 郎咸朋, Procurement `[待确认]` | Planned |
| 7 | Week 14-16 (Aug-Sep) | Contract negotiation + legal review | VP 郎咸朋, Legal, Procurement | Planned |

> *Status: **Next ↓** (detailed below) · **Planned** · **Done** · **Skipped***

---

### Next Milestone Detail

**Milestone #1** — Target Date: Week 1 (May 13, 2026)

**Objective:** Validate pain points (data backfill latency, cost), understand multi-cloud evaluation process, build initial trust through technical depth

**Customer Attendees & Target Outcome:**
- **VP 郎咸朋** — build rapport, confirm multi-cloud evaluation is real (not just price benchmarking); understand his vision for 智驾数据闭环; agree that technical deep-dive is worthwhile
- **Dir 孙浩** — begin technical relationship; understand current architecture pain points; gauge openness to AWS; identify if he could be Champion
- **Mgr 周小林** — understand team composition and day-to-day operational pain; get a sense of data scale and pipeline complexity

**AWS Team:** AE 张磊 (Lead), SA 李珊 (Support), Automotive SA Specialist 陈航 (SME)

**Suggested Discovery Questions:**
1. 目前智驾数据从路测车辆回传到标注完成、进入训练，端到端需要多长时间？你们内部对这个速度满意吗？ *(Metrics, Implicated Pain)*
2. 这次多云评估的触发点是什么？是成本、性能、还是战略层面的考虑？技术委员会的评估标准已经定了吗？ *(Decision Process, Decision Criteria)*
3. 如果年底之前数据闭环的速度没有显著提升，对明年的智驾 OTA 推送节奏会有什么影响？ *(Compelling Event, Economic Buyer pressure)*
4. 除了你们三位，还有谁会参与这次多云评估的最终决策？CTO 或 CEO 会直接参与吗？ *(Decision Process, Champion mapping)*
5. 你们现在的数据湖架构是基于什么技术栈？最大的痛点是什么 — 是性能、成本，还是运维复杂度？ *(Technical, Implicated Pain)*
6. 智驾团队现在有多少数据？日增量大概多少？未来 12 个月的增长预期是什么？ *(Metrics, sizing for proposal)*

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 5 | 9 |
| **Timeline** | 14 weeks (Sep close) | 22 weeks (Nov close) |

**What could change:**
- 多云评估如果只是 price benchmark（无真实切换意图），整个 opp 可能是 tire-kicking — 首次会议必须验证
- 孙浩如果对 vendor lock-in 极度敏感，可能推动 "只用 S3 存储，不用 SageMaker" — 会压缩 deal size
- 阿里云如果提供大幅折扣续约（常见防守策略），可能削弱多云动力
- 郎咸朋如果不是最终 budget owner（需要 CTO/CEO 审批），决策链会拉长 2-4 周
- POC 如果涉及真实路测数据（含地图信息），可能触发数据合规审批，增加 4-6 周

---

## 3. Execution Log

> *Auto-updated after each Call Plan + PMR. Most recent at top.*

*No entries yet — first visit pending.*

---

*Engagement Plan Template | Version: 1.1*
