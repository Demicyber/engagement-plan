# Engagement Plan: 港交所 (HKEX) - Core Trading Platform Modernization

> **What is this?** A focused action plan for winning a specific opportunity. Answers: who do I need to win, what do I need from each person, and what's my engagement roadmap to get there?
>
> 🤖 *Automatically generated. Updated after each visit.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise.*

---

## 1. Opportunity Snapshot

| Field | Value |
|---|---|
| **Customer** | 香港交易及結算所有限公司 (Hong Kong Exchanges and Clearing Limited / HKEX) |
| **Opportunity Name** | Core Trading Platform Modernization + Market Data Analytics + DR |
| **Deal Value** | $4.5M ARR |
| **Current Stage** | Technical Validation |
| **Target Close Date** | 2026-Q3 |
| **Why Now** | HKEX's existing Azure enterprise agreement is up for renewal in Q4 2026. Concurrently, their Orion Trading Platform (OTP) is undergoing a multi-year modernization — latency spikes during market open on Azure (measured at 800μs P99 vs. target <500μs) have caused visible order book delays twice in 2026. The SFC issued new operational resilience guidelines (Dec 2025) requiring geographic DR within HK SAR with <15min RTO. Azure's nearest DR option is Southeast Asia, which doesn't meet the data residency requirement. |
| **Deal Objective** | Sign $4.5M PPA by end of Q3 2026 covering: (1) low-latency matching engine infrastructure on AWS HK Region with Nitro/Graviton4, (2) real-time market data analytics pipeline (tick data → insights), (3) intra-HK disaster recovery meeting SFC operational resilience guidelines. |

### Win Strategy

HKEX's core pain is **latency unpredictability on Azure during peak trading hours** — the two visible order book delays in 2026 damaged market confidence and triggered SFC scrutiny. Our win theme is **deterministic low-latency compute (Nitro + Graviton4 + EFA) delivering consistent sub-200μs P99 in the AWS Hong Kong Region, combined with intra-region DR that satisfies SFC/HKMA data residency requirements — something Azure structurally cannot offer today** (Azure HK has a single availability zone with no announced expansion timeline). The competitive displacement strategy is surgical: we are NOT proposing a full rip-and-replace of Azure (which would be rejected), but rather targeting the **latency-critical trading path** (matching engine + market data dissemination + FIX gateway) as the beachhead. Once the core trading path moves, market data analytics and DR follow naturally. Azure retains back-office, settlement (CCASS), and corporate workloads in the near term — this "coexist" positioning reduces perceived risk for the CTO while establishing AWS as the platform for mission-critical, latency-sensitive workloads. Key differentiators vs. Azure: (1) HK Region multi-AZ for true intra-city DR, (2) Nitro's consistent network performance vs. Azure's variable "accelerated networking," (3) proven exchange references (NASDAQ, SGX, CME Group), (4) EKS/containers approach avoids proprietary lock-in (addresses Chief Architect's stated concern).

---

## 2. Engagement Plan

> *Pull stance and relationship history from **Contact Profiling Skill**. For executive-level (C-suite/VP), also pull role-level priorities and pain points from **CXO Personas**. Do NOT include people who are not involved in this opportunity.*

### Key Stakeholders

**Dr. James Wong 黄志明** — CTO

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Champion + Technical Decision Maker — reports directly to HKEX CEO, owns all technology strategy including trading platform architecture. Has budget authority up to HK$50M; above that requires Group CEO + Board Technology Committee approval. |
| **Current Stance** | Supportive — initiated contact with AWS after the second latency incident in March 2026. Frustrated with Azure's response time ("three weeks to get a proper RCA from Microsoft"). Actively exploring alternatives for latency-critical path. However, politically careful — Azure relationship is managed at Group level and involves Microsoft's HK CEO personally. Won't make sudden moves. |
| **What They Care About** | *← CXO Persona: CTO (Financial Services / Exchange context)* — System reliability and deterministic latency; regulatory compliance (SFC operational resilience, HKMA technology risk management); market reputation ("an exchange cannot have outages — our credibility IS the product"); vendor diversification (learned from over-reliance on single vendor); talent retention (wants engineers working on modern stack, not legacy). |
| **Profiling** | *← Contact Profiling* — PhD in Computer Science (Cambridge), former Goldman Sachs infrastructure VP (8 years). Thinks in systems — loves architecture diagrams, hates hand-wavy "we'll figure it out" answers. Communication style: precise, measured, asks penetrating questions but gives you time to answer properly. Won't interrupt but will note inconsistencies and bring them up later. Prefers small meetings (3-4 people) over large presentations. Reads materials in advance — always comes prepared. Speaks English primarily in professional settings, Cantonese socially. Values long-term relationships over transactional vendor interactions. `[Updated: 2026-05-08 after first meeting]` |
| **What We Need From Them** | EBC endorsement to proceed to POC + define POC success criteria jointly + internal sponsorship to ring-fence budget separate from Azure EA renewal |
| **How to Win Them** | Peer-level technical credibility is non-negotiable — SA and FSI Specialist must demonstrate deep exchange domain knowledge (FIX, market data, matching engine architecture). Share NASDAQ and SGX references with specific latency metrics. Position AWS as the "exchange-grade cloud" — not a general-purpose platform. Avoid any perception of "selling" — he responds to consultative, problem-solving engagement. Suggest joint architecture review as next step (not a POC pitch). 王总 (GCR FSI Leader) for executive relationship building — James respects seniority and institutional commitment. Estimated 3-4 meetings to close. |

**Karen Chan 陈嘉欣** — Head of Cloud Strategy

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Economic Buyer (operational) + Project Lead — owns cloud vendor strategy, manages Azure relationship day-to-day, controls cloud budget allocation (~HK$180M/year across all vendors). Will lead the commercial negotiation and vendor selection process. |
| **Current Stance** | Neutral-Positive — pragmatic operator. Recognizes Azure limitations but also knows the switching cost. Her team has invested 2 years building Azure-native tooling (Terraform modules, CI/CD pipelines on Azure DevOps). She needs a compelling "why now" and a migration path that doesn't require her team to rebuild everything. Interested in AWS but not yet committed. |
| **What They Care About** | *← CXO Persona: Head of Cloud Strategy (FSI context)* — Total cost of ownership across multi-cloud; operational complexity of managing multiple vendors; team skill gap and training burden; contract flexibility and exit clauses; automation and IaC maturity; compliance automation (audit trails, policy-as-code). |
| **Profiling** | *← Contact Profiling* — HKUST Computer Science, previously at Standard Chartered (cloud platform team, 5 years). Very detail-oriented — will read every line of a proposal and mark up inconsistencies. Communication style: direct, data-driven, doesn't suffer vague commitments. Asks "what's the TCO delta?" within the first 10 minutes of any commercial discussion. Manages a team of 15 cloud engineers — their productivity and morale matter to her. Wary of vendor lock-in from experience (burned by Oracle licensing at Standard Chartered). English-first but uses Cantonese in internal discussions. `[Updated: 2026-05-08]` |
| **What We Need From Them** | Budget ring-fencing for AWS workloads + agreement to joint TCO analysis + team allocation for POC execution |
| **How to Win Them** | Lead with TCO and operational efficiency — she needs numbers, not vision. Prepare a detailed multi-cloud TCO model (AWS HK for latency-critical + Azure for back-office = optimal cost/performance). Address her team's concern about IaC rebuild by showing Terraform/EKS compatibility (most of their Terraform modules are cloud-agnostic). Offer AWS skills training credits. Don't position as "replace Azure" — position as "right workload, right cloud." AE 林浩 should build 1:1 relationship; she responds to partners who make her look good internally. Estimated 2-3 meetings. |

**Robert Yip 叶伟聪** — Chief Architect

| Dimension | Details |
|---|---|
| **Engagement Priority** | Must Meet |
| **Role in This Deal** | Technical Evaluator + Potential Blocker — owns architecture decisions for trading systems. His technical sign-off is required before any infrastructure change to production trading path. Reports to CTO but has strong independent authority on architecture matters. If he says "no," it doesn't happen. |
| **Current Stance** | Skeptical — technically rigorous, has valid concerns about (1) data residency guarantees in AWS HK Region (wants contractual, not just architectural assurance), (2) vendor lock-in risk of moving from one cloud to another ("are we just trading one dependency for another?"), (3) whether AWS can truly match colocation-grade latency in a cloud environment. His skepticism is professional, not political — he can be won with evidence. `[Updated: 2026-05-08]` |
| **What They Care About** | Deterministic latency at P99/P99.9 (not just averages); network jitter and tail latency in shared infrastructure; data sovereignty (contractual guarantees, not marketing); lock-in avoidance (open standards, containers, portable architectures); disaster recovery RTO/RPO that meets SFC requirements; FIX protocol performance under load |
| **Profiling** | *← Contact Profiling* — 20+ year exchange technology veteran (joined HKEX in 2009, was part of the OTP original build). Deep knowledge of matching engine internals. Communication style: quiet in large meetings, devastating in small technical sessions — asks the question you hoped nobody would ask. Thinks in failure modes ("what happens when X goes wrong?"). Prefers written technical proposals he can annotate. Won't commit verbally — needs time to analyze. Has seen multiple vendor migrations in his career and is wary of "this time it's different" promises. Respects engineers who know their stuff; dismisses anyone who hand-waves past complexity. `[待确认 — need more data on personal decision-making style from next technical session]` |
| **What We Need From Them** | Architecture sign-off on proposed trading path migration + POC test plan approval + agreement that AWS HK multi-AZ meets DR requirements |
| **How to Win Them** | This is a "show, don't tell" stakeholder. Written technical deep-dive document (not slides) addressing his three concerns point-by-point: (1) AWS HK Region data residency — provide contractual language and compliance attestation (HKMA TM-E-1 mapping), (2) lock-in avoidance — propose EKS/containers architecture with open standards (FIX engine in containers, portable across clouds), (3) latency evidence — share actual measured P99 data from SGX deployment on similar instance types. Arrange a dedicated 1:1 technical session with Andrew Zhang (FSI Specialist SA) — Robert will open up more in a small, purely technical setting. Do NOT bring commercial people to his sessions. Estimated 3-4 meetings to get sign-off (he's thorough). |

*Engagement sequence rationale: CTO 黄志明 is the Champion who initiated — we have executive cover. Karen Chan controls budget and vendor process — she's the operational gatekeeper. Robert Yip is the architectural veto — if he's not satisfied, the deal stalls regardless of CTO and Karen's support. Strategy: maintain CTO momentum (EBC with 王总), simultaneously run a parallel technical track to win Robert through evidence and depth. Karen comes along once TCO story is solid and Robert's concerns are addressed.*
*Suggest validation, please confirm.*

---

### Engagement Roadmap

| # | Target Window | Objective | Key Stakeholders | Status |
|---|---|---|---|---|
| 1 | Week 1 (May 8) | First meeting: validate latency pain, understand decision process, confirm CTO as champion | CTO 黄志明, Karen Chan | **Done** ✓ |
| 2 | Week 2 (May 15) | Technical deep-dive: current OTP architecture, latency measurements, DR requirements | CTO 黄志明, Robert Yip, Karen Chan | **Done** ✓ |
| 3 | Week 3 (May 28) | EBC: AWS GCR FSI Leader meets HKEX CTO team, strategic alignment, POC endorsement | CTO 黄志明, Karen Chan, Robert Yip | **Next** ↓ |
| 4 | Week 5 (Jun 11) | Joint architecture review: proposed trading path on AWS HK + DR design | Robert Yip, CTO 黄志明 | Planned |
| 5 | Week 7-10 (Jun 25 - Jul 16) | POC: latency benchmark on Graviton4 + market data pipeline + DR failover test | Robert Yip, Karen Chan (team) | Planned |
| 6 | Week 12 (Jul 30) | POC results + commercial proposal + PPA negotiation | Karen Chan, CTO 黄志明 | Planned |

> *Status: **Next ↓** (detailed below) · **Planned** · **Done** ✓ · **Skipped***

---

### Next Milestone Detail

**Milestone #3** — Target Date: May 28, 2026

**Objective:** Executive alignment via EBC — secure CTO's endorsement to proceed to POC, get Karen's commitment to ring-fence budget, begin addressing Robert's technical concerns with evidence

**Customer Attendees & Target Outcome:**
- **CTO 黄志明** — reaffirm champion role; hear AWS GCR FSI Leader's commitment to HKEX as strategic account; endorse POC timeline
- **Karen Chan** — understand TCO positioning (multi-cloud optimization, not rip-and-replace); agree to allocate team resources for POC phase
- **Robert Yip** — receive initial technical evidence (SGX latency data, HK Region architecture); identify specific concerns to address in dedicated follow-up session

**AWS Team:** 王总 (GCR FSI Leader, executive sponsor), AE 林浩 (relationship lead), SA 赵鹏 (architecture), FSI Specialist SA Andrew Zhang (exchange domain)

**Success looks like:**
1. CTO verbally endorses POC scope and timeline (targeting June start)
2. Karen confirms her team can allocate 2-3 engineers for POC execution in June
3. Robert raises specific technical questions (expected: data residency, latency, lock-in) and agrees to a dedicated follow-up architecture session
4. 王总 and CTO establish executive relationship — "you have my direct line"

---

### Estimate & Uncertainty

| | Best Case | Worst Case |
|---|---|---|
| **Calls to Close** | 5 | 9 |
| **Timeline** | 10 weeks (Jul close) | 18 weeks (Sep close, tight before Azure renewal) |

**What could change:**
- Robert Yip's technical objections — if data residency or lock-in concerns aren't resolved to his satisfaction, architecture sign-off could delay POC by 3-4 weeks
- Azure counter-offer — Microsoft will likely respond aggressively once they learn AWS is in play (they have executive relationships at HKEX board level). Could trigger a competitive bake-off scenario adding 4-6 weeks
- SFC regulatory timeline — if the operational resilience compliance deadline is extended, HKEX's urgency to move off single-vendor DR decreases
- POC scope creep — Robert may want to test more scenarios than planned (market stress simulation, failover under load), extending POC duration
- Karen's team capacity — if Azure EA renewal negotiations consume her team's bandwidth in June/July, POC execution could slip

---

## 3. Execution Log

> *Auto-updated after each Call Plan + PMR. Most recent at top.*

**[2026-05-15] Technical Deep-Dive** — Stage unchanged (Technical Validation)
- Robert Yip attended and asked pointed questions about P99.9 tail latency under correlated load (market open scenario). Not satisfied with generic benchmarks — wants HKEX-specific workload testing. Data residency concern formally raised: "I need to see the contractual language, not just architecture diagrams."
- Karen confirmed Azure EA renewal is October 2026 — gives us a hard deadline to present alternative before auto-renewal clause triggers (90-day notice = July 1 deadline for notice of non-renewal).
- CTO supportive throughout but deferred to Robert on technical judgment.
- *→ Updated EP: Robert stance confirmed as Skeptical; Azure renewal deadline added to timeline*

**[2026-05-08] First Meeting** — Stage: Prospect → Technical Validation
- CTO 黄志明 confirmed latency incidents and SFC pressure. "We can't afford another order book delay — the market is watching."
- Karen open but cautious: "Show me the TCO story and I'll listen. But my team can't support another cloud migration without clear ROI."
- Robert not present (traveling). CTO said Robert will be at the technical session — "you'll need to convince him, he's the one who says yes or no on architecture."
- *→ EP created. CTO confirmed as Champion. Karen identified as Economic Buyer (operational). Robert flagged as potential blocker.*

---

*Engagement Plan Template | Version: 1.1*
