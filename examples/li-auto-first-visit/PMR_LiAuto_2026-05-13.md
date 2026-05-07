# Post-Meeting Report — 理想汽车 (Li Auto) 首次拜访

> **Related Document:** [EP_LiAuto_Intelligent-Driving-DataLake.md](./EP_LiAuto_Intelligent-Driving-DataLake.md) | [CP_LiAuto_2026-05-13.md](./CP_LiAuto_2026-05-13.md)  
> **Date:** 2026-05-13 14:00–15:40  
> **Recorded by:** 张磊 (AE) + 李珊 (SA)

---

## 1. Outcome Assessment

| Criteria (from Call Plan) | Result | Notes |
|--------------------------|--------|-------|
| 获得数据架构和规模基本信息 | ✅ Achieved | 孙浩详细介绍了现有架构 |
| 了解多云评估 timeline 和参与者 | ✅ Achieved | Q3 完成评估，Q4 决策 |
| 识别具体痛点 | ✅ Achieved | 数据回灌延迟 + 存储成本是核心痛点 |
| 赵明辉愿意继续交流 | ✅ Achieved | 明确表示 "值得深入看看" |
| 确定下一步并约定时间 | ✅ Achieved | 5/27 技术交流会 |
| 客户对 AWS 智驾能力有正面认知 | 🟡 Partial | 认可案例，但对中国区落地能力仍有疑虑 |

### Stage Progression

| Before | After | Evidence |
|--------|-------|----------|
| Prospect | Qualify | 确认真实需求 + 明确 timeline + 下一步会议已约 |

---

## 2. Meeting Notes

### Customer Sentiment

| Stakeholder | Sentiment | Key Signals |
|------------|-----------|-------------|
| 赵明辉 (VP) | 🟢 Positive | 多待了 10 分钟（原计划只参加 30 min），主动问了 pricing model，会后安排孙浩对接 |
| 孙浩 (Arch Director) | 🟡 Cautious-Positive | 技术问题问得很细，关注多云架构一致性；对 Lake Formation 表示兴趣但担心 vendor lock-in |
| 周小林 (Data Eng Mgr) | 🟢 Positive | 主动提了三个具体痛点，会后加了李珊微信，问 S3 vs OSS 性能对比数据 |

### Key Findings

| Topic | Finding | Impact on Deal |
|-------|---------|---------------|
| 数据规模 | 智驾数据日增 50TB+，年底预计翻倍；目前 80% 在阿里云 OSS | 规模符合预期，$1.5M ARR 合理 |
| 核心痛点 | ① 路测数据回灌训练集群延迟 4-6h（目标 <1h）② 存储成本年增 40% 无法持续 | 明确且紧迫的 pain points |
| 技术栈 | Spark + Flink + 自研标注平台；考虑引入 Iceberg | 与 AWS 方案契合度高 |
| 多云评估 | 已与华为云有初步接触；Azure 暂未进入；阿里云是 incumbent | 竞争格局基本确认 |
| 决策流程 | 技术评估 → 孙浩团队；商务决策 → 赵明辉 + CFO 联签（>$500K） | CFO 是新 stakeholder，需后续 map |
| OTA 场景 | 当前 OTA 自研为主，但全球化部署有需求（欧洲市场） | 可作为第二切入点 |
| 预算 | FY2026 下半年有专项预算（多云评估 + POC） | 预算已有，不需要等下一财年 |

---

## 3. What Changed — EP Update

| EP Field | Before | After |
|----------|--------|-------|
| Current Stage | Prospect | Qualify |
| 赵明辉 Stance | Neutral [待确认] | Positive-Neutral — 开放但未承诺 |
| 孙浩 Stance | [待确认] | Cautious — 关注 lock-in 和落地能力 |
| 周小林 Stance | [待确认] | Positive — 有实际痛点，愿意探索 |
| Champion | None | 周小林 (potential) — 主动加微信，有内部推动意愿 |
| Competition | 阿里云 + 华为云 + Azure [待确认] | 阿里云 (incumbent) + 华为云 (active) |
| Decision Process | Unknown | 技术评估 Q3 → 商务决策 Q4，VP + CFO 联签 |
| Identified Pain | Hypothesized | Confirmed: 数据回灌延迟 + 存储成本 |
| Deal Value | $1.5M ARR (estimated) | $1.5M ARR (validated — 规模支撑) |

### 🤖 Agent Recommendation

> 机会经过首次验证，质量较高。建议：
> 1. 将此机会升级为 Qualify stage，正式进入 pipeline
> 2. 在 5/27 技术交流会前准备：① 针对数据回灌延迟的 S3 + EMR Serverless 方案 ② 存储成本 TCO 对比
> 3. 尽早安排一次与周小林的 1:1 技术深聊，培养 Champion
> 4. 关注华为云动态 — 可通过渠道伙伴了解对方进展

---

## 4. Next Steps

| # | Action | Owner | Deadline | Status |
|---|--------|-------|----------|--------|
| 1 | 发送会议纪要 + AWS 智驾数据湖白皮书给孙浩 | 张磊 | 2026-05-14 | 🔲 Pending |
| 2 | 准备 S3 vs OSS 性能对比材料发给周小林 | 李珊 | 2026-05-16 | 🔲 Pending |
| 3 | 确认 5/27 技术交流会议程和参与人 | 张磊 | 2026-05-20 | 🔲 Pending |
| 4 | 准备数据回灌场景 Demo（S3 + EMR Serverless + Iceberg）| 李珊 | 2026-05-25 | 🔲 Pending |
| 5 | 内部 brief SSM 和 GTMS，争取 POC credit 资源 | 张磊 | 2026-05-20 | 🔲 Pending |
| 6 | 约周小林线下 coffee chat | 李珊 | 2026-05-19 | 🔲 Pending |
