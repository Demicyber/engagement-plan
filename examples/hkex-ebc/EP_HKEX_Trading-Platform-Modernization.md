# Engagement Plan: HKEX - Core Trading Platform Modernization

> **What is this?** A focused action plan for winning a specific opportunity.

## 1. Opportunity Snapshot

| Dimension | Detail |
|-----------|--------|
| **Customer** | Hong Kong Exchanges and Clearing Limited (HKEX 港交所) |
| **Opportunity Name** | Core Trading Platform Modernization + Market Data Analytics + DR |
| **Deal Value** | $4.5M ARR |
| **Current Stage** | Technical Validation |
| **Target Close Date** | 2026-09-30 |
| **Why Now** | HKEX Orion Trading Platform approaching end-of-cycle refresh; board mandate to reduce RTO/RPO for market continuity; Azure contract renewal in Q4 creates switching window |
| **Deal Objective** | Win core trading infrastructure modernization (compute + networking), market data lake analytics, and cross-region DR — displacing Azure for latency-sensitive workloads |

## 2. Engagement Plan

### Key Stakeholders

#### Dr. James Wong 黄志明 — CTO

| Dimension | Detail |
|-----------|--------|
| **Role & Influence** | CTO, final technical authority; reports directly to CEO |
| **Decision Power** | Technical Decision Maker (TDM) — signs off on architecture |
| **Priority** | Modernize trading infrastructure without disrupting market operations |
| **Pain Points** | Current Azure latency inconsistency during peak trading; vendor lock-in concerns |
| **Communication Style** | Data-driven, concise; prefers whitepapers and benchmarks over slides |
| **Attitude to AWS** | Cautiously positive — impressed by AWS financial services track record globally |
| **Engagement History** | Attended re:Invent 2025; met AWS FSI team at SIBOS Hong Kong |

#### Karen Chan 陈嘉欣 — Head of Cloud Strategy

| Dimension | Detail |
|-----------|--------|
| **Role & Influence** | Owns cloud vendor strategy and budget allocation |
| **Decision Power** | Economic Buyer (EB) for cloud spend; influences CTO |
| **Priority** | Cost optimization, multi-cloud governance, regulatory compliance |
| **Pain Points** | Fragmented cloud governance; HKMA regulatory reporting overhead |
| **Communication Style** | Strategic, business-outcome focused; bilingual presentations preferred |
| **Attitude to AWS** | Open but cautious — wants clear differentiation vs. Azure incumbent |
| **Engagement History** | Briefed by Hao Lin in Q1; requested EBC to evaluate AWS FSI capabilities |

#### Robert Yip 叶伟聪 — Chief Architect

| Dimension | Detail |
|-----------|--------|
| **Role & Influence** | Owns technical architecture decisions; team of 40 engineers |
| **Decision Power** | Champion or Blocker — technical veto power |
| **Priority** | Low-latency compute, FIX protocol optimization, data sovereignty |
| **Pain Points** | Concerned about cloud vendor lock-in; wants portable architectures |
| **Communication Style** | Deep technical; asks hard questions; values hands-on demos |
| **Attitude to AWS** | Skeptical — prefers open-source/cloud-agnostic patterns |
| **Engagement History** | Attended AWS FSI Immersion Day (March 2026); raised lock-in concerns |

### Engagement Roadmap

| Date | Milestone | Owner | Status |
|------|-----------|-------|--------|
| 2026-05-12 | Pre-EBC technical prep call with Robert Yip | 赵鹏 + Andrew Zhang | ✅ Done |
| 2026-05-28 | **EBC @ AWS HK Office** | Full team | 🎯 Next |
| 2026-06-10 | Proof of Concept kick-off (latency benchmarks) | Andrew Zhang | Planned |
| 2026-07-15 | POC results review + commercial proposal | 林浩 + Karen Chan | Planned |
| 2026-09-30 | Target close | 林浩 | Planned |

## 3. MEDDPICC Tracker

| Element | Status | Detail |
|---------|--------|--------|
| **Metrics** | 🟡 | Target: <50μs jitter for order matching; 99.999% availability; RTO <15min |
| **Economic Buyer** | 🟢 | Karen Chan — engaged, requested EBC |
| **Decision Criteria** | 🟡 | Latency, data sovereignty (HK), regulatory compliance, portability |
| **Decision Process** | 🟢 | CTO recommends → CFO approves >$2M; board visibility |
| **Paper Process** | 🔴 | Procurement requires 3-vendor evaluation; legal review 6-8 weeks |
| **Implicate Pain** | 🟢 | Azure latency spikes during market open caused 2 near-incidents in 2025 |
| **Champion** | 🟡 | Karen Chan is sponsor; need Robert Yip as technical champion |
| **Competition** | 🟡 | Azure incumbent (60% workloads); GCP exploring market data analytics angle |

## 4. Account Intelligence

### Competitive Landscape
- **Azure**: Incumbent for ~60% of HKEX cloud workloads (non-latency-sensitive); 3-year EA expiring Q4 2026
- **GCP**: Pitched BigQuery for market data analytics; early conversations only
- **AWS opportunity**: Win latency-sensitive trading workloads + DR where Azure has underperformed

### Technical Context
- Orion Trading Platform (proprietary, C++/Java); FIX 4.4 protocol
- Current DR: Active-passive across two HK data centers; exploring cloud-based DR
- HKMA regulatory requirements: data must remain in Hong Kong jurisdiction
- Peak load: 3M+ orders/day during market hours (09:30-16:00 HKT)

### Recent Activities
- 2026-03: Robert Yip attended AWS FSI Immersion Day — positive but raised lock-in concerns
- 2026-04: Karen Chan requested EBC after seeing AWS exchange customer references (SGX, ASX)
- 2026-05-12: Technical prep call — agreed on EBC agenda focusing on low-latency compute + DR

### Risks & Mitigations
| Risk | Likelihood | Mitigation |
|------|-----------|------------|
| Robert Yip blocks on lock-in concerns | Medium | Demo Kubernetes-based portable architecture; show open-source tooling |
| Azure counter-offers aggressive pricing | High | Lead with technical differentiation (latency); PPA commercial terms |
| Regulatory uncertainty delays decision | Low | Engage AWS HK compliance team; pre-clear with HKMA framework |
