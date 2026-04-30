# Call Plan — 星辰科技 (Starlight Tech)

> **Purpose:** Prepares AWS sales team members before external customer meetings.
> **Note:** Generated via Path B (direct sales request). No prior EP existed — EP auto-created after this Call Plan (see EP_StarlightTech_SaaS-Migration.md).
>
> ✅ *After generating, agent always asks sales to review and revise as needed.*

---

## 1. Meeting Details

| Field | Value |
|---|---|
| **Date & Time** | 2026-05-19 10:00-11:00 CST (UTC+8) |
| **Duration** | 1 hour |
| **Format** | Virtual (Feishu Meeting) |
| **Location / Link** | `[待确认 — CTO 陈思远发会议链接]` |
| **Opportunity Name** | SaaS Platform Cloud Migration |
| **Current Sales Stage** | Prospect |

### Customer Attendees

| Name | Title | Role in Decision |
|---|---|---|
| 陈思远 (Chen Siyuan) | CTO & Co-founder | Champion / Technical Decision Maker |

### Attendee Insights

> *💡 Built via Path B: agent invoked Contact Profiling (initial, from sales input) + CXO Persona (CTO) directly.*

**陈思远 (Chen Siyuan)** — CTO & Co-founder
- **Focus & Priorities:** Platform reliability & SLA guarantees; migration risk mitigation (zero-downtime); multi-tenancy best practices. *This opp:* reliability + migration risk 是核心，其余是加分项。 *← CXO Persona: CTO, context-adjusted for SaaS stability opp*
- **Communication Approach:** Failure-scenario thinker（"如果 XXX 挂了怎么办"）。偏好架构图 + failover demo。沟通直接高效，30 分钟 > 1 小时。90 后创始人。 *← Contact Profiling (initial)*
- **Current Stance:** Supportive — 主动联系 AWS，但对迁移风险有顾虑（"不能再出事了"）
- **Our Goal:** 确认 Champion 角色；验证痛点真实性；agree to architecture assessment

### AWS Attendees

| Name | Title | Role in Meeting |
|---|---|---|
| 张磊 (Zhang Lei) | Account Executive | Lead |
| 李珊 (Li Shan) | Solutions Architect | Support |

---

## 2. Target Meeting Outcomes

> *Prospect stage: 70/30 rule (customer talks 70%). Earn a second meeting, not close anything.*

| # | Customer Perspective | Our Perspective |
|---|---|---|
| 1 | 了解 AWS 能否解决 SaaS 平台稳定性问题，特别是高可用架构 | 验证痛点真实性：两次宕机的影响到底多严重？是痛还是痒？ |
| 2 | 评估 AWS 迁移风险是否可控（"不能再出事"） | 确认 CTO 为 Champion，了解 CEO 和 advisor 的态度 |
| 3 | 获得初步的迁移路径参考 | 了解竞争格局：阿里云走到哪一步了？ |

**Target Stage Progression:** ( Prospect ) → ( Qualified ) — 如果痛点验证 + CTO 认可 + 同意下一步

---

## 3. Success Criteria

| # | Customer Would Consider It Successful If… | We Would Consider It Successful If… |
|---|---|---|
| 1 | AWS 能清晰回答 "如果数据库挂了，系统怎么自动恢复" 这类问题 | CTO 同意安排第二次 architecture assessment，并给出具体时间 |
| 2 | 了解 AWS 上类似规模 SaaS 公司的迁移经验和时间线 | 确认决策链：CTO 技术选型 → CEO 预算审批 → 是否有其他 stakeholder |
| 3 | 对迁移风险有初步信心（不是零风险，而是风险可控） | 了解阿里云的竞争状态：是已经报价了，还是只是有人推荐 |

---

## 4. Information Exchange

### Information to Gather

| # | Question | Category | Target Attendee | Purpose |
|---|---|---|---|---|
| 1 | 去年两次宕机的根因是什么？是单点故障、数据库问题，还是架构层面的？ | Implicated Pain / Technical | CTO 陈思远 | 量化痛点，判断迁移的真实紧迫度和架构改造深度 |
| 2 | 现在平台架构长什么样？数据库（MySQL/PG/MongoDB?）、应用层、缓存、消息队列分别跑在哪里？ | Technical baseline | CTO 陈思远 | 评估迁移复杂度，为下次 architecture assessment 做准备 |
| 3 | 你们有没有跟阿里云聊过？走到哪一步了？有报价或 POC 吗？ | Competition / Decision Process | CTO 陈思远 | 了解竞争格局，判断我们的紧迫度和差异化重点 |
| 4 | 迁移决策林总（CEO）参与多少？她对 AWS vs 阿里云有没有倾向？ | Decision Process / Economic Buyer | CTO 陈思远 | 完善 stakeholder map，判断 CEO 是否需要单独 engage |
| 5 | Q3 完成迁移的 deadline 是硬性的吗？如果延迟会怎样？ | Compelling Event / Timeline | CTO 陈思远 | 验证 compelling event 的真实性 — 是董事会硬性要求还是内部愿望 |

### Information to Deliver

| # | What to Share | Format | Purpose |
|---|---|---|---|
| 1 | AWS Multi-AZ 高可用架构概述：failover 机制、RTO/RPO 指标 | Whiteboard / 架构图 | 直接回应 CTO 最大的顾虑 — "不能再出事" |
| 2 | 类似规模 SaaS 公司迁移案例（某 HR SaaS，50 万用户，12 周迁移，uptime 99.97%） | Case study summary (口头) | 建立信心：跟你们差不多的公司做过，成功了 |
| 3 | AWS MAP（Migration Acceleration Program）简介 | 1 sentence overview | 埋个种子 — 有迁移补贴和专业服务，后续跟 CEO 讨论成本时有用 |

> *Prospect stage: 不要过度 deliver。今天重点是**听**，不是**讲**。信息交付控制在 15 分钟内。*

---

## 5. Potential Objections & Responses

> *Based on CXO Persona (CTO) + Contact Profiling + competitive context.*

| # | Anticipated Objection | Our Response |
|---|---|---|
| 1 | **"迁移过程中不能停服务，我们的客户不能接受任何 downtime。"** *(CTO 陈思远, failure-scenario thinker)* | 完全理解 — 这也是我们最重视的。AWS 迁移的标准做法是 "并行运行"：先在 AWS 搭建完整环境，流量逐步切换（灰度/蓝绿部署），旧环境作为 fallback 至少保留两周。你们的客户不会感知到任何变化。那个 HR SaaS 的迁移就是零 downtime 完成的。 |
| 2 | **"我们内部有人推荐阿里云，说国内用起来更方便。"** *(Competition — advisor influence)* | 阿里云在国内确实有优势，特别是 ICP 备案和本地化支持。但 SaaS 平台有几个独特需求：第一，你们的企业客户可能对 "跑在哪朵云" 有偏好 — 国际化企业客户通常更信任 AWS；第二，AWS 的 SaaS 行业工具（Well-Architected SaaS Lens、SaaS Boost）是阿里云没有的；第三，如果星辰科技未来有出海计划，AWS 的全球 region 覆盖是现成的。当然，最终要看你们的具体需求 — 我们可以帮你做一个客观的 comparison。 |
| 3 | **"AWS 比阿里云贵吧？我们是创业公司，成本敏感。"** *(Cost concern)* | SaaS 公司的成本不只是云账单 — 还有宕机赔偿、客户流失、工程师 on-call 的时间成本。你们去年两次宕机赔了 ¥200 万，加上客户信任损失，远超云服务的差价。另外 AWS 有 MAP funding 可以 offset 迁移成本，也有 SaaS startup 专项 credits。我们下次可以拉上你们 CEO 详细聊 — 这个数字她可能很感兴趣。 |

---

## 6. Meeting Agenda

> *Virtual meeting, 1 hour. CTO 偏好高效沟通。前 5 分钟建立关系，然后快速进入正题。*

| Time | Topic | Owner | Purpose |
|---|---|---|---|
| 10:00–10:05 | 开场 & 自我介绍 | AE 张磊 | 建立关系，确认今天议程（"今天主要想听你聊聊现在遇到的问题"） |
| 10:05–10:25 | 星辰科技现状深入了解 | SA 李珊 (引导提问) + CTO 陈思远 | 验证痛点 + 收集技术细节（Discovery Q1-Q5）。**客户说 70%，我们说 30%** |
| 10:25–10:40 | AWS 高可用架构 & SaaS 迁移案例 | SA 李珊 | 回应痛点 — failover 机制 + HR SaaS 案例。用架构图，不用 PPT |
| 10:40–10:50 | 竞争与决策讨论 | AE 张磊 | 了解阿里云情况 + 决策链 + CEO 态度 |
| 10:50–10:55 | 总结 & 下一步 | AE 张磊 | 确认 architecture assessment 时间 |
| 10:55–11:00 | 结束 | AE 张磊 | — |

---

## 7. Potential Next Steps

| # | Proposed Next Step | Timeline | Owner | Purpose |
|---|---|---|---|---|
| 1 | Architecture assessment：详细评估现有架构 → 设计 AWS 目标架构 | 2 周内（Jun 2） | Joint (AWS SA + 星辰 CTO + VP Eng) | 进入 Technical Validation，同时让 VP Eng 参与 |
| 2 | 发送 SaaS 迁移案例详细报告 + MAP program 简介 | 3 天内 | AWS (AE 张磊) | 给 CTO 内部推动的弹药 |
| 3 | 如果 CTO 同意，安排一次 AE 与 CEO 的简短通话（15-20 分钟） | 2-3 周内 | AWS (AE 张磊) | 尽早 engage CEO，避免 advisor 影响固化 |

---

*Call Plan Template | Version: 1.1*
