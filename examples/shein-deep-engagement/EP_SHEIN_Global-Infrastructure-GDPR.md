# Engagement Plan: SHEIN - Global Infrastructure Optimization + GDPR Compliance

> **What is this?** A focused action plan for winning a specific opportunity. Answers: who do I need to win, what do I need from each person, and what's my engagement roadmap to get there?
>
> 🤖 *Automatically generated. Updated after each visit.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise.*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | SHEIN (希音) |
| **Opportunity Name** | Global CDN Optimization + Recommendation System + GDPR Compliance |
| **Deal Value** | $3.2M ARR |
| **Current Stage** | Business Validation |
| **Target Close Date** | 2026-Q3 |
| **Why Now** | EU Digital Services Act enforcement deadlines tightening (Q4 2026 full compliance required). SHEIN's current GDPR infrastructure spans 3 clouds with inconsistent data residency controls — EU regulators issued a formal inquiry letter in March 2026. Board-level mandate to resolve before next earnings call. |
| **Deal Objective** | Sign $3.2M PPA covering: (1) CloudFront global CDN consolidation, (2) SageMaker-powered recommendation engine with EU data isolation, (3) GDPR-compliant data architecture on AWS with automated DPA enforcement. |

### Win Strategy

SHEIN 的核心痛点是 GDPR 合规的紧迫性（EU 监管正式问询 + 董事会压力）叠加全球基础设施碎片化（3 朵云、数据治理不一致）。我们的 win theme 是 **"一个平台解决三个问题" — 用 AWS 的全球基础设施统一 CDN + 推荐系统 + GDPR 合规，而不是继续用 point solutions 打补丁**。具体差异化：AWS 在欧洲有 8 个 Region（法兰克福、爱尔兰、巴黎等）+ AWS Clean Rooms + Macie + Lake Formation 的数据治理组合拳，能提供 end-to-end 的数据驻留和自动化合规审计能力。Google Cloud 正在以 "GDPR-native" 定位争夺合规工作负载，但他们在亚太 CDN 覆盖和推荐系统（SageMaker vs Vertex AI）上劣于 AWS。我们的策略：**把 GDPR 合规和 CDN/推荐捆绑为一个整体方案，让 Google Cloud 无法单点突破合规场景**。

---

## 2. Engagement Plan

> *Pull stance and relationship history from **Contact Profiling Skill**. For executive-level (C-suite/VP), also pull role-level priorities and pain points from **CXO Personas**. Do NOT include people who are not involved in this opportunity.*

### Key Stakeholders

**Chu-Cheng Hsieh (谢楚政)** — CTO

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Economic Buyer + Technical Decision Maker — CTO 直接管理技术预算，$2M+ 投资需要他签字。也是技术路线最终拍板人。 |
| **Current Stance** | Supportive `[Updated: 2026-05-07]` — 前 4 次会议全程参与，在第 3 次 tech deep-dive 后明确表达 "AWS 方案是最完整的"。但对 timeline 有压力（"董事会要 Q3 看到进展"），同时受到 Google Cloud 的积极 approach（Google 的 EMEA VP 亲自给他打过电话）。 |
| **What They Care About** | *← CXO Persona: CTO (E-commerce/Fast Fashion context)* — Global infrastructure reliability (99.99% uptime SLA); cost-efficiency at massive scale (SHEIN 日均 5 亿次 API 调用); regulatory compliance as a board-level risk item; platform consolidation to reduce operational complexity; vendor diversification (not putting all eggs in one basket). Agent focus: 本次 opp 重点是 **GDPR 合规紧迫性 + 平台统一化的运维效率**。 |
| **Profiling** | *← Contact Profiling* `[Updated: 2026-05-07]` — PhD Computer Science (UCLA). 15+ years in digital transformation and e-commerce technology. Prior: VP of Engineering → Chief Data Officer at Etsy (headed data division — engineering, data science, ML). 现任 SHEIN (US) CTO，leads technology vision and engineering teams。决策风格快但要数据支撑 — 典型的 "show me the benchmark, then I decide fast"。开会时 multitask（看手机处理 Slack），但关键决策点会突然聚焦，提出非常尖锐的问题。偏好 30 分钟高效会议。跟 SA 李珊建立了较好的技术信任关系（第 2 次会议后开始直接 WeChat 问技术问题）。对竞争情报敏感 — 第 4 次会议主动告知 Google Cloud 在接触，说 "你们得给我一个理由不选他们做 GDPR 那块"。跟 Head of Infra 张锐关系密切（前同事），张锐的意见对他有很大影响。 |
| **What We Need From Them** | GDPR 工作负载 timeline 承诺 + 授权团队进入合同谈判 + 明确告知 Google Cloud 竞争的最新状态 |
| **How to Win Them** | 用 "统一平台 vs 多云碎片化" 的 TCO 和运维复杂度数据打动他。准备一份 AWS vs Google Cloud 在 GDPR 场景的详细对比（不攻击 Google，用差异化数据说话）。关键：要有欧洲客户参考案例（ASOS 或 Zalando 级别的电商 GDPR 案例）来回应他 "给我一个理由" 的挑战。AE lead 商务对话，SA 提供技术 backup。下次会议要 tight — 30 分钟议程，不浪费他时间。 |

**张锐 (Ray Zhang)** — Head of Infrastructure

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Technical Champion — 基础设施最终负责人，CDN 和推荐系统的直接 owner。他的技术评估决定了方案选型。 |
| **Current Stance** | Strongly Supportive `[Updated: 2026-04-23]` — 从第 1 次会议就对 AWS 方案高度认可。在内部多次为 AWS 背书（Chu-Cheng 透露 "张锐说你们的 CDN 方案是他评估过最好的"）。但他对 GDPR 部分的安全 SA 方案还在做最终确认。 |
| **What They Care About** | CDN 全球覆盖和性能（亚太 + 欧洲 latency 目标 <50ms）; 推荐系统训练/推理成本优化; 基础设施统一管理（当前 3 朵云运维团队疲惫不堪）; 容灾和高可用 |
| **Profiling** | *← Contact Profiling* `[Updated: 2026-04-23]` — Chu-Cheng 的前同事，2020 年一起跳到 SHEIN。Deep tech background（前 Facebook Infra），对架构细节有极强掌控欲。开会时话不多但每次发言都 cut to the point。偏好看架构图和 benchmark 数据，对 "概念性讨论" 没耐心。跟 SA 李珊建立了很好的技术关系（第 3 次 deep-dive 后给李珊发了一份内部架构文档 "帮我看看怎么对接"）。为人低调但在内部技术评审有一票否决权。对 Google Cloud 的态度比较 neutral — 认为 "Google 的 network 确实不错，但 managed service 生态不如 AWS"。 |
| **What We Need From Them** | 技术方案最终 sign-off（特别是 GDPR 数据隔离架构） + 帮我们在内部推动 timeline |
| **How to Win Them** | 已经赢了大半。这次会议重点：Security Specialist SA 陈晨给他做 GDPR 数据隔离架构的最终确认（Macie + Lake Formation + Clean Rooms 的具体部署方案）。准备一份详细的 EU 数据驻留架构图，标注每个数据流的合规边界。让他彻底放心后，他会帮我们在内部推 CTO 做决定。 |

**李莎 (Sarah Li)** — GDPR Compliance Lead

| Dimension | Details |
|---|---|
| **Engagement Priority** | Important |
| **Role in This Deal** | Compliance Gatekeeper — GDPR 合规方案必须经过她的评审和签字。虽然不做技术选型，但有否决权（"合规不过，方案不上"）。 |
| **Current Stance** | Cautious-Positive `[Updated: 2026-05-07]` — 第 3 次会议首次参与，对 AWS 的合规能力有正面印象但要求看 "实际运行的欧洲客户案例"。第 4 次会议上追问了 DPA（Data Processing Agreement）的具体条款，对 AWS 的标准 DPA 有两个具体修改要求。法律团队给她的压力是 "不能出任何合规风险"。 |
| **What They Care About** | EU 数据驻留的法律保证（不只是技术保证）; DPA 条款的灵活性; 自动化合规审计和报告能力; 出事后的响应 SLA; 参考客户案例（同行业、同规模） |
| **Profiling** | *← Contact Profiling* `[Updated: 2026-05-07]` — 法律背景（曾在 Baker McKenzie 做数据隐私律师 5 年），2023 年加入 SHEIN 组建合规团队。非常注重细节，每次会议都会带一份 checklist 逐项确认。不关心技术实现只关心法律结果 — "我不在乎用什么服务，我在乎合规报告能不能自动生成、能不能在审计时直接提交"。对 AWS 和 Google Cloud 都持 "证明给我看" 的态度。第 4 次会议后跟 AE 张磊说："AWS 的技术我大概信了，但我需要看一个欧洲电商的活案例 — 有没有人已经用 AWS 通过了 EU DPA 审计的？" |
| **What We Need From Them** | GDPR 方案合规 sign-off + 不被竞争对手 flip（Google Cloud 在 GDPR 领域有 narrative 优势） |
| **How to Win Them** | 给她想要的：一个活的欧洲电商参考案例。已经联系了 ASOS 的 compliance team，确认他们愿意做 reference call（待最终确认日期）。这次会议重点：呈现 AWS GDPR Reference Architecture + DPA 条款修改方案 + 告知 reference call 安排。Security SA 陈晨 lead 合规讨论。 |

*Engagement sequence rationale: 张锐（Technical Champion）已经在我们这边，持续用他推动内部进程。Chu-Cheng（CTO/Economic Buyer）是最终决策人，需要在这次会议确认 timeline。李莎（Compliance Gatekeeper）是当前 blocker — 她的 reference case 需求必须在这次会议给出明确回应，否则 timeline 会被拖延。策略：先满足李莎的合规关切 → 解除 blocker → Chu-Cheng 才能 commit timeline。*

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1 (Mar 5) | First meeting: validate pain, understand multi-cloud challenges, confirm opportunity scope | CTO Chu-Cheng, Head of Infra 张锐 | **Done** |
| 2 | Week 3 (Mar 19) | CDN + Recommendation deep-dive, benchmark AWS vs current setup | CTO Chu-Cheng, 张锐, Infra team | **Done** |
| 3 | Week 6 (Apr 9) | GDPR architecture workshop + Security deep-dive, introduce 李莎 | CTO Chu-Cheng, 张锐, 李莎 | **Done** |
| 4 | Week 9 (Apr 23) | Technical validation complete; DPA review with legal; confirm deal structure | CTO Chu-Cheng, 张锐, 李莎 | **Done** |
| 5 | Week 12 (May 21) | Push for timeline commitment; address compliance blockers; competitive response | CTO Chu-Cheng, 张锐, 李莎 | **Next** ↓ |
| 6 | Week 14 (Jun 4) | Reference call (ASOS/EU customer) + final compliance sign-off | 李莎 + legal team | Planned |
| 7 | Week 16 (Jun 18) | Commercial negotiation: PPA terms, pricing, payment structure | CTO Chu-Cheng, Procurement | Planned |
| 8 | Week 18-19 (Jul) | Contract execution + implementation kickoff | CTO Chu-Cheng, 张锐, Procurement | Planned |

> *Status: **Next ↓** (detailed below) · **Planned** · **Done** · **Skipped***

---

### Next Milestone Detail

**Milestone #5** — Target Date: Week 12 (May 21, 2026)

**Objective:** Secure timeline commitment from CTO; address 李莎's reference case requirement; provide competitive counter-positioning vs Google Cloud

**Customer Attendees & Target Outcome:**
- **CTO Chu-Cheng** — commit to PPA signing timeline (target: contract execution by end of June); confirm Google Cloud is not being awarded GDPR workload separately
- **张锐** — final technical sign-off on GDPR data isolation architecture; confirm implementation readiness
- **李莎** — accept the reference call arrangement (ASOS, June first week) as sufficient for her compliance evaluation; confirm no further legal blockers

**AWS Team:** AE 张磊 (Lead), SA 李珊 (Technical), Security Specialist SA 陈晨 (GDPR/Compliance)

**Key Questions for This Meeting:**
1. GDPR 工作负载的内部审批还有哪些步骤没走完？Legal team 的 sign-off 还差什么？ *(Blocker identification)*
2. Google Cloud 的提案目前走到什么阶段了？有没有在做技术评估？ *(Competitive intelligence)*
3. 如果 reference call 安排在 6 月第一周，李莎的评估 timeline 能对得上 Q3 目标吗？ *(Timeline alignment)*
4. 预算审批流程里还有谁需要 sign off？Procurement 是否已经 engaged？ *(Paper process)*
5. 如果 GDPR 方案先行、CDN/推荐整体打包签，这种分期落地方式是否可接受？ *(Deal structure flexibility)*

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 2 (this + final negotiation) | 5 (if compliance blocker persists) |
| **Timeline** | 8 weeks (Jul close) | 14 weeks (Sep close) |

**What could change:**
- 李莎如果不接受 ASOS reference call 作为充分证据，可能要求额外的合规审计（增加 4-6 周）
- Google Cloud 如果给出 aggressive pricing on GDPR-only scope，可能导致 split deal（我们拿 CDN/推荐，Google 拿 GDPR）— 这是最差结果
- CEO/Board 如果在下一次 earnings call 被问到 GDPR 进展，可能加速 timeline（利好）
- DPA 条款修改如果触发 AWS Legal 升级流程，增加 2-3 周内部审批
- SHEIN 的 Procurement 团队出了名的 aggressive on pricing — 商务谈判可能需要 2-3 轮

---

## 3. Execution Log

> *Auto-updated after each Call Plan + PMR. Most recent at top.*

| Date | Visit # | Key Outcome | Stage Change |
|---|---|---|---|
| 2026-04-23 | #4 | Technical validation 完成。张锐 sign off CDN + 推荐方案。李莎提出 reference case 需求和 DPA 修改请求。Chu-Cheng 首次透露 Google Cloud 竞争（"给我一个理由不选他们做 GDPR"）。 | Technical Validation → Business Validation |
| 2026-04-09 | #3 | GDPR architecture deep-dive 成功。李莎首次参与，对 Macie + Clean Rooms 方案初步认可但保留意见。张锐确认推荐系统 POC 结果（CTR 提升 12%，训练成本降 35%）。 | — (still Technical Validation) |
| 2026-03-19 | #2 | CDN benchmark 完成：CloudFront vs 现有方案 latency 降低 23%（亚太）。推荐系统 POC scope 确认。Chu-Cheng stance 从 Neutral 转向 Supportive。张锐开始直接跟 SA 李珊 WeChat 沟通。 | Prospect → Qualified |
| 2026-03-05 | #1 | 首次拜访成功。痛点验证：3 朵云运维复杂度 + GDPR 合规压力。Chu-Cheng 确认机会真实性。张锐表达对 AWS CDN 的强烈兴趣。Opportunity scope 从最初的 CDN-only 扩展到包含推荐和 GDPR。 | — (Prospect) |

---

*Engagement Plan Template | Version: 1.1*
