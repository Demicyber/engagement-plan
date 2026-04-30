# Call Plan — 明华重工 (Minghua Heavy Industries)

> **Purpose:** Prepares AWS sales team members before external customer meetings.
>
> ✅ *After generating, agent always asks sales to review and revise as needed.*

---

## 1. Meeting Details

| Field | Value |
|---|---|
| **Date & Time** | 2026-05-15 14:00-16:00 CST (UTC+8) |
| **Duration** | 2 hours |
| **Format** | In-person |
| **Location** | 明华重工总部，北京市朝阳区建国路 88 号，明华大厦 18F 会议室 |
| **Opportunity Name** | AI Quality Inspection System |
| **Current Sales Stage** | Qualified |

### Customer Attendees

| Name | Title | Role in Decision |
|---|---|---|
| 张敏 (Zhang Min) | CTO | Champion / Technical Decision Maker |
| 李华 (Li Hua) | VP Manufacturing | Influencer |

### Attendee Insights

> *💡 Condensed from EP Key Stakeholders.*

**张敏 (Zhang Min)** — CTO
- **Focus & Priorities:** Technology architecture scalability; AI/ML production-readiness; integration with MES/ERP; MLOps and model lifecycle; team enablement path *← CXO Persona: CTO*
- **Communication Approach:** 技术出身，喜欢白板讨论胜过 PPT。如果觉得对方不懂技术会迅速失去耐心。决策风格 "先证明再推广"。沟通直接不绕弯。 *← Contact Profiling*
- **Current Stance:** Supportive — 主动发起项目，但对 "POC 不落地" 有顾虑（去年华为云 POC 烂尾）
- **Our Goal:** 确认 Champion 角色；技术方案认可；agree to technical deep-dive as next step

**李华 (Li Hua)** — VP Manufacturing
- **Focus & Priorities:** 产线不停机、实施影响最小化、质检准确率和速度、一线培训成本、MES 集成
- **Communication Approach:** 实干型，注重可操作性。经常问 "这个在我的产线上能跑吗"。喜欢看实际效果（demo > slide）。 *← Contact Profiling*
- **Current Stance:** Neutral — 感兴趣但不确定能否集成到现有产线
- **Our Goal:** 了解产线痛点；确认 POC 配合意愿

### AWS Attendees

| Name | Title | Role in Meeting |
|---|---|---|
| 陈伟 (Chen Wei) | Account Executive | Lead |
| 刘洋 (Liu Yang) | Solutions Architect | Support |
| 周明 (Zhou Ming) | Manufacturing SA Specialist | SME |

---

## 2. Target Meeting Outcomes

| # | Customer Perspective | Our Perspective |
|---|---|---|
| 1 | 了解 AWS 在 AI 质检领域的真实能力和同行案例 | 验证痛点真实性和紧迫度（退货率 3.2% 的具体影响） |
| 2 | 评估 AWS 方案与现有系统（MES、ERP）的集成可行性 | 确认 CTO 张敏作为 Champion，了解内部决策流程 |
| 3 | 获得初步的实施路径和时间线参考 | 收集 POC scope 定义所需的技术信息 |

**Target Stage Progression:** ( Qualified ) → ( Technical Validation ) — 如果成功获得 CTO 认可进入技术 deep-dive

---

## 3. Success Criteria

| # | Customer Would Consider It Successful If… | We Would Consider It Successful If… |
|---|---|---|
| 1 | AWS 能清晰展示一个与明华类似的制造业 AI 质检案例，包括具体指标 | CTO 张敏明确表示愿意安排第二次 technical deep-dive，并给出具体时间 |
| 2 | AWS 团队理解明华产线的具体技术约束（MES 版本、产线节拍、网络条件） | VP Mfg 李华确认至少一条产线可用于 POC 测试 |
| 3 | 获得清晰的下一步行动计划，不是 "我们回去研究研究" | 确认完整的决策链：CTO 技术认可 → CFO 预算审批 → Procurement 执行 |

---

## 4. Information Exchange

### Information to Gather

| # | Question | Category | Target Attendee | Purpose |
|---|---|---|---|---|
| 1 | 目前质检流程是怎样的？从原材料进场到成品出货，哪个环节的退货率最高？ | Metrics / Implicated Pain | CTO 张敏 + VP Mfg 李华 | 量化痛点，确认 AI 质检的最高价值切入点 |
| 2 | 去年华为云 POC 的具体情况是什么？做了多久？为什么没有落地？ | Decision Criteria / Competition | CTO 张敏 | 理解竞争格局和客户对 POC 的真实顾虑，避免踩同样的坑 |
| 3 | 如果年底前退货率没有降到 1% 以下，对明华的业务影响是什么？董事会有什么具体要求？ | Economic Buyer / Compelling Event | CTO 张敏 | 确认 compelling event 的真实性和紧迫度，为后续 CFO 沟通铺垫 |
| 4 | 这个项目的技术评估和预算审批分别由谁决定？除了你和王总（CFO），还有谁需要 sign off？ | Decision Process / Champion | CTO 张敏 | 完善 stakeholder map，确认是否有隐藏的 blocker |
| 5 | 产线的网络条件怎么样？质检站点离云端的延迟要求是多少？能接受边缘推理的方案吗？ | Technical / Decision Criteria | VP Mfg 李华 | 确认边缘 vs 云端推理的架构选择，影响方案设计和定价 |
| 6 | 质检图片的类型和质量如何？现有标注数据有多少？ | Technical | CTO 张敏 | 评估 ML 训练数据就绪程度，影响 POC timeline |

### Information to Deliver

| # | What to Share | Format | Purpose |
|---|---|---|---|
| 1 | 东风汽车零部件 AI 质检案例：退货率从 2.8% 降至 0.5%，年节省 ¥1,500 万 | Case study (2-page summary) | 用同行数据建立信任，展示 AWS 在制造业 AI 质检的实际交付能力 |
| 2 | SageMaker + 边缘推理架构示意图（产线部署） | Whiteboard sketch | 让 CTO 看到端到端架构，让 VP Mfg 看到产线部署方式（非侵入式） |
| 3 | 中国制造业 AI 质检趋势数据（IDC 2026 报告摘要） | Data point (1 slide) | 建立行业紧迫感：头部制造商已在部署，明华不能落后 |

---

## 5. Potential Objections & Responses

| # | Anticipated Objection | Our Response |
|---|---|---|
| 1 | **"上次华为云 POC 做了半年也没落地，怎么保证这次不一样？"** *(CTO 张敏)* | 完全理解。我们的做法不同：第一，POC scope 由双方共同定义，包括明确的成功标准（不是 "看看效果"）；第二，我们用 SageMaker MLOps pipeline 确保模型从 POC 到生产的连续性，不存在 "POC 环境和生产环境不一样" 的问题；第三，我们建议 4 周 POC 而不是 6 个月 — 快速验证，快速决策。东风那边的 POC 从启动到出结果就用了 3 周。 |
| 2 | **"AI 部署会不会影响产线节拍？我们停不起机。"** *(VP Mfg 李华)* | 不会。方案采用边缘推理，质检模型部署在产线旁的边缘设备上，inference latency < 200ms，完全不影响产线节拍。部署过程是 "并行上线" — 先在旁边跑，跟现有质检对比，数据验证 OK 后再切换。东风的部署就是这样，产线零停机。 |
| 3 | **"AWS 的成本比国内云贵，CFO 那边不好过。"** *(CTO 张敏)* | 理解成本敏感度。但这里的对比不应该是 "AWS vs 阿里云的云服务单价"，而是 "AI 质检方案的总体 ROI"。明华每季度退货损失约 ¥2,000 万，如果方案能把退货率从 3.2% 降到 1% 以下，年回报远超投资。我们会给王总（CFO）准备一份详细的 TCO 分析和 3 年 payback 模型，让数字说话。 |

---

## 6. Meeting Agenda

| Time | Topic | Owner | Purpose |
|---|---|---|---|
| 14:00–14:10 | 开场介绍 & 明华现状了解 | AE 陈伟 | 建立关系，确认今天议程 |
| 14:10–14:40 | 明华质检痛点深入讨论 | SA 刘洋 (引导提问) + 张敏/李华 | 验证痛点，收集技术细节（Discovery Q1-Q6） |
| 14:40–15:10 | AWS AI 质检方案 & 东风案例 | SA Specialist 周明 | 展示方案能力 + 同行验证（白板 session） |
| 15:10–15:30 | 架构讨论：边缘推理 + MES 集成 | SA 刘洋 + CTO 张敏 | 技术可行性验证（白板讨论，非 PPT） |
| 15:30–15:45 | 实施路径 & POC 方式讨论 | AE 陈伟 + 全体 | 确认 POC 意愿和初步 scope |
| 15:45–15:55 | 总结 & 下一步 | AE 陈伟 | 确认 next steps 和时间线 |
| 15:55–16:00 | 结束 | AE 陈伟 | — |

> *注意：张敏偏好白板讨论，架构部分不要用 PPT。李华关注产线实操，周明准备好边缘部署的实际照片/视频。*

---

## 7. Potential Next Steps

| # | Proposed Next Step | Timeline | Owner | Purpose |
|---|---|---|---|---|
| 1 | 安排技术 deep-dive：SageMaker MLOps + 边缘推理架构详细设计 | 2 周内（May 26） | Joint (AWS SA + 明华 CTO team) | 技术方案验证，进入 Technical Validation 阶段 |
| 2 | AWS 提供东风汽车案例详细报告 + TCO 分析初稿 | 1 周内 | AWS (AE 陈伟) | 为后续 CFO 沟通准备弹药 |
| 3 | 安排东风汽车客户参考电话（如果张敏/李华感兴趣） | 2 周内 | AWS (AE 陈伟) | 通过 peer validation 增强信心，特别是解决 "POC 不落地" 的顾虑 |

---

*Call Plan Template | Version: 1.1*
