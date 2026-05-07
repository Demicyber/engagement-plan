# Engagement Plan: 理想汽车 (Li Auto) - 智能驾驶数据湖 + OTA 平台

> **What is this?** A focused action plan for winning a specific opportunity.  
> ⚠️ 新客户首次接触，部分信息标记 [待确认]，需通过首次拜访验证。

---

## 1. Opportunity Snapshot

| Dimension | Detail |
|-----------|--------|
| **Customer** | 理想汽车 (Li Auto) — 智能驾驶事业部 |
| **Opportunity Name** | Intelligent Driving Data Lake + OTA Platform |
| **Deal Value** | $1.5M ARR (estimated) |
| **Current Stage** | Prospect — 首次正式接触 |
| **Target Close Date** | 2026-Q4 [待确认] |
| **Why Now** | 理想 2026 年智驾全栈自研加速，数据量指数增长；现有单云架构遇到成本和弹性瓶颈，正在做多云评估 |
| **Deal Objective** | 成为理想智驾数据湖的主力云平台，同时拿下 OTA 数据分发场景 |
| **Win Strategy** | 以 S3 + Lake Formation 数据湖方案切入，结合 IoT/Edge 能力覆盖 OTA；通过 POC 建立技术信任，利用 AWS 汽车行业客户案例（蔚来、小鹏）形成 peer pressure |

---

## 2. Engagement Plan

### Key Stakeholders

#### 赵明辉 — VP of Autonomous Driving (智能驾驶副总裁)

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | 🔴 Critical — Executive Sponsor & Economic Buyer |
| **Role in This Deal** | 最终决策者，掌握预算审批权 |
| **Current Stance** | Neutral — 愿意见面了解，但尚未表达明确倾向 [待确认] |
| **What They Care About** | 智驾研发效率、数据闭环速度、成本可控、供应商生态多元化 |
| **Profiling** | 技术出身（前百度 Apollo），重视方案深度，不喜欢纯销售话术 [待确认] |
| **What We Need From Them** | 确认决策流程、预算周期、竞品评估范围 |
| **How to Win Them** | 用行业洞察和技术深度赢得尊重；展示 AWS 在自动驾驶数据处理的差异化能力 |

#### 孙浩 — Platform Architecture Director (平台架构总监)

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | 🟠 High — Technical Evaluator |
| **Role in This Deal** | 技术选型主导者，向赵明辉汇报 |
| **Current Stance** | [待确认] — 首次接触后判断 |
| **What They Care About** | 架构可扩展性、多云兼容、数据治理、性能基准 |
| **Profiling** | [待确认] |
| **What We Need From Them** | 当前技术栈细节、评估标准、timeline |
| **How to Win Them** | SA 深度技术交流 + 定制架构白皮书 |

#### 周小林 — Data Engineering Manager (数据工程经理)

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | 🟡 Medium — Day-to-day Influencer |
| **Role in This Deal** | 实际使用者和实施负责人 |
| **Current Stance** | [待确认] |
| **What They Care About** | 工具链成熟度、迁移复杂度、团队学习曲线 |
| **Profiling** | [待确认] |
| **What We Need From Them** | 数据规模、现有痛点、团队技能分布 |
| **How to Win Them** | Hands-on workshop + 免费培训资源 |

### Engagement Roadmap

| Phase | Timeline | Action | Owner |
|-------|----------|--------|-------|
| 1. Discovery | 2026-05-13 | 首次拜访：建立关系 + 需求摸底 | 张磊 / 李珊 |
| 2. Deep Dive | 2026-05 W3-4 | 技术交流会：架构讨论 + Demo | 李珊 + SA Manager |
| 3. Validation | 2026-06 | POC：智驾数据入湖 + 查询性能对比 | 李珊 + PSA |
| 4. Proposal | 2026-07 | 商务方案 + 定价 | 张磊 |
| 5. Close | 2026-Q4 | 签约 + 实施启动 | 张磊 |

---

## 3. MEDDPICC Tracker

| Element | Status | Notes |
|---------|--------|-------|
| **Metrics** | 🔴 Unknown | 需确认数据增长量、查询延迟目标、成本基线 |
| **Economic Buyer** | 🟡 Identified | 赵明辉 (VP)，但决策链可能涉及 CTO [待确认] |
| **Decision Criteria** | 🔴 Unknown | 首次拜访需探索 |
| **Decision Process** | 🔴 Unknown | 多云评估流程、参与部门 [待确认] |
| **Paper Process** | 🔴 Unknown | 采购流程、合规要求 |
| **Identified Pain** | 🟡 Hypothesized | 数据规模增长 vs 现有架构弹性不足（基于公开信息推断） |
| **Champion** | 🔴 None yet | 首次拜访后识别 |
| **Competition** | 🟡 Known | 阿里云（现有供应商）、华为云、Azure [待确认] |

---

## 4. Account Intelligence

### Competitive Landscape
- **阿里云**: 理想现有主力云，深度绑定；但客户有多云诉求，说明存在不满或风险对冲需求
- **华为云**: 车企圈影响力强，可能已有接触 [待确认]
- **Azure**: 全球化场景可能涉及，海外数据合规 [待确认]

### Technical Environment
- 现有数据湖基于阿里云 OSS + DataLake Analytics（公开信息推断）[待确认]
- 智驾数据量：预估 PB 级/年（基于行业 benchmark）[待确认]
- OTA 平台：自研 + 云服务混合架构 [待确认]

### Recent Activities
- 2026-Q1：理想发布新一代智驾芯片，数据处理需求升级
- 2026-04：行业媒体报道理想启动多云战略评估
- 2026-05：AWS 侧首次获得拜访机会（通过渠道伙伴引荐）

### Risk Register

| Risk | Impact | Mitigation |
|------|--------|-----------|
| 阿里云深度绑定，迁移成本高 | High | 定位增量场景而非存量替换 |
| 客户仅做 price benchmark 无真实意图 | Medium | 首次拜访验证真实痛点和 timeline |
| 华为云政府关系优势 | Medium | 强调全球化 + 技术领先性 |
| 决策链不清晰导致项目延期 | Medium | 尽早 map 完整决策流程 |
