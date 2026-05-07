# Engagement Plan: SHEIN - Global Infrastructure Optimization & GDPR Compliance

> **What is this?** A focused action plan for winning a specific opportunity.

## 1. Opportunity Snapshot

| Dimension | Detail |
|-----------|--------|
| **Customer** | SHEIN (希音) — Global fast fashion e-commerce |
| **Opportunity Name** | Global CDN Optimization + Recommendation System + GDPR Compliance |
| **Deal Value** | $3.2M ARR |
| **Current Stage** | Business Validation |
| **Target Close Date** | 2026-07-15 |
| **Why Now** | EU Digital Services Act enforcement Aug 2026; SHEIN IPO prep requires compliance posture; Google Cloud actively pitching alternative |
| **Deal Objective** | Land full-stack compliance + infrastructure modernization bundle |
| **Win Strategy** | Leverage completed technical validation to lock GDPR module timeline; use reference architecture from similar e-commerce customer (Zalando) to de-risk; neutralize Google Cloud's pricing play with TCO + compliance breadth story |

## 2. Engagement Plan

### Key Stakeholders

#### 王凯 Kevin Wang — CTO

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | ★★★ Champion — Primary decision maker |
| **Role in This Deal** | Final sign-off on architecture direction and budget allocation |
| **Current Stance** | Supportive — technically convinced, needs business justification for board |
| **What They Care About** | Platform reliability at scale; IPO-readiness; not being locked into single vendor |
| **Profiling** | 前阿里 P9，技术出身但现在更关注商业价值。喜欢数据驱动的论证，不喜欢 vendor 的空话。Decision style: consensus-builder, will defer to domain leads then consolidate. |
| **What We Need From Them** | Board-level budget approval; internal champion to push legal team timeline |
| **How to Win Them** | Provide TCO model with 3-year projection; show competitive risk of delay; give him "board-ready" materials he can reuse |

#### 张锐 Ray Zhang — Head of Infrastructure

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | ★★★ Technical Champion — Owns implementation |
| **Role in This Deal** | Technical decision maker; owns infrastructure budget line |
| **Current Stance** | Strong advocate — led technical validation, impressed with CDN performance |
| **What They Care About** | Operational simplicity; team skill gaps; migration risk |
| **Profiling** | 基础设施老兵，10+ years experience。务实派，关注落地而非 PPT。已经在内部推动 AWS 方案，但担心 GDPR 模块增加运维复杂度。 |
| **What We Need From Them** | Implementation timeline sign-off; resource commitment for migration team |
| **How to Win Them** | Managed service approach to reduce ops burden; training plan for his team; phased rollout to minimize risk |

#### Sarah Li 李莎 — GDPR Compliance Lead

| Dimension | Assessment |
|-----------|-----------|
| **Engagement Priority** | ★★☆ Key Influencer — Domain authority on compliance |
| **Role in This Deal** | Compliance requirements owner; interfaces with EU legal counsel |
| **Current Stance** | Cautious positive — wants to see reference case before committing timeline |
| **What They Care About** | Audit trail completeness; data residency guarantees; legal defensibility |
| **Profiling** | 法律背景转合规，在 SHEIN 2年。非常谨慎，需要 evidence-based assurance。上次会议后私下问了很多关于 data sovereignty 的细节问题。与外部法律顾问 (Clifford Chance) 关系紧密。 |
| **What We Need From Them** | Compliance requirements sign-off; timeline agreement for GDPR module |
| **How to Win Them** | Reference case from comparable e-commerce company; direct engagement with AWS compliance team; written data residency commitments |

### Engagement Roadmap

| Phase | Milestone | Date | Status |
|-------|-----------|------|--------|
| Discovery | Initial meeting — scope alignment | 2026-02-12 | ✅ Done |
| Technical Validation | CDN + Rec System POC | 2026-03-05 | ✅ Done |
| Technical Validation | Architecture review with SA team | 2026-03-26 | ✅ Done |
| Technical Validation | Security & compliance deep-dive | 2026-04-16 | ✅ Done |
| **Business Validation** | **GDPR timeline commitment + commercial terms** | **2026-05-21** | 🔄 Next |
| Negotiation | MSA + SOW finalization | 2026-06-15 | ⏳ Planned |
| Close | Contract signature | 2026-07-15 | ⏳ Planned |

## 3. MEDDPICC Tracker

| Element | Status | Detail |
|---------|--------|--------|
| **Metrics** | ✅ Strong | 35% latency reduction proven in POC; $1.8M/yr compliance cost avoidance vs. build-in-house |
| **Economic Buyer** | ✅ Identified | CFO 刘洋 — Kevin has direct line, will present business case |
| **Decision Criteria** | ✅ Defined | TCO, compliance coverage, migration risk, vendor lock-in concerns |
| **Decision Process** | ✅ Mapped | Domain lead → CTO → CFO → Board (quarterly cycle, next board: June 20) |
| **Paper Process** | 🟡 In Progress | Legal reviewing MSA template; procurement cycle ~4 weeks |
| **Identified Pain** | ✅ Quantified | EU DSA deadline Aug 2026; current compliance gap = IPO risk |
| **Champion** | ✅ Active | Ray Zhang — actively selling internally, provided org chart and budget cycle info |
| **Competition** | ⚠️ Active | Google Cloud pitching Assured Workloads + Chronicle; ~20% lower list price but narrower compliance scope |

## 4. Account Intelligence

### Competitive Landscape
- **Google Cloud**: Active competitor. Pitching Assured Workloads for GDPR + Chronicle for audit. Strength: pricing (~20% below). Weakness: narrower compliance certifications, no equivalent to AWS Artifact for audit evidence.
- **Counter-strategy**: Emphasize breadth (200+ compliance certifications vs. GCP's ~100); reference Zalando case; highlight hidden costs of GCP compliance gaps requiring 3rd-party tooling.

### Technical Environment
- Current: Multi-cloud (AWS 60%, Alibaba Cloud 30%, GCP 10% for specific ML workloads)
- CDN: Migrating from Cloudflare to CloudFront (Phase 1 complete)
- Data: Primarily on AWS (S3 + Redshift); some legacy on-prem in Shenzhen DC

### Recent Activities
- 2026-04-16: Security deep-dive completed. Sarah Li raised 3 data residency questions — all answered via follow-up doc.
- 2026-04-28: Ray shared internal infrastructure roadmap (H2 2026). GDPR module is a board-level priority.
- 2026-05-02: Competitive intel — Google Cloud rep met with Sarah Li's team. Focus was on pricing.

### Risk Register

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|-----------|
| Legal team delays timeline past board cycle | Medium | High | Provide reference case + pre-drafted compliance attestation |
| Google Cloud undercuts on price | High | Medium | TCO analysis showing 3-year cost advantage with compliance bundle |
| IPO timeline shifts, reducing urgency | Low | High | Anchor to EU DSA deadline (independent of IPO) |
