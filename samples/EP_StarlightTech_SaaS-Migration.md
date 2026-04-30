# Engagement Plan: 星辰科技 (Starlight Tech) - SaaS Platform Cloud Migration

> **What is this?** A focused action plan for winning a specific opportunity.
>
> 🤖 *Auto-generated after Call Plan (Path B) — no prior EP existed.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise.*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | 星辰科技 (Starlight Tech) |
| **Opportunity Name** | SaaS Platform Cloud Migration |
| **Deal Value** | $650K ARR |
| **Current Stage** | Prospect |
| **Target Close Date** | 2026-Q3 |
| **Why Now** | 星辰科技的 SaaS 平台目前跑在 IDC 托管机房，去年两次宕机导致 SLA 违约，赔偿了客户 ¥200 万。董事会要求 Q3 前完成云迁移，确保 99.95% 可用性。 |
| **Deal Objective** | Sign $650K PPA by Q3 2026, migrate core SaaS platform to AWS with 99.95% SLA. |

### Win Strategy

星辰科技的核心痛点是 SaaS 平台稳定性导致的客户信任危机（两次宕机 → SLA 赔偿 → 客户流失风险）。Win theme：**AWS 的高可用架构（Multi-AZ + Auto Scaling）+ SaaS 行业最佳实践 + 迁移加速器（MAP）降低迁移风险**。竞争对手：阿里云是现有候选（客户内部有人推荐），但阿里云的 SaaS ISV 支持生态不如 AWS（缺少 SaaS Boost、Well-Architected SaaS Lens）。腾讯云在 SaaS 行业存在感弱。

---

## 2. Engagement Plan

### Key Stakeholders

**陈思远 (Chen Siyuan)** — CTO & Co-founder

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Champion + Technical Decision Maker — 联合创始人兼 CTO，技术架构最终拍板，也是最关注稳定性问题的人 |
| **Current Stance** | Supportive — 主动联系 AWS 询问迁移方案。但对迁移风险有顾虑（"不能再出事了"） *← from sales input* |
| **What They Care About** | *← CXO Persona: CTO (SaaS context)* — Platform reliability & SLA guarantees; migration risk mitigation (zero-downtime migration); multi-tenancy architecture best practices; cost predictability (SaaS margins are tight); DevOps maturity and CI/CD pipeline integration. Agent focus: 本次 opp 重点是 **reliability + migration risk**，SaaS multi-tenancy 和 DevOps 是加分项但不是决策关键。 |
| **Profiling** | *← Contact Profiling (initial, from sales input)* — 技术创始人，对架构细节有极强的掌控欲。开会时会不断追问 "如果 XXX 挂了怎么办" — 典型的 failure-scenario thinker。偏好看架构图和 failover demo，不喜欢纯商业 pitch。沟通风格直接，不喜欢绕弯。90 后，喜欢高效沟通（WeChat > email，30 分钟会议 > 1 小时）。 `[待确认 — 首次接触，需要在第一次会议中验证和补充]` |
| **What We Need From Them** | 确认迁移意愿 + 同意进入架构评估（Technical Validation）+ 内部推动 CEO 批预算 |
| **How to Win Them** | SA lead 架构讨论。重点演示 Multi-AZ failover 和 Auto Scaling。准备一个 SaaS 平台迁移的 failure scenario walkthrough（"如果数据库挂了，系统怎么自动恢复"）。带 SaaS ISV SA specialist。不要超过 30 分钟的 formal presentation — 快速进入技术对话。建议 2 次 meeting。 |

**林婉清 (Lin Wanqing)** — CEO & Co-founder

| Dimension | Details |
|---|---|
| **Engagement Priority** | Important |
| **Role in This Deal** | Economic Buyer — $500K 以上投资需要她签字。关注客户留存和公司增长，不参与技术决策但对投资回报很敏感。 |
| **Current Stance** | Neutral — 知道要迁移，但不确定 AWS vs 阿里云。她的 advisor 推荐了阿里云（"国内用阿里比较方便"）。 *← from sales input* |
| **What They Care About** | *← CXO Persona: CEO (SaaS startup context)* — Customer retention and NRR; SaaS unit economics (CAC, LTV, gross margin); platform credibility for enterprise clients; fundraising narrative ("we run on AWS" vs "we run on Alibaba Cloud" for Series B). Agent focus: 本次 opp 重点是 **customer retention（SLA 违约导致的流失风险）+ 品牌信号（AWS for enterprise credibility）**。 |
| **Profiling** | *← Contact Profiling (initial, from sales input)* — 商业背景，北大光华 MBA。决策风格偏理性分析 — 需要数据支撑，不接受 "大家都在用 AWS" 这种说法。对成本敏感但不是 cost-first thinker — 更看 ROI 和长期价值。她的 advisor 是前阿里云员工，需要注意这个影响力。 `[待确认 — 尚未直接接触，需要 AE 验证]` |
| **What We Need From Them** | 预算审批 + 对 AWS vs 阿里云的偏好转向 |
| **How to Win Them** | AE lead 商业对话。准备 SaaS 行业 benchmark：AWS 上的 SaaS 公司 vs 阿里云的 NPS、uptime 对比。用 "enterprise 客户更信任 AWS" 的 branding 角度（星辰科技正在拓展 enterprise 客户）。准备 MAP（Migration Acceleration Program）的 funding 优惠，降低她的成本顾虑。不直接攻击阿里云 — 用差异化而非贬低。建议在 CTO 技术认可后安排 1-on-1。 |

**王浩 (Wang Hao)** — VP Engineering

| Dimension | Details |
|---|---|
| **Engagement Priority** | Nice to Have (Prospect) → Important (Technical Validation) |
| **Role in This Deal** | Evaluator — 带领 8 人工程团队，迁移的实际执行者。他的配合度直接决定迁移速度。 |
| **Current Stance** | Unknown — CTO 提到他 "还在观望"，可能对迁移工作量有顾虑。 `[待确认 — 需要在 tech deep-dive 时了解]` |
| **What They Care About** | 迁移工作量和时间线、对现有 CI/CD pipeline 的影响、学习曲线、团队是否需要加人 |
| **Profiling** | `[待确认 — 尚未接触。建议在 Technical Validation 阶段开始构建画像。]` |
| **What We Need From Them** | 迁移方案配合 + 时间线承诺 |
| **How to Win Them** | Technical Validation 阶段再详细规划。初步策略：展示 AWS 的迁移工具链（MGN、DMS），强调 "不需要重写代码" 的迁移路径。如果可能，安排一次类似规模 SaaS 公司的迁移经验分享。 |

*Engagement sequence: CTO 陈思远是 Champion 且主动发起 → 先搞定技术认可 → 再通过 CTO 影响 CEO 的 AWS vs 阿里云判断 → VP Engineering 在 Technical Validation 阶段参与。*
*建议顺序，请确认。*

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1 (May 19) | First meeting: validate pain, understand decision process, confirm CTO as champion | CTO 陈思远 | **Next** ↓ |
| 2 | Week 3 (Jun 2) | Architecture assessment: current state → target state, migration approach | CTO 陈思远, VP Eng 王浩 | Planned |
| 3 | Week 5 (Jun 16) | CEO business case: ROI, MAP funding, AWS vs 阿里云 positioning | CEO 林婉清, CTO 陈思远 | Planned |
| 4 | Week 7-8 (Jun 30 - Jul 7) | POC: migrate non-prod environment, validate failover | CTO 陈思远, VP Eng 王浩 | Planned |
| 5 | Week 10 (Jul 21) | POC results + pricing proposal | CEO 林婉清, CTO 陈思远 | Planned |
| 6 | Week 12-14 (Aug) | Contract negotiation + PPA signing | CEO 林婉清, Finance | Planned |

---

### Next Milestone Detail

**Milestone #1** — Target Date: Week 1 (May 19, 2026)

**Objective:** Validate pain points, understand decision process, confirm CTO as champion

**Customer Attendees & Target Outcome:**
- **CTO 陈思远** — confirm as Champion; understand technical requirements and migration constraints; agree to architecture assessment as next step

**AWS Team:** AE 张磊 (Lead), SA 李珊 (Support)

**Suggested Discovery Questions:**
1. 去年两次宕机的根因是什么？是单点故障还是架构层面的问题？ *(Implicated Pain, Technical)*
2. 现在平台的架构是什么样的？数据库、应用层、缓存分别跑在哪里？ *(Technical baseline)*
3. 你们评估过阿里云吗？目前倾向如何？有没有已经做了 POC 或报价？ *(Competition, Decision Process)*
4. 迁移的决策谁来拍板？林总（CEO）在技术选型上参与多少？ *(Decision Process, Economic Buyer)*
5. 如果 Q3 前没有完成迁移，对公司有什么影响？会影响融资吗？ *(Compelling event, Metrics)*

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 5 | 8 |
| **Timeline** | 12 weeks (Aug close) | 18 weeks (Sep close) |

**What could change:**
- CEO 的 advisor 如果持续推阿里云，可能需要额外 1-2 次 meeting 做差异化对比
- VP Engineering 如果对迁移工作量有强烈抵触，需要额外时间解决
- 如果客户坚持要做 AWS vs 阿里云 bake-off，增加 3-4 周
- MAP funding 审批流程可能影响时间线

---

## 3. Execution Log(回滚)

*No entries yet — first visit pending.*

---

*Engagement Plan Template | Version: 1.1*
