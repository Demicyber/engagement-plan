# Engagement Plan: Anker — Global DTC Cloud Migration & Data Analytics Platform

> **What is this?** A focused action plan for winning a specific opportunity.

## 1. Opportunity Snapshot

| Dimension | Detail |
|-----------|--------|
| **Customer** | Anker Innovations (安克创新科技) |
| **Opportunity Name** | Global DTC Expansion + Supply Chain Cloud Migration + Data Analytics Platform |
| **Deal Value** | $2.1M ARR (首年), 3年 TCV ~$5.8M |
| **Current Stage** | Technical Validation (Stage 3) |
| **Target Close Date** | 2026-08-15 |
| **Why Now** | Anker 2026 战略重点：DTC 渠道占比从 35% 提升至 55%；现有 on-prem 供应链系统面临 EOL；CEO 在 Q1 earnings call 提到 "data-driven decision making" |
| **Primary Competitor** | Azure (现有部分 workload 在 Azure；阿里云负责国内电商) |

### Deal Objective & Win Strategy

**Objective:** 拿下 DTC 全球化平台 + 供应链数据湖作为 landing workload，建立 Anker 全球基础设施标准化的 precedent。

**Win Strategy:**
- 利用 AWS Global Infrastructure 优势（Anker DTC 覆盖 40+ 国家，Azure 在部分区域无 presence）
- 通过 Supply Chain POC 证明 real-time visibility 价值，对标现有 on-prem 方案 3-5x 延迟改善
- Executive alignment：马总与 Anker CEO 阳萌有过一次简短交流（2025 re:Invent），本次 EB 是深化关系的关键触点
- 用 Data Analytics 作为 wedge — Anker 数据团队已在用 Redshift Serverless（shadow IT），可以 legitimize + expand

## 2. Engagement Plan

### Key Stakeholders

#### Mark Chen — VP of Supply Chain

| Dimension | Assessment |
|-----------|-----------|
| **Title & Org** | VP of Supply Chain, Operations Division |
| **Decision Role** | Economic Buyer (供应链预算 owner) |
| **Pain Points** | 全球供应链可视性不足；库存周转天数高于行业平均 15%；on-prem 系统 EOL 迫在眉睫 |
| **Success Metrics** | 库存成本降低 20%、供应链响应时间 <4h、系统 uptime 99.95% |
| **Communication Style** | 数据驱动，喜欢看 benchmark 和 ROI 计算；英文沟通为主 |
| **Attitude Toward AWS** | Neutral-positive；之前用 Azure 是历史原因，对 AWS 全球覆盖感兴趣 |
| **Engagement History** | 2 次技术交流 (SA-led)，1 次 supply chain workshop |

#### David Liu — CTO

| Dimension | Assessment |
|-----------|-----------|
| **Title & Org** | CTO, Technology Division |
| **Decision Role** | Technical Decision Maker + Champion (内部推动云优先战略) |
| **Pain Points** | 技术债务重；团队招聘困难（深圳 vs 北京竞争）；需要 managed services 减少 ops burden |
| **Success Metrics** | 工程效率提升、release velocity 翻倍、降低 on-call 负担 |
| **Communication Style** | 技术深度对话，喜欢 whiteboard session；中英文混合 |
| **Attitude Toward AWS** | Champion — 个人经验丰富，前公司 all-in AWS |
| **Engagement History** | 参加过 re:Invent 2025，主动联系 SA 讨论 EKS 方案 |

### Engagement Roadmap

| Phase | Activity | Owner | Target Date | Status |
|-------|----------|-------|-------------|--------|
| Phase 1 | Discovery Workshop (completed) | 李珊 | 2026-03-20 | ✅ Done |
| Phase 2 | Supply Chain POC Scoping | 李珊 + 周明 | 2026-04-15 | ✅ Done |
| **Phase 3** | **Executive Briefing (VP Visit)** | **张磊 + 马总** | **2026-05-14** | **🔄 In Progress** |
| Phase 4 | POC Execution (6 weeks) | 李珊 | 2026-06-01 ~ 07-15 | ⏳ Planned |
| Phase 5 | Business Case & Proposal | 张磊 | 2026-07-20 | ⏳ Planned |
| Phase 6 | Negotiation & Close | 张磊 + 马总 | 2026-08-15 | ⏳ Planned |

## 3. MEDDPICC Tracker

| Element | Status | Detail |
|---------|--------|--------|
| **Metrics** | 🟡 Partial | 有定性目标，需要量化 baseline (库存周转天数、current infra cost) |
| **Economic Buyer** | 🟢 Identified | Mark Chen (supply chain budget) + CFO [待确认] for platform-level spend |
| **Decision Criteria** | 🟡 Partial | 技术层面清晰 (global coverage, managed services)；商业层面需进一步确认 |
| **Decision Process** | 🟡 Partial | CTO + VP SC 联合推荐 → CEO 批准；采购流程 [待确认] |
| **Paper Process** | 🔴 Unknown | 合同审批流程未明确，需了解法务和采购周期 |
| **Identified Pain** | 🟢 Confirmed | Supply chain visibility + EOL urgency + DTC global expansion |
| **Champion** | 🟢 Strong | David Liu (CTO) — 积极推动，有内部影响力 |
| **Competition** | 🟡 Active | Azure incumbent (部分 workload)；阿里云 (国内电商) |

## 4. Account Intelligence

### Competitive Landscape

| Competitor | Footprint | Threat Level | Our Counter |
|-----------|-----------|--------------|-------------|
| Microsoft Azure | 部分 infra workload, O365 | 🟡 Medium | Global coverage gap in SEA/LATAM; 价格竞争力 |
| 阿里云 | 国内电商平台 hosting | 🟢 Low | 不争国内电商部分，focus on global + analytics |
| GCP | BigQuery 评估中 | 🟡 Medium | Redshift Serverless 已有 adoption；生态整合优势 |

### Technical Environment

| Layer | Current State | Target State |
|-------|--------------|--------------|
| Compute | On-prem VMware + Azure VMs | EKS (global DTC) + EC2 (supply chain) |
| Data | Oracle DB + Hadoop on-prem | RDS Aurora + S3 Data Lake + Redshift |
| Analytics | Tableau + custom scripts | QuickSight + SageMaker + Redshift Serverless |
| Supply Chain | SAP ECC (on-prem, EOL 2027) | SAP on AWS + custom microservices |

### Recent Activities

| Date | Activity | Key Takeaway |
|------|----------|-------------|
| 2026-03-20 | Discovery Workshop | 确认 3 大 workload 方向；David Liu 表态支持 AWS |
| 2026-04-08 | SA Deep Dive (Supply Chain) | 技术方案初步成型；Mark Chen 参与度高 |
| 2026-04-15 | POC Scope Alignment | POC 范围确定：supply chain visibility dashboard |
| 2026-04-28 | Pre-brief call (张磊 ↔ Mark Chen) | 确认 VP visit agenda 方向；Mark 会带 CTO 一起 |

### Risk Register

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|-----------|
| Azure counter-offer (大幅折扣) | Medium | High | 提前准备 PPA/EDP 方案；强调 TCO 而非 unit price |
| POC 延期影响 close timeline | Medium | Medium | 缩小 POC scope，确保 6 周内可交付 |
| CFO 卡预算 | Low | High | 通过 EB 建立 executive sponsorship；准备 ROI business case |
| 内部 champion 离职 | Low | Critical | 多点关系建设，不单一依赖 David Liu |
