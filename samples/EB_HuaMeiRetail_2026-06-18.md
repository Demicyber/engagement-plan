# Executive Briefing Document — 华美零售 (HuaMei Retail)

> **INTERNAL USE ONLY** — AWS Confidential
>
> Internal leadership briefing — AWS SVP Sales 加入 Technical Validation 关键会议
>
> - **Internal leadership briefing** → This is the sole preparation document

---

## 1. Meeting Logistics

| Field | Details |
|---|---|
| **Date / Time / Format** | 2026-06-18 / 14:00-16:00 CST / In-person / 华美零售总部，上海市浦东新区陆家嘴环路 1000 号 |
| **AWS Attendees** | 赵总 (AWS GCR SVP Sales), AE 吴迪, SA 郑一凡, AI/ML SA Specialist 黄磊 |
| **Current Sales Stage** | Technical Validation |

**Who requested this meeting and why?**

> Account team 请求 AWS GCR SVP Sales 赵总参加此次 Technical Validation 会议。原因：华美零售 CEO 方明亲自参与技术评估会（不常见），表明此项目被列为集团战略级优先事项。客户 CTO 暗示 "CEO 想看看 AWS 的重视程度"。赵总的出席能传递 "AWS 高度重视这个合作" 的信号。

| Role | Name / Contact | Notes |
|---|---|---|
| **Account Manager** | 吴迪, @wudi, 139-xxxx-8888 | 负责华美零售 2 年，跟 CTO 和 CDO 关系稳固 |
| **Sales Leader** | 刘总 (GCR Enterprise East Director), @liuzong | 参与过初期 deal review |
| **Executive Sponsor** | 赵总 (AWS GCR SVP Sales), @zhaozong | 首次参与该客户，需要 full briefing |

---

## 2. Customer Attendee Background

### Attendees

**方明 (Fang Ming)** — CEO

> *1. **Position & Tenure** — 2020 年从宝洁中国区 VP 跳槽加入华美零售任 CEO。MBA（INSEAD）。在华美推动了 "数据驱动零售" 战略，上任后三年内线上收入占比从 12% 提升到 35%。向集团董事长汇报。*
>
> *2. **Communication Style** — CXO Persona (CEO): 战略导向，关注市场竞争格局和增长引擎。Contact Profiling: 方明个人风格偏外企文化 — 流利英语，喜欢用数据和 benchmark 说话，偏好结构化的讨论（framework > free-form）。高管出身，对 peer-level 对话有期待 — 如果 AWS 只派 AE 和 SA 来，他会觉得不够重视。这也是本次安排赵总出席的原因。不喜欢被 "教育" — 他要的是平等讨论，不是 vendor pitch。*
>
> *3. **Decision Role & Business Focus** — 最终决策者。当前三大优先：(1) 全渠道库存优化（core to this opp）, (2) 自有品牌增长, (3) 下沉市场扩张。CXO Persona: CEO 级关注 revenue growth, market share, competitive differentiation。本次 opp focus: 全渠道库存优化 — AI demand forecasting 直接影响他的 #1 priority。*
>
> *4. **Attitude Toward AWS** — Positive-leaning。方明在宝洁时期用过 AWS（全球 supply chain analytics 跑在 AWS 上），有正面记忆。但到华美后发现公司现有 IT 以阿里云为主（历史原因），对 "多云策略" 持开放态度。他不会因为个人偏好选 AWS — 需要看到明确的 "为什么 AWS 做这件事比阿里云好" 的证据。 `[Updated: 2026-06-10 — 从 CDO 沟通中获知]`*
>
> *5. **Collaboration History** — 无直接 AWS 接触记录。本次是第一次正式参与 AWS 相关会议。*

**周海波 (Zhou Haibo)** — CTO

> *1. **Position & Tenure** — 2018 年加入华美零售，此前在京东技术团队任架构总监。负责华美全部 IT 基础设施和技术架构。*
>
> *2. **Communication Style** — CXO Persona (CTO): 技术深度驱动，重视架构可扩展性。Contact Profiling: 京东技术背景让他对大规模分布式系统有极高标准。不喜欢 "小而美" 的 demo — 他关心的是 "100 万 SKU × 500 家门店的规模能不能扛住"。开会时会直接打断技术细节不对的地方。对 vendor 的态度比较冷 — 需要用技术实力赢得尊重。跟 CDO 配合紧密。 `[Updated: 2026-06-10]`*
>
> *3. **Decision Role & Business Focus** — 技术方案最终拍板。负责基础设施和平台层，AI/ML 的实际部署归他管（虽然需求端由 CDO 驱动）。*
>
> *4. **Attitude Toward AWS** — Neutral-to-Cautious。现有 IT 全在阿里云上，迁移成本是他的顾虑。不反对 AWS，但需要看到 "增量价值" — 不是替换阿里云，而是 AWS 能做阿里云做不了的事。 `[Updated: 2026-06-10]`*
>
> *5. **Collaboration History** — Week 3 technical deep-dive 参与。SA 郑一凡与他有过 3 次技术沟通，关系在建立中。他在 deep-dive 后评价 "AWS 的 SageMaker 确实比阿里云 PAI 成熟"。*

**孙莉 (Sun Li)** — CDO (Chief Data Officer)

> *1. **Position & Tenure** — 2022 年新设 CDO 岗位，从内部提拔（原 VP Data Analytics）。负责全公司数据战略和 AI 应用。*
>
> *2. **Communication Style** — Contact Profiling: 数据人出身，偏好看实验结果和 A/B 测试数据。对 "AI 能做什么" 的 vision 很兴奋，但对 "AI 落地有多难" 有清醒认识。是 CEO 和 CTO 之间的桥梁 — 能把技术语言翻译成商业语言。开会时话不多但提的问题往往最关键。*
>
> *3. **Decision Role & Business Focus** — Champion。这个项目的发起人。AI demand forecasting 是她的 OKR，成败直接影响她的年度评价。*
>
> *4. **Attitude Toward AWS** — Strongly Supportive。在技术评估中明确表示 "SageMaker 的 MLOps 比 PAI 好用"。已在内部为 AWS 方案背书。 `[Updated: 2026-06-10]`*
>
> *5. **Collaboration History** — 全程参与从 Week 1 开始的所有会议。与 AE 吴迪和 AI/ML SA 黄磊建立了良好关系。*

### Company Profile

> 华美零售成立于 2005 年，是中国领先的连锁零售企业，拥有 500+ 门店覆盖华东和华南，2025 年营收 ¥320 亿，员工 45,000 人，SKU 超过 100 万。公司正在推进 "智慧零售" 战略，重点投资 AI/ML 驱动的库存优化和个性化推荐。AI 采用处于快速增长期 — 数据团队 60 人，已有基础的分析能力但 ML 工程化不成熟。云使用以阿里云为主（约 ¥3,000 万/年），主要是电商平台和数据仓库。2026 年关键事件：全渠道库存优化被列为集团 #1 战略项目；下半年计划新开 80 家下沉市场门店（库存预测更关键）。CEO 方明上任后推动的 "数据驱动零售" 战略进入第二阶段。

---

## 3. Meeting Objectives

### Success Definition

> CEO 方明在会后确认 AI demand forecasting 项目使用 AWS 作为首选平台，并授权团队进入 POC 阶段。

### Strategic Alignment

> 这是 Technical Validation 阶段的关键会议。之前的 technical deep-dive 已经获得 CTO 和 CDO 的技术认可。CEO 本次亲自参与表明这是集团战略级项目 — 他需要在技术评估阶段看到 AWS 的技术深度和战略重视程度，才会在后续预算讨论中倾向 AWS。

### Objective 1:

| Element | Content |
|---|---|
| **Objective / Outcome** | 展示 AWS AI/ML 在零售 demand forecasting 的技术深度和差异化优势，获得 CEO 对方向的认可 |
| **Context** | CTO 和 CDO 已在 technical deep-dive 中认可 SageMaker > 阿里云 PAI。但 CEO 还没有看到具体方案。CEO 是数据驱动决策者（宝洁背景），需要看到 benchmark 和同行案例，不接受 "我们更好" 的空话。阿里云作为现有供应商，有惯性优势（"不迁移就是最低风险选项"）。 |
| **Talking Points** | 1. AWS 全球零售行业客户案例：Walmart、Carrefour 的 demand forecasting（准确率提升 15-30%）<br>2. SageMaker vs PAI 的具体对比：AutoML pipeline、built-in algorithms for time series、A/B testing framework<br>3. 华美场景分析：100 万 SKU × 500 门店的规模下，AWS 架构如何支撑（这是 CTO 最关心的）<br>4. "不是替换阿里云，是做阿里云做不了的事" — multi-cloud 定位 |
| **Asks** | **赵总 (AWS GCR SVP Sales) 问方明：**<br>"华美的全渠道库存优化在你的战略里是什么位置？如果 AI demand forecasting 能将库存周转提升 20%，对华美意味着什么？" *(引导 CEO 自己量化价值)* |

### Objective 2:

| Element | Content |
|---|---|
| **Objective / Outcome** | 获得 CEO 授权进入 POC 阶段，确认 POC scope 和 timeline |
| **Context** | CDO 孙莉已经准备了 POC proposal（华东 50 家门店 × 1000 SKU，4 周），CTO 周海波原则同意。需要 CEO sign-off 才能正式启动。CEO 对 POC 的期望可能高于技术团队 — 他可能问 "为什么不直接全量" 或 "4 周太长"。 |
| **Talking Points** | 1. POC scope 的合理性 — "先验证算法准确率，再扩展规模" 是行业最佳实践<br>2. POC 成功标准：demand forecast accuracy 提升 >15%（vs 现有规则引擎），库存周转天数改善<br>3. POC → Production 的路径清晰：4 周 POC → 2 周评估 → 12 周 production rollout（如果 POC 成功） |
| **Asks** | **赵总 (AWS GCR SVP Sales) 问方明：**<br>"如果 POC 结果达标，您这边需要什么才能做 go/no-go 决策？我们想确保 POC 设计对齐您的期望。" |

---

## 4. AWS Account Background

| Field | Details |
|---|---|
| **Geo / Segment** | GCR / Enterprise |
| **Current AWS Spend** | $8K (FY2026 YTD) — SA team 的 POC prep 用量 |
| **Expected Spend** | $1.2M ARR (AI/ML workloads, if won) |
| **Commit / PPA Status** | No existing PPA. Would be first AWS commercial engagement. |

### Account Summary

> *1. **AWS Usage** — 目前仅 SA 团队在 sandbox 环境做 POC prep（SageMaker training experiments + S3）。生产工作负载全在阿里云（电商平台、数据仓库 MaxCompute、推荐系统 PAI）。AI/ML 是 AWS 切入点。*
>
> *2. **PPA / Commercial** — 无现有承诺。阿里云有 3 年 PPA（¥3,000 万/年，2027 年 Q1 到期）。本次 AWS deal 是**增量**而非替换 — multi-cloud positioning。*
>
> *3. **Recent Wins / Momentum** — Technical deep-dive 获得 CTO "SageMaker 比 PAI 成熟" 的正面评价。CDO 成为强力 Champion。CEO 亲自参与本次技术评估会 — 非常正面的信号。*
>
> *4. **Issues / Concerns** — 阿里云客户经理已察觉 AWS 在接触华美，据 CDO 透露 "阿里云最近突然变得很积极，主动提供了 AI 能力升级方案"。需要关注阿里云的反制策略。另外，CTO 对 multi-cloud 的运维复杂度有顾虑。*
>
> *5. **Competitive Landscape** — 阿里云是现有供应商（全栈，¥3,000 万/年）。优势：既有关系 + 数据已在阿里云 + 运维团队熟悉。劣势：PAI 在 MLOps 成熟度上不如 SageMaker，demand forecasting 的行业案例深度不如 AWS（全球 vs 中国本地）。华为云未在 picture。我们的定位：不替换阿里云，AWS 做 AI/ML 增量 — "用 AWS 做阿里云做不了的事"。*

---

## 5. Appendix

### A. Previous Meeting Notes & Action Items

| Date | Meeting | Key Outcomes | Open Action Items |
|---|---|---|---|
| May 5 | First visit (CDO + CTO) | Pain validated (库存周转天数 45 天 vs 行业 30 天), CDO confirmed as Champion | ✅ All closed |
| May 19 | Technical deep-dive (CTO + CDO + Data team) | SageMaker MLOps 获认可, POC scope 初步讨论 | ✅ All closed |
| Jun 10 | CDO 1-on-1 follow-up | CEO 将参加下次会议, 阿里云开始反制 | ✅ All closed (this EB is the follow-up) |

### B. Relevant Customer Success Stories

> **Carrefour (家乐福) AI Demand Forecasting** — 全球 12,000+ 门店，使用 AWS SageMaker 部署 AI demand forecasting。库存准确率提升 25%，库存周转天数从 42 天降至 31 天，年减少食品浪费 ¥2 亿+。关键成功因素：SageMaker Autopilot 快速迭代 + 与现有 ERP 集成。
>
> **永辉超市 AI 补货** — 中国超市连锁，1000+ 门店。使用 AWS 部署 AI 自动补货系统，SKU 缺货率下降 35%，库存成本降低 18%。从 POC 到生产上线 10 周。

### C. Competitive Intelligence

> **阿里云：**
> - **Products in use:** ECS, MaxCompute (数据仓库), PAI (AI平台), OSS, RDS — 全栈
> - **Contract status:** 3 年 PPA, ¥3,000 万/年, 2027 Q1 到期。lock-in 中等 — 数据在 MaxCompute 里，迁移有成本
> - **Customer satisfaction:** CTO 对基础设施满意，对 PAI 的 AI/ML 能力不满意（"功能有但不好用"）。CDO 直接说 "PAI 的 MLOps 不行"
> - **Recent move:** 察觉 AWS 接触后变得积极，主动提供 AI 能力升级方案（据 CDO 透露）。需要关注后续动作
> - **Our differentiators:** SageMaker MLOps 成熟度（pipeline, model registry, A/B testing）; 全球零售 AI 案例深度（Walmart, Carrefour, 永辉）; demand forecasting 专项算法; AWS 不争夺阿里云存量，聚焦 AI/ML 增量
> - **Strategy:** Multi-cloud 共存。AWS 做 AI/ML 工作负载，阿里云保留基础 IaaS 和数据仓库。长期随着 PPA 到期（2027 Q1），可以讨论更多工作负载迁移

---

*Executive Briefing Template | Version: 1.1 | INTERNAL USE ONLY*
