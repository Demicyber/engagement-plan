# Engagement Plan: 瑞安集团 - 数据平台现代化

> **What is this?** 针对瑞安集团数据平台迁移商机的行动计划。回答：我需要搞定谁、从每个人那里获得什么、以及我的整体推进路线。
>
> 🤖 *基于 BD 输入自动生成。每次拜访后更新。*
>
> ✅ *生成后请 BD 审阅并修改。*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | 瑞安集团（大型零售企业，300+ 线下门店 + 线上电商平台） |
| **Opportunity Name** | 数据平台现代化（Oracle 数仓迁移至 AWS） |
| **Deal Value** | $600K ARR [Updated: 2026-04-30] |
| **Current Stage** | Qualified [Updated: 2026-04-30] |
| **Target Close Date** | [待确认 — 请确认客户期望的上线时间，以便反推关单日期] |
| **Why Now** | Oracle 数仓维护成本每年涨 15%（客户已完成内部评估确认），必须迁移；同时需要实时分析能力支撑 300+ 门店运营 [Updated: 2026-04-30] |
| **Deal Objective** | 签订 $600K ARR 合同，将客户核心数据仓库从 Oracle 迁移至 AWS 云原生数据平台，实现实时分析能力 |

### Win Strategy

瑞安集团的核心痛点是 Oracle 数仓维护成本每年涨 15% 且无法满足 300+ 门店实时分析需求。我们的赢单主题是 **AWS 云原生数据平台（Amazon Redshift / Lake Formation / Kinesis）+ 零停机迁移方案**，核心差异化在于：(1) 成熟的 Oracle 迁移方案（SCT + DMS CDC 增量迁移），(2) 实时分析能力（Kinesis + Redshift Streaming），(3) 客户已有 EC2 存量工作负载——一体化平台价值，(4) Azure 尚无正式提案——先发优势窗口。关键风险：刘洋的业务连续性顾虑必须在技术深潜中彻底解决。[Updated: 2026-04-30]

---

## 2. Engagement Plan

### Key Stakeholders

**陈明** — CTO

| Dimension | Details |
|---|---|
| **Role in This Deal** | Champion / Decision Maker |
| **Current Stance** | **Supportive / Champion** — 非常积极，已完成内部评估，明确选 AWS，主动透露 EB 和预算信息，主动建议下一步 [Updated: 2026-04-30] |
| **What They Care About** | *← CTO Persona:* (1) 技术架构现代化与平台工程——从传统数仓迁移到云原生数据平台；(2) 工程效率与成本优化——Oracle 许可费用每年涨 15% 是直接痛点；(3) AI/ML 集成——迁移到云上后为未来 AI 分析铺路；(4) 可靠性——300+ 门店实时系统不能中断 |
| **What We Need From Them** | (1) ✅ 已确认技术方向选 AWS；(2) ✅ 已安排技术深潜（2 周内）；(3) 推动 CFO 李红审批预算；(4) 持续作为内部 Champion 推进项目 |
| **How to Win Them** | 已验证有效策略：技术语言 + 同行案例 + 具体迁移路径。下一步在技术深潜中展示详细方案，重点解决业务连续性保障，让陈明有信心向 CFO 汇报。 [Updated: 2026-04-30] |

**刘洋** — Head of Data

| Dimension | Details |
|---|---|
| **Role in This Deal** | Evaluator / Influencer（潜在 Blocker 风险） |
| **Current Stance** | **Cautious** — 主要担心数据迁移过程中 300+ 门店实时库存系统的业务连续性 [Updated: 2026-04-30] |
| **What They Care About** | *← CDO Persona:* (1) 数据迁移过程中的业务连续性——300+ 门店实时库存系统不能停（已确认为最大顾虑）；(2) 数据迁移的数据质量与完整性；(3) 实时数据管道架构；(4) 数据治理与可观测性 |
| **What We Need From Them** | (1) 提供当前数据架构信息（数据量、核心表、ETL 清单）——已请求；(2) 在技术深潜后认可迁移方案的可行性和业务连续性保障；(3) 转变 stance: Cautious → Supportive |
| **How to Win Them** | 技术深潜中重点演示 DMS CDC 增量迁移 + 双跑验证方案，用具体技术细节（而非空洞承诺）消除业务连续性顾虑。准备零售行业零停机迁移案例。如果刘洋不被说服，他可能成为 Blocker。 [Updated: 2026-04-30] |

**李红** — CFO [New: 2026-04-30]

| Dimension | Details |
|---|---|
| **Role in This Deal** | Economic Buyer |
| **Current Stance** | Unknown — 尚未直接接触 [Updated: 2026-04-30] |
| **What They Care About** | [待确认 — 预计关注：(1) Oracle 维护成本 vs. AWS 迁移 + 运营的 TCO 对比；(2) 迁移项目的 ROI 和回收周期；(3) 预算 ~$600K 的合理性] |
| **What We Need From Them** | 预算审批 |
| **How to Win Them** | 通过陈明传递 TCO/ROI 材料，或在 Business Validation 阶段安排直接拜访。准备 3 年 TCO 对比（Oracle vs. AWS），量化每年 15% 维护成本增长的长期影响。 [Updated: 2026-04-30] |

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1（2026-04-30） | 验证痛点、了解决策流程、确认技术方向偏好、识别 Champion | 陈明 (CTO), 刘洋 (Head of Data) | **Done** ✅ [Updated: 2026-04-30] |
| 2 | Week 3（~2026-05-14） | 技术深潜：迁移方案 + 业务连续性保障 + 架构评估 | 陈明, 刘洋, AWS SA | **Next** ↓ |
| 3 | Week 5-6 | POC 范围定义 / 试点迁移方案 + TCO/ROI 呈现 | 陈明, 刘洋, CFO 李红 | Planned |
| 4 | Week 8-9 | 业务案例 + 报价方案 + CFO 拜访 | CFO 李红, 陈明 | Planned |
| 5 | Week 11-12 | 合同谈判 + 签约 | CFO 李红, Procurement | Planned |

---

### Next Milestone Detail

**Milestone #2** — ~2026-05-14（Week 3） [Updated: 2026-04-30]

**Objective:** 技术深潜——展示详细迁移方案，重点解决业务连续性保障，验证技术可行性

**Customer Attendees & Target Outcome:**
- **陈明 (CTO)** — 确认迁移方案可行，有信心向 CFO 汇报 → 保持 Supportive
- **刘洋 (Head of Data)** — 消除业务连续性顾虑 → Cautious → Supportive

**AWS Team:** BD + SA（解决方案架构师）

**Suggested Discovery Questions:**
- 当前 Oracle 数仓到实时库存系统的数据流是怎样的？有没有中间层？——评估迁移切入点
- 可接受的迁移窗口（maintenance window）是多长？有没有业务低谷期？——制定迁移计划
- 如果做试点，哪个工作负载最适合先迁移？——定义 POC 范围
- 内部 IT 团队有多少人可以参与迁移项目？——评估交付模式（自研 vs. 合作伙伴）
- CFO 李红对这个项目的态度如何？有什么特别关注的点吗？——为后续 EB 接触做准备

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 4 | 7 |
| **Timeline** | 10 weeks | 16 weeks |

[Updated: 2026-04-30] 比初始估计乐观——Champion 已确认、EB 已识别、预算已确认，缩短了 Qualified 阶段的探索时间。

**What could change:**
- 刘洋的业务连续性顾虑未消除——可能增加额外技术验证轮次（+2 周）
- Azure 正式提案——可能触发 POC 对比（+3-4 周）
- CFO 李红对迁移 ROI 有疑虑——需要额外 EB 拜访
- 客户内部采购流程未知——可能增加 2-4 周

---

## 3. Execution Log（回滚）

### Call #1 - 2026-04-30 - 陈明 (CTO), 刘洋 (Head of Data) [Updated: 2026-04-30]

| Field | Details |
|---|---|
| **Planned** | 验证痛点、了解决策流程、确认技术方向偏好、识别 Champion |
| **Actual** | 超出预期——痛点已量化（Oracle 成本年涨 15%）、技术方向确认（AWS 首选）、Champion 确认（陈明）、EB 识别（CFO 李红）、预算确认（$600K）、竞争态势摸清（Azure 无正式提案） |
| **People Updates** | 陈明: Unknown → Supportive/Champion · 刘洋: Unknown → Cautious（业务连续性顾虑）· 新增: CFO 李红 (EB) |
| **Key Learnings** | (1) 迁移动力很强——Oracle 成本年涨 15% 是量化痛点；(2) 刘洋的业务连续性顾虑是本 deal 最大风险点；(3) 陈明是高质量 Champion——主动推进、主动透露信息 |
| **Plan Adjustment** | Stage: Prospect → Qualified · Deal Value: $500K → $600K · 新增 CFO 李红到 stakeholder · Milestone #1 完成，#2 成为 Next |

---

*Engagement Plan | Version: 1.1 | Created: 2026-04-29 | Last Updated: 2026-04-30*
