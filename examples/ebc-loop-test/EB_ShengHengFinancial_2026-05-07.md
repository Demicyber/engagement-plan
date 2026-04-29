# Executive Briefing Document: 盛恒金融 EBC

> **INTERNAL USE ONLY — AWS Confidential**
>
> 本文件为 AWS 内部高管准备材料，用于 2026-05-07 盛恒金融 EBC 会议。

---

## 1. Meeting Logistics

| Field | Details |
|---|---|
| **Date / Time / Format** | 2026-05-07（周三）/ 时间 [待确认] / In-person / 地点 [待确认] |
| **AWS Attendees** | 张总（AWS 大中华区总经理）、客户经理、SA |
| **Current Sales Stage** | Business Validation（POC 已完成） |

**Who requested this meeting and why?**

> 客户团队发起 EBC 邀请，目的是通过张总与盛恒金融 CEO 王建国的 CEO-to-CEO 对话，推动核心保险业务系统迁移至 AWS 的战略决策。盛恒金融是存量客户（年消费 $800K），但大部分工作负载在阿里云（约 $3M）。POC 已证明 AWS 在性能（+30%）和成本（-15%）上的优势，CTO 赵磊已是我们的 Champion，关键突破口是获取 CEO 的战略承诺。

| Role | Name / Contact | Notes |
|---|---|---|
| **Account Manager** | [待确认] | |
| **Sales Leader / VP** | [待确认] | |
| **Executive Sponsor** | 张总（AWS 大中华区总经理） | CEO-to-CEO 对话，与王建国同级别对等 |

---

## 2. Customer Attendee Background

### Attendees

**王建国**, CEO

> **Position & Tenure** — 盛恒金融 CEO，管理资产规模 5000亿+ 的大型保险集团。具体任职年限和职业背景 [待确认 — 建议客户团队补充，有助于张总建立个人连接]。
>
> **Communication Style** — *（CXO Persona: CEO）* 作为大型保险集团 CEO，预期沟通风格为战略导向、结果驱动。CEO 级别决策者通常关注全局战略和商业回报，而非技术细节。建议张总以 peer-to-peer 的方式、用商业语言（而非技术语言）沟通。CEO 决策的核心逻辑是资本配置——每一笔投入都在与其他投资选项竞争管理层注意力和资金。
>
> **Decision Role & Business Focus** — 最终决策者（Final Decision Maker），控制集团预算和战略方向。*（CXO Persona: CEO 优先级）* 预期关注：(1) 盈利性增长——保险行业利润率承压背景下的降本增效；(2) 战略简化——减少供应商复杂度、优化技术架构；(3) 数字化转型 ROI——核心系统现代化对业务竞争力的影响；(4) 风险管控——保险行业监管合规（银保监会）和数据安全是不可逾越的底线。
>
> **Attitude Toward AWS** — **Neutral / Wait-and-see**。CTO 赵磊已支持 AWS，但王建国尚未明确表态。盛恒金融主要工作负载在阿里云（$3M vs AWS $800K），说明王建国此前的战略倾向是阿里云。本次 EBC 是打破这一格局的关键窗口。*（CXO Persona: CEO 常见顾虑）* 预期关注点包括：迁移风险对业务连续性的影响、数据主权和合规（银保监会要求数据不出境）、供应商锁定风险。**避免话题：** 不要直接贬低阿里云——王建国选择阿里云是他过去的决策，攻击阿里云 = 质疑他的判断力。
>
> **Collaboration History** — 盛恒金融是 AWS 存量客户，年消费 $800K，但规模有限。具体合作历史和此前高管互动 [待确认 — 建议客户团队补充张总此前是否与王建国有过接触]。

---

**赵磊**, CTO

> **Position & Tenure** — 盛恒金融 CTO，主导了本次 POC 评估。具体任职年限和技术背景 [待确认]。
>
> **Communication Style** — *（CXO Persona: CTO）* 作为主导 POC 的技术负责人，预期沟通风格为数据驱动、重视技术细节和可行性论证。CTO 评估的核心逻辑是技术真实性——方案要么能落地，要么不能。赵磊在本次 EBC 中的角色是向 CEO 汇报 POC 结果，建议让他用数据说话。
>
> **Decision Role & Business Focus** — 技术决策推动者 / Champion。*（CXO Persona: CTO 优先级）* 预期关注：(1) 核心系统架构的先进性和可靠性——保险核心系统的稳定性直接影响业务运营；(2) 迁移过程中的技术风险和业务连续性保障；(3) 长期技术平台的可扩展性——支撑集团未来 3-5 年的数字化需求；(4) 团队工程效率提升——AWS 技术栈是否让技术团队更高效。
>
> **Attitude Toward AWS** — **Supportive**。赵磊主导了 POC，对 AWS 的技术能力有第一手认知（性能+30%、成本-15%）。他是我们在客户内部的核心盟友，在 EBC 中需要他用 POC 数据为 AWS 站台。
>
> **Collaboration History** — 与 AWS SA 团队在 POC 阶段有深度合作。具体协作细节 [待确认]。

### Company Profile

> **Positioning & Industry Standing** — 盛恒金融是中国大型保险集团，资产规模 5000亿+ 人民币，在中国保险市场具有重要地位。具体市场排名和业务构成（寿险/财险/资管等） [待确认]。
>
> **Scale & Impact** — 资产管理规模 5000亿+，具体年保费收入、客户数量和市场份额 [待确认 — 这些数据可帮助张总了解客户量级，建议从公开年报获取]。
>
> **Technology Profile** — 目前多云架构：阿里云为主力（约 $3M 年消费），AWS 为辅（$800K 年消费）。核心保险业务系统目前运行在 [待确认 — 阿里云/自建机房？]。POC 已验证 AWS 性能优于阿里云 30%、成本低 15%。AI 采用阶段 [待确认]。
>
> **Strategic Priorities & Key Events** — 核心保险业务系统现代化是当前战略焦点（本次 EBC 的核心议题）。保险行业数字化转型、AI 应用（智能理赔、智能核保等）是行业趋势。近期是否有其他重大战略动作（融资、并购、业务调整等） [待确认]。
>
> **Recent Leadership Changes** — [待确认 — 建议确认近 6 个月内是否有高管变动，可能影响决策链]。

---

## 3. Meeting Objectives

### Success Definition

> EBC 成功标志：王建国明确表态支持核心系统迁移至 AWS，给出迁移决策时间承诺，并授权团队推进下一步商务谈判。

### Strategic Alignment

> 本次 EBC 是盛恒金融机会推进的关键转折点。EP 中规划的第一个里程碑（Milestone #1）。如果 CEO 给出明确承诺，将直接加速从 Business Validation → Committed 的推进。CEO-to-CEO 对话是打破当前僵局（CTO 支持但 CEO 未表态）的最高杠杆动作。

### Objective 1: 获取 CEO 对核心系统迁移的战略承诺

| Element | Content |
|---|---|
| **Objective / Outcome** | 推动王建国从"观望"转变为"明确支持"核心保险业务系统迁移至 AWS |
| **Context** | 盛恒金融目前大部分工作负载在阿里云（$3M），AWS 仅 $800K。POC 已证明 AWS 性能优于阿里云 30%、成本低 15%——这是客户 CTO 已验证的硬数据。但 CEO 尚未表态，可能因为：(1) 迁移核心系统的风险顾虑（业务连续性）；(2) 现有阿里云关系的惯性；(3) 需要更高级别的战略对话来建立信任。竞争风险：阿里云可能在得知 POC 结果后发起防守（降价、高管拜访） |
| **Talking Points** | • "我们看到保险行业最优秀的公司都在用核心系统现代化来建立竞争优势。盛恒金融的 POC 结果证明了这个路径是可行的。"<br>• "AWS 在全球服务了 XX 家保险公司 [待确认 — 补充具体数据]，我们理解保险行业对安全、合规和业务连续性的极高要求。"<br>• "我个人承诺为盛恒金融的迁移提供全程支持，包括专属架构团队和合规团队的对接。"（张总的个人承诺增加信任感）<br>• "核心系统上云不仅是技术升级，也是为盛恒金融的 AI 战略打好基础——现代化的云架构是 AI 落地的前提。" |
| **Asks** | • **张总 → 王建国：** "王总，核心系统迁移在您今年的战略优先级中排在什么位置？您希望在什么时间范围内做出迁移决策？"<br>• **张总 → 王建国：** "如果我们在合规和数据主权方面能完全满足银保监会的要求，您还有其他顾虑吗？"<br>• **张总 → 王建国：** "盛恒金融在 AI 驱动的保险业务创新方面有什么规划？AWS 在这方面可以如何支持您？" |

### Objective 2: 确认商务谈判路径和时间线

| Element | Content |
|---|---|
| **Objective / Outcome** | 明确下一步商务谈判的参与人、流程和时间节点 |
| **Context** | 从 Business Validation 推进到合同签订，需要确认：(1) 谁参与商务谈判（CFO？采购？）；(2) 预算审批流程；(3) 合同签订的目标时间。这些信息目前均未确认 |
| **Talking Points** | • "赵磊总的 POC 报告给了我们很好的技术基础，接下来我们希望推进到商务讨论阶段。"<br>• "我们可以提供灵活的商务方案，包括 PPA（Private Pricing Agreement）和分阶段迁移的成本模型。" |
| **Asks** | • **客户经理 → 王建国/赵磊：** "下一步商务谈判，您这边需要哪些部门参与？我们可以尽快安排。"<br>• **张总 → 王建国：** "您认为什么时间启动商务谈判比较合适？" |

### Objective 3: 了解客户对 AI 及新技术的战略需求

| Element | Content |
|---|---|
| **Objective / Outcome** | 发掘 AI 及新技术方向的增量商机，为后续 upsell 铺路 |
| **Context** | 保险行业正在快速拥抱 AI（智能理赔、智能核保、风控等）。盛恒金融作为大型保险集团，可能有 AI 战略但尚未与 AWS 讨论过。核心系统迁移到 AWS 后，可以自然延伸到 AI/ML 场景，增加客户粘性和 deal size |
| **Talking Points** | • "我们看到全球领先的保险公司正在用 AI 重新定义理赔、核保和客户服务流程——有些已经实现了 XX% 的效率提升 [待确认 — 补充案例]。"<br>• "AWS 的 Amazon Bedrock 和 SageMaker 为保险行业提供了成熟的 AI 平台，可以帮助盛恒金融快速落地 AI 应用。" |
| **Asks** | • **张总 → 王建国：** "盛恒金融在 AI 驱动的保险业务创新方面有什么规划？" |

---

## 4. AWS Account Background

| Field | Details |
|---|---|
| **Geo / Segment** | GCR / Enterprise |
| **Current AWS Spend** | $800K（年消费） |
| **Expected Spend** | $2.8M+（如核心系统迁移成功：$800K 现有 + $2M 新增 ARR） |
| **Commit / PPA Status** | [待确认 — 是否有现有 PPA？] |

### Account Summary

> **AWS Usage** — 盛恒金融目前在 AWS 上的年消费为 $800K，具体工作负载类型 [待确认 — 可能是非核心应用、开发测试环境、或特定业务线]。核心保险业务系统目前不在 AWS 上。本次 deal 的目标是将核心系统迁移到 AWS，预计增加 $2M ARR。
>
> **PPA / Commercial** — 现有商务安排 [待确认]。如果迁移成功，建议推进 PPA 覆盖新增消费。
>
> **Recent Wins / Momentum** — POC 成功完成，结果优异（性能+30%、成本-15%）。CTO 赵磊已成为 Champion。EBC 会议已确认——这是高管层面的重大突破。
>
> **Issues / Concerns** — 客户大部分工作负载在阿里云（$3M），AWS 目前只是辅助角色。需要在本次 EBC 中改变这一格局。数据合规和银保监会监管要求可能是关键风险点。
>
> **Competitive Landscape** — **阿里云** 是主要竞争对手，目前占客户 $3M 年消费（vs AWS $800K）。阿里云是盛恒金融现有核心系统的主力供应商。POC 数据已证明 AWS 在核心系统场景下性能和成本优于阿里云。Win theme：**已验证的技术优势 + 全球保险行业经验 + CEO-to-CEO 信任背书**。

---

## 5. Appendix

### A. Previous Meeting Notes & Action Items

> [待确认 — 建议客户团队补充此前与盛恒金融的会议记录、POC 过程中的关键讨论和遗留 action items]

### B. Relevant Customer Success Stories

> **建议准备 1-2 个保险行业客户案例：**
> - 大型保险公司核心系统迁移至 AWS 的成功案例 [待确认 — 建议从 AWS 保险行业案例库中挑选，优先选择中国或亚太区案例]
> - 保险行业 AI 应用（智能理赔/核保）的成功案例 [待确认 — 用于 Objective 3 的 AI 话题]

### C. Competitive Intelligence

> **阿里云**
> - **Products in use** — 盛恒金融的主力云供应商，年消费约 $3M。具体使用的阿里云产品和服务 [待确认]
> - **Contract status** — 现有合同条款和到期时间 [待确认 — 这会影响迁移节奏]
> - **Customer satisfaction** — CTO 赵磊在 POC 后已认可 AWS 优于阿里云（核心系统场景）。CEO 王建国对阿里云的满意度 [待确认]
> - **Our differentiators** — POC 已验证：性能优于阿里云 30%、成本低 15%（核心保险系统场景）。全球保险行业经验和合规能力。Amazon Bedrock / SageMaker 在 AI 场景的成熟度
> - **Displacement / coexistence strategy** — 短期共存：核心系统迁移至 AWS，非核心可继续在阿里云。长期目标：随着更多工作负载验证 AWS 优势，逐步扩大 AWS 占比

---

*Executive Briefing | Version: 1.0 | Generated: 2026-04-29 | INTERNAL USE ONLY*
