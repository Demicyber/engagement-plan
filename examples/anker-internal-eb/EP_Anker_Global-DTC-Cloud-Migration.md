# Engagement Plan: Anker Innovations (安克创新) - Global DTC Cloud Migration & Data Analytics Platform

> **What is this?** A focused action plan for winning a specific opportunity. Answers: who do I need to win, what do I need from each person, and what's my engagement roadmap to get there?
>
> 🤖 *Automatically generated. Updated after each visit.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise.*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | Anker Innovations (安克创新) |
| **Opportunity Name** | Global DTC Cloud Migration + Supply Chain Analytics Platform |
| **Deal Value** | $2.1M ARR |
| **Current Stage** | Technical Validation |
| **Target Close Date** | 2026-Q3 |
| **Why Now** | Anker 正在从 Amazon 渠道依赖转向自建 DTC（anker.com + 独立站），2025 年 DTC 占比已从 8% 升至 18%，目标 2027 年达 35%。现有 Shopify + 多云拼凑架构在 Black Friday 2025 出现 3 次宕机，直接损失约 $2M GMV。同时全球 12 个仓的供应链数据分散在 5 个系统中，库存周转天数比行业标杆高 40%。CEO 要求 2026 年底前完成全球基础设施统一。 |
| **Deal Objective** | Sign $2.1M PPA by Q3 2026; migrate DTC platform to AWS (CloudFront + ECS + Aurora Global); deploy supply chain analytics on Redshift + SageMaker for demand forecasting. |

### Win Strategy

Anker 的核心痛点是 **DTC 高速增长暴露了基础设施的拼凑本质** — Shopify Plus + 阿里云国内 + Azure 部分海外 + 自建 IDC 的混合架构导致运维复杂度和宕机风险急剧上升。我们的 win theme：**AWS 全球化基础设施一致性（CloudFront 400+ PoP + Global Accelerator）+ 零售/DTC 行业最佳实践（SHEIN、Anker 竞品 Baseus 都在 AWS 上）+ 供应链 AI 能力（SageMaker demand forecasting，已有类似客户如 Cainiao 的案例）**。竞争对手阿里云在国内电商 infra 有存量优势但全球 CDN 覆盖和 DTC 独立站经验不足；Azure 有部分海外工作负载但 AI/ML 和零售行业解决方案弱于 AWS。关键差异化：全球一致的基础设施 + DTC 行业深度 + 供应链 AI 一站式方案（从数据入湖到预测到决策）。

---

## 2. Engagement Plan

> *Pull stance and relationship history from **Contact Profiling Skill**. For executive-level (C-suite/VP), also pull role-level priorities and pain points from **CXO Personas**. Do NOT include people who are not involved in this opportunity.*

### Key Stakeholders

**Mark Chen 陈明** — VP of Supply Chain (供应链副总裁)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Champion — 主动发起这个项目，供应链数据平台是他的 KPI。也是供应链模块的 Economic Buyer（$1M 以内他可以自己批）。 |
| **Current Stance** | Supportive — 第一次拜访就明确表达 "我们需要一个统一的数据底座"。第二次 tech deep-dive 后更加坚定，已在内部推动立项。`[Updated: 2026-04-28]` |
| **What They Care About** | *← CXO Persona: VP Supply Chain* — Inventory optimization & demand forecasting accuracy; global warehouse visibility (12 warehouses across 5 countries); supply chain resilience and risk mitigation; total logistics cost reduction; supplier collaboration efficiency. Agent focus: 本次 opp 重点是 **全球库存可视化 + 需求预测**，其他是 phase 2。 |
| **Profiling** | *← Contact Profiling* — 美国 MBA 背景（Northwestern Kellogg），之前在 Amazon FBA 做了 5 年 supply chain ops，对 AWS 生态非常熟悉。沟通风格偏美式 — 直接、数据驱动、喜欢看 metrics。英文流利，开会经常中英混杂。不喜欢 "画饼式" 沟通，要看具体的 implementation timeline 和 resource commitment。跟 CTO 刘大卫关系很好（一起从亚马逊跳槽过来的），两人经常联合推项目。`[Updated: 2026-04-28]` |
| **What We Need From Them** | 内部推动预算审批 + 协调供应链团队配合 POC + 在 CFO 面前为项目 ROI 背书 |
| **How to Win Them** | AE lead 商业对话 + SA 提供 demand forecasting 的 POC demo。重点展示：全球库存可视化 dashboard（类似 Cainiao 案例）+ SageMaker demand forecasting 的准确率提升数据。他是 Amazon 出身，对 AWS 有天然好感 — 用 AWS 内部语言跟他沟通（"two-pizza team"、"working backwards"）。建议每次 meeting 都带 metrics/data。 |

**David Liu 刘大卫** — CTO (首席技术官)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Technical Decision Maker — DTC 平台迁移的技术拍板人。全公司云架构最终由他决定。 |
| **Current Stance** | Supportive — 对 AWS 技术能力认可（特别是 Global Accelerator 和 CloudFront 方案），但对迁移风险有务实的顾虑（"Black Friday 前不能动生产环境"）。`[Updated: 2026-04-28]` |
| **What They Care About** | *← CXO Persona: CTO* — Platform reliability & global performance (DTC must sustain 10x traffic spikes during sales events); migration risk mitigation (zero-downtime migration); microservices architecture maturity; DevOps/SRE team capability building; cost predictability at scale. Agent focus: 本次 opp 重点是 **全球性能一致性 + 迁移零风险 + 大促弹性**。 |
| **Profiling** | *← Contact Profiling* — 技术实干派，前亚马逊 Senior SDE。重视架构优雅和代码质量。开会时问题很尖锐但 constructive — 如果回答不上来会迅速失去兴趣。偏好看架构图和 actual code/config，不喜欢高层 deck。对 SA 的技术深度要求很高。第二次 meeting 时跟 SA 李珊的白板讨论非常投入，明确说 "这是我见过最懂 DTC 架构的 SA"。习惯在 Slack（内部）和 WeChat（外部）沟通，回复很快。`[Updated: 2026-04-28]` |
| **What We Need From Them** | 技术方案签字 + 迁移 timeline 承诺 + 协调工程团队配合 |
| **How to Win Them** | SA lead 全程。继续用白板方式深入讨论迁移计划（phase-by-phase）。重点解决他的核心顾虑：Black Friday 前不动生产。建议做一个 "migration playbook" 展示每个 phase 的 rollback plan。利用他跟李珊的信任关系。技术深度 > 一切。 |

**Jenny Zhao 赵婧** — CFO (首席财务官)

| Dimension | Details |
|---|---|
| **Engagement Priority** | Important |
| **Role in This Deal** | Economic Buyer — $1M 以上投资需要她签字。对 ROI 和 payback period 极其敏感。 |
| **Current Stance** | Cautious — 第二次 meeting 后听了 CTO 的汇报，原则上认可项目必要性，但对 $2.1M 的投资规模有保留。多次提到 "能不能分阶段投入" 和 "阿里云那边给的折扣力度很大"。`[Updated: 2026-04-28]` |
| **What They Care About** | *← CXO Persona: CFO* — Capital efficiency & cash flow management; clear ROI with measurable business outcomes (not just "faster" or "better"); cost predictability (no surprise bills); competitive vendor pricing; CFO-level business cases need 3-year TCO comparison. Agent focus: 本次 opp 重点是 **TCO 对比 + 分阶段投入方案 + ROI 量化**。 |
| **Profiling** | *← Contact Profiling* — CPA + CFA 背景，曾在 PwC 做 TMT audit。对数字极其敏感，会自己拉 Excel 验证供应商给的 ROI 模型。沟通风格冷静克制，不会当面说 "不行"，但会用 "我需要更多数据" 来表示不满意。注重 governance — 任何大额投资要走 Finance Committee。每月只给供应商 1-2 次 meeting 机会，时间必须高效。不参与技术讨论，只看商业结果。`[Updated: 2026-04-28]` |
| **What We Need From Them** | Finance Committee 通过 + PPA 签字 |
| **How to Win Them** | AE lead 商业对话。准备极致的 TCO 分析：当前多云架构 vs AWS 统一架构的 3 年对比（含运维人力成本）。展示分阶段投入方案（Phase 1: DTC migration $800K → Phase 2: Supply Chain analytics $700K → Phase 3: ML + optimization $600K）。用 Black Friday 宕机的 $2M 损失做 "cost of doing nothing" 论证。不要谈技术。回应阿里云折扣时，用 "total value" 框架（不只是 unit price，含全球覆盖、减少多云运维人力等）。建议在 VP 拜访后 1-on-1 跟进。 |

*Engagement sequence rationale: CTO 和 VP Supply Chain 联合推动（两人从 Amazon 一起过来，互相支持），先搞定技术认可和业务需求确认 → 再联合向 CFO 呈现商业案例。VP visit 是关键节点 — 用 AWS 高层的战略对话打动 CEO/CFO 层面的信心。*
*建议顺序，请确认。*

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1 (Apr 14) | First visit: validate pain, understand multi-cloud challenges, confirm Champion | VP SC Mark Chen, CTO David Liu | **Done** ✅ |
| 2 | Week 3 (Apr 28) | Technical deep-dive: DTC migration architecture + supply chain data platform design | CTO David Liu, VP SC Mark Chen, Platform Engineering team | **Done** ✅ |
| 3 | Week 5 (May 14) | AWS VP visit: strategic alignment, build executive relationship, advance to Business Validation | CTO David Liu, VP SC Mark Chen, CFO Jenny Zhao + AWS VP 马总 | **Next** ↓ |
| 4 | Week 7 (May 28) | CFO business case: TCO analysis, phased investment plan, ROI model | CFO Jenny Zhao, VP SC Mark Chen | Planned |
| 5 | Week 9-11 (Jun-Jul) | Phase 1 POC: DTC traffic routing via CloudFront + Global Accelerator | CTO David Liu, Platform Engineering | Planned |
| 6 | Week 13 (Jul) | PPA negotiation + contract | CFO Jenny Zhao, Procurement | Planned |

> *Status: **Next ↓** (detailed below) · **Planned** · **Done** · **Skipped***

---

### Next Milestone Detail

**Milestone #3** — Target Date: May 14, 2026

**Objective:** AWS VP 拜访 Anker 深圳总部，建立高层关系，确认战略合作方向，推动进入 Business Validation

**Customer Attendees & Target Outcome:**
- **CTO David Liu 刘大卫** — 向 VP 展示技术方案成熟度，获得高层背书加速内部推进
- **VP SC Mark Chen 陈明** — 确认供应链数据平台的战略价值，为 CFO business case 铺垫
- **CFO Jenny Zhao 赵婧** — 首次接触 AWS 高层，建立信任，了解 AWS 战略投入承诺

**AWS Team:** VP 马总 (Lead), AE 张磊, SA 李珊, SA Lead 周明

**Key Messages for VP:**
1. Anker 是中国出海品牌标杆 — AWS 服务这类客户的全球化能力是核心差异化
2. 技术团队已高度认可（CTO 和 VP SC 都是 ex-Amazon），差的是 CFO 层面的信心
3. $2.1M 是起步 — Anker 全球 12 仓 + DTC 平台 + AI 推荐引擎的 total addressable spend 可达 $8-10M
4. 竞争压力：阿里云正在用大折扣 retain 国内工作负载

**Suggested Questions for VP to Ask:**
1. "Anker 在全球化过程中，基础设施一致性是最大的挑战吗？还是有其他更紧迫的问题？" *(Strategic alignment)*
2. "DTC 对 Anker 的长期战略意味着什么？Amazon 渠道和自有渠道的比例目标是多少？" *(Business context depth)*
3. "在 IT 投资优先级上，cloud migration 跟你们 R&D 投入是怎么排序的？" *(Budget priority, for CFO context)*

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 5 | 8 |
| **Timeline** | 10 weeks (Jul close) | 18 weeks (Sep close) |

**What could change:**
- CFO 可能要求阿里云/Azure 正式 competitive bid，增加 3-4 周
- Black Friday 冻结期（Oct-Nov）如果影响迁移计划，可能需要调整 PPA scope 和 timeline
- 如果 VP visit 无法打动 CFO，可能需要追加一次 CEO-to-CEO engagement
- Phase 1 POC 结果如果不够有说服力（性能不达标），可能需要延长验证期
- Anker IPO 准备（传闻中）可能导致 capex 审批收紧

---

## 3. Execution Log

> *Auto-updated after each Call Plan + PMR. Most recent at top.*

### Visit 2 — 2026-04-28 | Technical Deep-Dive

**Result:** CTO 和 VP SC 对 DTC migration 架构方案高度认可。CTO 明确说 "这就是我想要的方案"。白板讨论了 3 小时（原计划 2 小时）。关键共识：Phase 1 先做 CDN + 全球流量调度，Phase 2 供应链数据平台。CTO 提出 "Black Friday 之前不能动生产" 的硬约束。VP SC 确认他会推动 CFO 安排 VP 拜访。
**Stage:** Qualified → Technical Validation
**Key Change:** CTO 从 "感兴趣" 升级为明确支持；VP SC 开始主动帮我们在内部推动。

### Visit 1 — 2026-04-14 | Discovery & Relationship Building

**Result:** 验证了核心痛点（Black Friday 宕机 + 全球库存不可视）。确认 Mark Chen 为 Champion。了解到多云架构现状（阿里云国内 + Azure 部分海外 + Shopify 前端）。CTO David Liu 到场时间超出预期（原计划 30 分钟，实际聊了 90 分钟），对 AWS 全球架构非常感兴趣。CFO 未参加，需要后续安排。
**Stage:** Prospect → Qualified
**Key Change:** 确认 opportunity 真实性和紧迫度；initial stakeholder map 建立。

---

*Engagement Plan Template | Version: 1.1*
