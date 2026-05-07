# Post-Meeting Report — 理想汽车 (Li Auto)

> **Related Document:** [CP_LiAuto_2026-05-13.md](CP_LiAuto_2026-05-13.md)
> **Date:** 2026-05-13
> **Recorded by:** AE 张磊 (verbal debrief via WeChat voice message) + Agent

---

## 1. Outcome Assessment

> *💡 Auto-pulled from Call Plan Success Criteria, combined with sales feedback.*

| # | Objective / Success Criteria | Result | Notes |
|---|------|------|------|
| 1 | 赵明辉或孙浩同意安排第二次技术 deep-dive，并给出具体时间 | ✅ Achieved | 孙浩当场说 "5 月 27 号可以，我带我的架构组一起来"。赵明辉点头认可但没承诺本人参加 deep-dive（"你们先把技术聊透"）。 |
| 2 | 确认数据闭环延迟（>48h）是真实痛点，且有明确的改进 urgency | ✅ Achieved | 痛点比预想的更严重 — 实际是 72h+（不是之前了解的 48h），原因是标注回传链路有额外一层审批。赵明辉原话："这个速度，Q3 的 OTA 大版本肯定来不及。" |
| 3 | 了解多云评估的完整决策流程（参与者、标准、timeline） | ⚠️ Partial | 确认了技术委员会评估（赵明辉是主席），Q2 出初步结论。但**评估标准**没有明确给出 — 赵明辉说 "还在定义中，你们的输入也是我们参考的一部分"。采购流程和最终审批人未能确认。 |

**Stage Progression:** ( Prospect ) → ( Qualified ) — ✅ Achieved — 客户同意进入正式技术交流，pain validated，next step confirmed

---

## 2. Meeting Notes

### Customer Sentiment

| Attendee | Sentiment | Evidence |
|----------|-----------|----------|
| VP 赵明辉 | Neutral → Cautious-Positive | 前 20 分钟比较保留（短句回应、不主动展开），但陈航讲蔚来案例时身体前倾，追问了两个细节问题。会后跟张磊握手时说 "你们这个团队还行，不是来念 PPT 的"。没有承诺参加 deep-dive 但没有 push back。 |
| Dir 孙浩 | Positive | 全程最活跃的人。白板环节主动拿笔画了现有架构图（未被要求），解释了 MaxCompute 的 3 个具体痛点。对 S3+Iceberg 架构方向眼睛亮了一下，说 "你们支持 Iceberg 这个我知道，但没想到 Lake Formation 能跟 Iceberg 这么原生集成"。会后单独加了李珊微信，发了一篇他写的 InfoQ 文章说 "这是我去年写的，现在想法更进了一步，下次聊"。 |
| Mgr 周小林 | Neutral | 全程话不多（约 5-6 句），主要是在孙浩讲架构时补充数据细节。但记了很多笔记。最后问了一个很实际的问题："如果做 POC，我需要提前准备什么？我怕临时抱佛脚。" — 说明他已经在想执行层面了。 |

### Key Findings

| Finding | Source (who said it) | Implication (what this means for our strategy) |
|---------|---------------------|-----------------------------------------------|
| 数据闭环实际是 72h+（不是之前了解的 48h），瓶颈在标注数据回传有一层质量审批（人工抽检 10%） | 孙浩 + 周小林补充 | 痛点比预想更大。"6h 闭环" 的架构故事更有说服力。但需注意：人工审批环节不是纯技术能解决的 — 方案要包含 "AI 辅助质量审核" 减少人工抽检比例。 |
| 孙浩对阿里云 MaxCompute 的 3 个痛点：(1) 表元数据管理混乱 (2) 缺乏细粒度权限控制 (3) Spark 兼容性差导致算法团队无法自服务 | 孙浩（白板上画了现有架构并标出 pain points） | **关键竞争情报**。孙浩的痛点跟 Lake Formation 的 value prop 精准匹配。他大概率可以发展为 Champion — 他的不满不是泛泛的 "想试试别的"，而是有具体的技术诉求。 |
| 多云评估 timeline: Q2 出初步技术结论，Q3 做 POC 验证，Q4 签约执行 | 赵明辉 | Timeline 跟我们预估基本吻合。但 "Q2 出初步技术结论" 意味着 5 月 27 日的 deep-dive 非常关键 — 可能直接影响他们把谁列入正式评估 shortlist。 |
| 赵明辉提到 "CTO 不太管智驾这块的供应商选择，是我这边定" | 赵明辉（在 decision process 讨论中） | 好消息 — 决策链比预想的短。VP 级别就能拍板，不需要再往上走 CTO/CEO。但需要验证预算审批是否也在他权限内 `[待确认]`。 |
| 智驾数据日增量约 15TB（200 台路测车，每台日均 75GB），总存量约 8PB | 周小林 | 规模数据对方案设计和定价至关重要。8PB 存量 + 15TB/日增量 → S3 Intelligent-Tiering 可以显著降低存储成本（冷数据自动分层）。这也是 business case 的一个支点。 |
| 赵明辉在智驾圈子跟小鹏副总裁有私交，可能了解小鹏的数据闭环方案 | 赵明辉（提到 "我跟 XX 聊过，他们也在做类似的事"） | 竞争情报：小鹏可能也在我们的 pipeline 里。但更重要的是 — peer pressure 可以利用。如果小鹏在用 AWS（需确认），这对赵明辉有影响力。 |

---

## 3. What Changed — EP Update

> *Only dimensions with actual changes listed.*

| Dimension | What Changed |
|-----------|-------------|
| **Stakeholder: Dir 孙浩 — Stance** | Unknown → Positive。主动画架构图、展示痛点、加 SA 微信、分享文章。极高概率可发展为 Champion。 `[Updated: 2026-05-13]` |
| **Stakeholder: Dir 孙浩 — Profiling** | 新增：白板讨论型（主动拿笔画图），乐于分享技术观点。对 Lake Formation + Iceberg 集成有明确兴趣。沟通风格开放，不设防。确认 Iceberg 偏好。 `[Updated: 2026-05-13]` |
| **Stakeholder: VP 赵明辉 — Profiling** | 新增：开场保留但可以被技术深度打动（案例环节态度转变）。不喜欢被 "销售"，但尊重懂行的人（"不是来念 PPT 的"）。决策风格 — 让下面人先看技术，自己把关战略方向。 `[Updated: 2026-05-13]` |
| **Stakeholder: Mgr 周小林 — Profiling** | 新增：会议中偏沉默但在记笔记。已经在想执行层面（"POC 需要我准备什么"）。实用主义者。 `[Updated: 2026-05-13]` |
| **Pain Point** | 数据闭环延迟从 48h 上修为 72h+。增加新发现：瓶颈含人工审批环节（10% 抽检），不纯是技术问题。 `[Updated: 2026-05-13]` |
| **Decision Process** | 赵明辉确认自己是最终决策人（"CTO 不太管智驾供应商"），无需再往上。但预算审批权限未确认。Timeline: Q2 技术结论 → Q3 POC → Q4 签约。 `[Updated: 2026-05-13]` |
| **Competition** | 阿里云（MaxCompute）的具体痛点已明确（3 点）。华为云未被提及 — 可能竞争压力没预想大 `[待确认]`。小鹏可能有可借鉴的 peer reference。 `[Updated: 2026-05-13]` |
| **Stage** | Prospect → Qualified `[Updated: 2026-05-13]` |

### Agent Recommendation

非常好的首次会面 — 从一个冷启动的新客户，一次会议就完成了 Prospect → Qualified 推进，并发现了一个高潜力 Champion（孙浩）。赵明辉的反应虽然没有孙浩那么热烈，但 "不是来念 PPT 的" 这句评价在 VP 层面已经是很高的认可了。

**三个关键策略建议：**

1. **All-in 发展孙浩为 Champion。** 他主动加了李珊微信并分享文章 — 这是非常积极的信号。5/27 的 deep-dive 要以孙浩为中心设计。建议李珊本周内就跟孙浩做一次非正式的 1-on-1 技术交流（微信语音或咖啡），进一步了解他的诉求，同时把 Lake Formation + Iceberg 的技术细节提前分享。目标：让孙浩在技术委员会上主动为 AWS 方案说话。

2. **方案要解决 "人工审批" 瓶颈，不能只讲基础设施。** 72h 延迟中有一部分是人工抽检造成的 — 如果我们的方案只加速数据传输和处理，不解决审批环节，客户体感改善有限。建议在 deep-dive 中加入 "SageMaker Ground Truth + AI 辅助质量审核" 的模块，让标注质量审批从 10% 人工抽检变成 AI 全量审核 + 异常人工复核。这能把方案从 "infrastructure play" 提升为 "workflow transformation"。

3. **不要急于提 PPA 或商业条款。** 赵明辉的决策风格是 "让下面人先验证技术"。在孙浩还没有给出明确技术认可之前，过早推商业只会让赵明辉觉得我们 "又是来卖东西的"。建议至少等 deep-dive 完成、POC scope 共同定义后再进入商业讨论（约 Week 5-6）。

---

## 4. Action Items

| # | Priority | Action Item | Owner | ETA | Status |
|---|----------|------------|-------|-----|--------|
| 1 | High | 准备 5/27 Technical Deep-Dive 议程 + 架构方案（重点：S3+Iceberg+Lake Formation + SageMaker pipeline） | SA 李珊 (AWS) | May 20 | Open |
| 2 | High | 本周内与孙浩做一次非正式 1-on-1 技术交流（微信），加深关系 | SA 李珊 (AWS) | May 16 | Open |
| 3 | High | 发送蔚来数据湖案例技术报告（脱敏版）给孙浩 | SA Specialist 陈航 (AWS) | May 15 | Open |
| 4 | Medium | 更新 EP：新增痛点细节（72h+, 人工审批瓶颈）、孙浩 Champion 发展计划、决策流程 | Agent | May 14 | Open |
| 5 | Medium | 评估 "AI 辅助标注质量审核" 方案可行性，为 deep-dive 准备 1 页概念 | SA Specialist 陈航 (AWS) | May 22 | Open |
| 6 | Low | 确认小鹏汽车是否在 AWS 上做智驾数据湖（内部查询，为 peer reference 做准备） | AE 张磊 (AWS) | May 20 | Open |

---

## 5. Customer Recap Email (Handoff)

> *💡 Handoff to Writer Skill (not yet available — agent drafts directly).*

**Key context for recap email:**
- 感谢赵总、孙总和周经理的时间，表达对理想智驾技术方向的认可
- 总结三个共识：数据闭环速度是关键瓶颈、AWS 开放架构方向契合理想需求、5/27 deep-dive 确认
- 附上蔚来案例技术摘要（Action Item #3）
- 确认 5/27 deep-dive 的参会人、时间和地点
- Tone: 技术伙伴感 > 供应商感。赵明辉不喜欢被 "销售"，邮件措辞要偏技术务实
- ⚠️ 不要提及：竞争对手分析（尤其不要提阿里云的痛点 — 那是孙浩私下说的）、商业条款、定价预估、小鹏的任何信息

---

*Post-Meeting Report Template | Version: 1.1*
