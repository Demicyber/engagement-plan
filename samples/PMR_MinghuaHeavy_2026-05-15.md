# Post-Meeting Report — 明华重工 (Minghua Heavy Industries)

> **Related Document:** [CP_MinghuaHeavy_2026-05-15.md](CP_MinghuaHeavy_2026-05-15.md)
> **Date:** 2026-05-15
> **Recorded by:** AE 陈伟 (verbal debrief) + Agent

---

## 1. Outcome Assessment

> *💡 Auto-pulled from Call Plan Success Criteria, combined with sales feedback.*

| # | Objective / Success Criteria | Result | Notes |
|---|------|------|------|
| 1 | CTO 张敏明确表示愿意安排第二次 technical deep-dive，并给出具体时间 | ✅ Achieved | 张敏当场拍板：5 月 26 日技术 deep-dive，带他的架构师团队（3 人）参加 |
| 2 | VP Mfg 李华确认至少一条产线可用于 POC 测试 | ✅ Achieved | 李华指定了 3 号冲压线（退货率最高的线，4.1%），说 "就拿最难的来试" |
| 3 | 确认完整的决策链：CTO 技术认可 → CFO 预算审批 → Procurement 执行 | ⚠️ Partial | 决策链基本确认，但新增一个关键信息：$1M 以上投资 CEO 刘建国要过目。张敏说 "王总（CFO）签字够了，但老刘（CEO）大概率会过问一下"。Procurement 赵芳的角色仍未确认。 |

**Stage Progression:** ( Qualified ) → ( Technical Validation ) — ✅ Achieved — CTO 同意进入技术验证阶段

---

## 2. Meeting Notes

### Customer Sentiment

| Attendee | Sentiment | Evidence |
|----------|-----------|----------|
| CTO 张敏 | Positive | 全程积极参与，白板讨论时亲自画了现有架构图。会后单独跟 SA 刘洋 exchanged WeChat，说 "终于遇到懂制造业的 SA 了"。主动提出下次 deep-dive 的时间。 |
| VP Mfg 李华 | Cautious → Positive | 开场时明显怀疑（"之前也有人来讲 AI，都是纸上谈兵"），但看到东风案例的产线部署视频后态度转变。周明讲边缘推理部署方式时，李华追问了 15 分钟细节，最后说 "这个不影响产线，我可以配合试"。关键转折点是边缘部署视频。 |

### Key Findings

| Finding | Source (who said it) | Implication (what this means for our strategy) |
|---------|---------------------|-----------------------------------------------|
| 3 号冲压线退货率实际是 4.1%，高于之前了解的整体 3.2% | VP Mfg 李华 | POC 如果在最差的线上成功，说服力更强。但也意味着模型训练难度更高 — SA 需要评估数据质量。 |
| 华为云 POC 失败的核心原因：模型在实验室准确率 95%，上产线后降到 72%（光线/角度变化）| CTO 张敏 | 关键竞争情报。我们的 POC 必须在**真实产线环境**测试，不能只在实验室。这也是我们的差异化机会 — 用 SageMaker 的 data augmentation + edge inference 解决这个问题。 |
| CEO 刘建国可能在最终决策时参与（$1M+ 投资） | CTO 张敏 | EP 需要更新 — 原来以为 CFO 是最终审批人，现在 CEO 也可能参与。可能需要安排 EBC。 |
| 明华正在筹建越南工厂，2027 Q2 投产 | CTO 张敏（闲聊时提到） | 潜在 upsell 机会。如果 AI 质检方案能复用到越南工厂，deal size 可以显著提升。记录到 EP 供后续跟进。 |
| 质检图片数据约 50 万张，已有基础标注（合格/不合格），但缺乏细粒度缺陷分类标注 | CTO 张敏 | 数据就绪度中等。POC 第一阶段可以用二分类（合格/不合格），fine-grained 分类作为 phase 2。影响 POC scope 定义。 |
| 李华关注一线工人培训成本："别搞得工人都要学编程" | VP Mfg 李华 | UX 和培训方案要在 POC proposal 里体现。强调 "看得见、点得动、不需要技术背景" 的质检看板。 |

---

## 3. What Changed — EP Update

> *Only dimensions with actual changes listed.*

| Dimension | What Changed |
|-----------|-------------|
| **Stakeholder: VP Mfg 李华** | Stance: Neutral → Cautious-Positive。指定 3 号冲压线用于 POC，表示愿意配合。 `[Updated: 2026-05-15]` |
| **Stakeholder: VP Mfg 李华 — Profiling** | 新增：对 demo/视频的反应很好，"眼见为实" 型。初期怀疑但可以被真实案例说服。边缘部署视频是转折点。 `[Updated: 2026-05-15]` |
| **Stakeholder: CTO 张敏 — Profiling** | 新增：跟 SA 刘洋建立了个人关系（exchanged WeChat）。白板讨论时喜欢亲自画图。技术信任度高。 `[Updated: 2026-05-15]` |
| **Decision Process** | 新增关键信息：$1M+ 投资 CEO 刘建国可能过问。决策链更新为：CTO 技术认可 → CFO 预算审批 → CEO 过目 → Procurement 执行。 `[Updated: 2026-05-15]` |
| **Competitive** | 华为云 POC 失败原因明确：模型在产线真实环境下准确率大幅下降（95% → 72%）。我们的差异化要点：真实环境测试 + data augmentation + edge inference。 `[Updated: 2026-05-15]` |
| **New Stakeholder** | CEO 刘建国加入 stakeholder map（Engagement Priority: Important，Role: Final Approver for $1M+）。`[Updated: 2026-05-15]` |
| **Expansion Opportunity** | 越南工厂 2027 Q2 投产 — 潜在 upsell，AI 质检方案全球复用。 `[Updated: 2026-05-15]` |
| **Stage** | Qualified → Technical Validation `[Updated: 2026-05-15]` |

### Agent Recommendation

本次会议非常成功 — CTO 作为 Champion 的角色进一步巩固，VP Manufacturing 从 Neutral 转向 Positive 并指定了 POC 产线，stage 顺利推进到 Technical Validation。

**建议不要急于推进 stage，先稳扎稳打做好 Technical Validation：**
1. 下次 tech deep-dive（May 26）重点共同定义 POC scope 和 success criteria，特别是在**真实产线环境**测试（这是打败华为云的关键）
2. CEO 参与是新变量 — 建议在 Engagement Roadmap 中增加一个 EBC 节点（大约在 POC 成功后），让 AE 跟张敏确认 CEO 见面的最佳时机
3. 越南工厂是 upsell 机会，但不要在 POC 前提出 — 等 POC 成功后在 EBC 场景自然引入

**下次会议应聚焦：** 与 CTO 团队共同定义 POC scope（产线环境、数据要求、成功标准、timeline），确认 AWS 侧需要提前准备什么（数据传输、边缘设备、SA onsite 支持）。

---

## 4. Action Items

| # | Priority | Action Item | Owner | ETA | Status |
|---|----------|------------|-------|-----|--------|
| 1 | High | 准备 Technical Deep-Dive 议程 + SageMaker MLOps 架构方案 | SA 刘洋 (AWS) | May 22 | Open |
| 2 | High | 确认 3 号冲压线的技术条件（网络、质检站点数量、图片采集设备） | CTO 张敏 (Customer) | May 22 | Open |
| 3 | High | 评估 50 万张标注数据的质量，输出 POC 数据就绪度报告 | SA Specialist 周明 (AWS) | May 22 | Open |
| 4 | Medium | 发送东风案例详细报告给张敏 | AE 陈伟 (AWS) | May 17 | Open |
| 5 | Medium | 更新 EP：加入 CEO 刘建国到 stakeholder map，增加 EBC 节点 | Agent | May 16 | Open |
| 6 | Low | 准备 "一线工人培训方案" 概要，用于后续 VP Mfg 沟通 | SA Specialist 周明 (AWS) | Jun 1 | Open |

---

## 5. Customer Recap Email (Handoff)

> *💡 Handoff to Writer Skill (not yet available — agent drafts directly).*

**Key context for recap email:**
- 感谢张总和李总的时间
- 总结三个共识：质检是优先项、技术方案可行、5/26 deep-dive 确认
- 附上东风案例报告（Action Item #4）
- 确认下次 deep-dive 日期和参会人
- Tone: 专业但不生硬，体现合作伙伴感而非供应商感
- ⚠️ 不要提及：竞争对手分析、内部定价策略、CEO 参与的判断

---

*Post-Meeting Report Template | Version: 1.1*
