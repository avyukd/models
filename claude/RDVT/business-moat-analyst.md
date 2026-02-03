# Red Violet (RDVT): Business Quality & Moat Analysis

**Date**: February 2026
**Stock Price**: $39.26 (valuation-agnostic analysis)

---

## Business Model Summary

**How RDVT makes money**: Usage-based fees for identity verification queries plus subscription/contractual revenue for platform access. Two primary products: (1) IDI/idiCORE - identity intelligence platform serving collections, fraud prevention, law enforcement, financial services; (2) FOREWARN - real estate agent safety app sold through REALTOR Association contracts.

**Who pays**: ~9,800 IDI billable customers (primarily SMB and mid-market) across collections, financial services, corporate risk, law enforcement. ~400K FOREWARN users through 575+ REALTOR Associations. 77% of revenue is contractual.

**Cost structure**: Primarily variable data acquisition costs (largest supplier = 45% of data costs, ~19% of revenue). Technology and personnel costs are relatively fixed. Gross margin 70%, adjusted gross margin 82% (excluding non-cash items). EBITDA margin 31%, targeting 40% at $100M revenue.

**Value chain position**: RDVT is a data fusion layer between raw data providers (credit bureaus, public records) and end-users. They license commoditized inputs and transform them into actionable identity intelligence through proprietary algorithms.

---

## The One Thing That Matters for Durability

**Workflow integration depth, not data uniqueness, determines competitive position.**

RDVT does not own proprietary data in any meaningful sense. They license data that competitors can also license. The moat exists because:

1. Their CORE platform transforms commodity data into unique analytical outputs ("data is carrots and onions; IDI is our proprietary carrot and onion soup")
2. Once embedded in customer workflows (collections agents, fraud analysts, law enforcement investigators), switching requires retraining, reintegration, and workflow disruption
3. The derived insights and entity resolution graphs are proprietary even if source data licenses expire

**Why this dominates**: If customers viewed RDVT as a commodity data provider, they would optimize on price. The 93-97% gross revenue retention (excluding expansion) and increasing revenue per customer indicate customers view RDVT as a workflow tool, not a data pipe. The distinction is critical.

**What would weaken it**: If a competitor offered API-compatible replacement with lower cost, or if customer workflows became less dependent on identity verification. Privacy regulation reducing data availability would hurt all players but disproportionately benefit larger competitors with regulatory resources.

---

## What Consensus May Be Missing

### The Bull Case Blind Spot: Data Supplier Concentration Risk

Bulls focus on management pedigree, cloud-native architecture, and retention metrics. They underweight a critical fragility: **45% of data acquisition costs come from a single vendor under a 5-year contract approaching renewal.**

This is not disclosed loudly. If this supplier raises prices materially or terminates, RDVT's gross margin compresses immediately. Management claims alternative tier-2/3 sources exist, but the quality delta is unproven. This single point of failure deserves more scrutiny than it receives.

### The Bear Case Blind Spot: FOREWARN's Strategic Optionality

Bears dismiss FOREWARN as a niche product (~$10M estimated revenue). They miss the structural difference in its customer acquisition model:

- IDI sells to individual companies; FOREWARN sells to REALTOR Associations
- Association contracts create multi-year, multi-member lock-in
- 575+ associations representing hundreds of thousands of agents creates distribution infrastructure
- FOREWARN could become a platform for additional agent safety/verification products

FOREWARN's B2B2C model through associations is structurally stickier than the core IDI business. The optionality value of this distribution network is underappreciated.

### The Second-Order Insight: They're Displacing Legacy, Not Competing on Data

RDVT's 25%+ growth while giants grow single digits suggests something structural. The insight: **RDVT wins not because their data is better, but because their delivery mechanism is better.**

Legacy competitors (LexisNexis, TransUnion Risk, Experian) run on-premise or hybrid architectures. RDVT is cloud-native. For SMB and mid-market customers, this means:
- Faster implementation
- No infrastructure requirements
- Usage-based pricing (vs. enterprise contracts)
- Modern API integrations

RDVT is winning the customers that legacy players serve poorly. The question is whether they can move upmarket (enterprise, government) where legacy relationships are stickier.

---

## Source(s) of Advantage

### 1. Switching Costs (Moderate-High for Existing Customers)

**Mechanism**: Identity verification becomes embedded in daily workflows. Collections agents, fraud analysts, and investigators build processes around specific interfaces and data formats. Switching requires:
- Retraining staff on new interfaces
- Re-integrating APIs into existing systems
- Re-validating data quality for compliance
- Workflow disruption during transition

**Evidence**: 93-97% gross revenue retention (trailing 12 months). Management targets 90-95% as normal range, suggesting this is structural, not cyclical. Revenue from existing customers grew 21% vs. 15% from new customers in 2024 - customers deepen usage, not just maintain it.

**Caveat**: Switching costs exist at the workflow level, not the data level. A customer could theoretically integrate multiple identity providers for redundancy, reducing any single provider's importance over time.

### 2. Data Fusion / Algorithmic Advantage (Moderate)

**Mechanism**: RDVT's CORE platform uses proprietary entity resolution algorithms to link disparate data sources into unified identity graphs. The value is not in raw data (which they license) but in the linking, cleaning, and inference layer.

**Evidence**: Powers 7 of top 10 identity players (including Jumio, Mastercard subsidiaries) - sophisticated buyers who could build internally choose to use RDVT's fusion layer. Management claims they "process customer workflows better than competition" due to cloud architecture efficiency.

**Caveat**: Algorithmic advantages are not durable barriers. Competitors with more resources (LexisNexis acquired Trulioo) can invest in similar capabilities. The advantage is real but time-limited without continuous innovation.

### 3. Management Track Record (Qualitative)

**Mechanism**: Management team (Dubner, Reilly, MacLachlan) built the identity intelligence subsidiaries that became part of LexisNexis and TransUnion. Third iteration of building similar businesses.

**Evidence**: They know the playbook - data licensing, entity resolution, vertical-specific go-to-market. They've done this before and succeeded.

**Caveat**: Past success doesn't guarantee future success. The market is more competitive now, with well-funded fintech competitors and giants who have learned from prior losses.

### 4. Barriers to Entry (High for New Entrants, Irrelevant vs. Incumbents)

**Mechanism**: New competitors would need:
- $50M+ investment over 5+ years before commercial scale
- Data licensing agreements requiring extensive compliance/security vetting
- Time to build entity resolution algorithms
- Go-to-market in fragmented verticals

**Evidence**: No meaningful new entrants in the core identity intelligence space in recent years. Competition is among established players.

**Caveat**: Barriers don't protect against existing giants (Experian, Equifax, TransUnion, LexisNexis). RDVT competes by serving customers that giants serve poorly, not by being insulated from them.

---

## Competitive Landscape

### Structure
The identity verification market is an **oligopoly at the top** (Experian, Equifax, TransUnion, LexisNexis control ~45-50%) with a **fragmented middle tier** where RDVT competes.

RDVT ($75M revenue, ~$600M market cap) is a small player vs. LexisNexis (~$3B+ in risk solutions), Experian (~$7B total), TransUnion (~$4B total).

### Why Giants Haven't Crushed RDVT

1. **Customer segment focus**: Giants prioritize enterprise; RDVT serves SMB/mid-market where sales efficiency matters more than brand.

2. **Architecture**: Legacy on-premise systems are expensive to serve smaller customers. RDVT's cloud-native model has better unit economics for the long tail.

3. **Attention**: Identity verification for collections/fraud is a small piece of giants' business. They don't optimize for it the way RDVT does.

### Competitive Threat Vectors

| Threat Source | Likelihood | Impact | Why |
|--------------|------------|--------|-----|
| Giant downmarket push | Medium | High | If Experian/LexisNexis build cloud-native offerings for SMB, RDVT loses advantage |
| Fintech horizontal expansion | Medium | Medium | Companies like Plaid, Persona could add competitive offerings |
| Customer insourcing | Low | Medium | Largest customers could build internal capabilities |
| Data supplier leverage | Medium | High | Concentrated data suppliers could extract more value |
| Regulatory restriction | Low-Medium | Catastrophic | CFPB/state privacy laws could restrict data broker operations |

---

## Customer Behavior & Revenue Quality

### Retention Metrics
- **Gross revenue retention**: 93-97% (excludes expansion, best-in-class for software)
- **Net revenue retention**: Not disclosed, but implied >100% given 21% growth from existing customers vs. 15% from new customers
- **Contractual revenue**: 77% of total (up from 74% prior year)

### Customer Concentration
- No single customer >10% of revenue (per standard 10-K disclosures)
- Top 105 customers generate >$100K annually (up from 96)
- Broad base: 9,800+ IDI customers, 400K+ FOREWARN users

### Revenue Visibility
- Multi-year REALTOR Association contracts for FOREWARN
- Contractual IDI relationships with monthly minimums
- Usage-based upside on top of contractual base

### Pricing Power Assessment
**Moderate**: RDVT has implemented price escalations but management emphasizes market share over pricing in current growth phase. True pricing power will be tested when growth slows. The 70% gross margin (82% adjusted) suggests meaningful pricing power exists but is not fully exercised.

---

## Evidence of Moat in the Financials

| Metric | 2022 | 2023 | 2024 | Implication |
|--------|------|------|------|-------------|
| Revenue Growth | ~18% | ~20% | 25% | Accelerating despite competition |
| Gross Margin | ~63% | ~66% | 70% | Improving - scale leverage on fixed data costs |
| Adj. EBITDA Margin | ~20% | ~25% | 31% | Operating leverage materializing |
| Gross Revenue Retention | ~93% | ~94% | 94-97% | Consistently high - workflow stickiness |
| Free Cash Flow | Minimal | $5.9M | $14.4M | Business generating real cash |

**Interpretation**: Margin expansion while growing 25% is unusual. This suggests either (a) operating leverage from fixed cost base, (b) pricing power, or (c) mix shift to higher-margin products. Most likely all three. The consistency of retention metrics across years suggests structural stickiness, not temporary satisfaction.

---

## Fragility Analysis: How the Moat Breaks

### Primary Fragility: Data Supplier Concentration

**The risk**: 45% of data acquisition costs come from one vendor. Contract renewal timing is opaque but approaching. If this vendor raises prices 50%, RDVT's gross margin compresses ~450bps immediately.

**Why it matters**: RDVT presents as a technology company but is fundamentally dependent on licensed data. The value creation happens in the fusion layer, but the input layer has concentration risk.

**What to monitor**: Data acquisition cost trends, gross margin trajectory, any disclosure about contract renewals.

### Secondary Fragility: Regulatory Risk

**The risk**: CFPB has expanded scrutiny of data brokers. State privacy laws (California, others) are increasingly restrictive. RDVT operates in a regulatory gray zone.

**Mitigating factor**: Deep integration with law enforcement (FBI, CIA use their data) creates political protection. Completely banning identity data brokers would harm government operations.

**What to monitor**: Federal privacy legislation, CFPB enforcement actions, state-level data broker restrictions.

### Tertiary Fragility: Privacy Removal Services

**The risk**: Services like Incogni help consumers remove their data from data broker databases. If adoption accelerates, database quality degrades.

**Why it's manageable for now**: Adoption is low. Most consumers don't know these services exist. Primarily affects people with reasons to hide (fraud risk correlates with removal requests).

**What to monitor**: Consumer privacy tool adoption rates, any data quality disclosures from RDVT.

### Scenario: Giant Downmarket Push

If Experian or LexisNexis launched a cloud-native, SMB-focused identity verification product with aggressive pricing, RDVT's competitive position erodes rapidly. The giants have better data, stronger brands, and more resources.

**Why it hasn't happened**: Giants are focused on enterprise where margins are higher. SMB is operationally intensive. But this could change.

---

## Moat & Durability Classification

**Moat Strength: Moderate**

*Justification*: RDVT has real switching costs at the workflow level, a competent management team with relevant track record, and a structural advantage serving customers that giants neglect. However, they do not own proprietary data (they license it), face concentrated supplier risk, and could be disrupted if giants prioritize the SMB segment. The moat exists but is not wide.

**Earnings Durability: Medium**

*Justification*: Current earnings are supported by high retention, contractual revenue, and embedded workflows. However, the business depends on (a) continued data licensing at favorable terms, (b) regulatory environment remaining permissive, and (c) giants continuing to neglect the SMB segment. Any of these changing would pressure earnings. The business is not fragile, but it is not fortress-like either.

---

## Summary: The Competitive Reality

RDVT is a well-run company taking share from poorly-served customers of larger competitors. The moat is real but narrow - it depends on workflow integration and delivery mechanism superiority, not proprietary data or insurmountable barriers.

**What's structurally strong**:
- 93-97% gross revenue retention demonstrates workflow stickiness
- Cloud-native architecture creates delivery advantage vs. legacy competitors
- Management has done this before successfully
- FOREWARN creates structurally different (association-based) customer lock-in

**What's structurally fragile**:
- 45% data cost concentration in single supplier
- No proprietary data - all licensed inputs
- Dependent on giants continuing to neglect SMB segment
- Regulatory environment could shift adversely

**The key question for durability**: Can RDVT move upmarket (enterprise, government) before giants move downmarket? The GSA contract and large enterprise wins (state toll authority, major payroll processor) suggest they're trying. Success here would significantly strengthen the moat; failure would leave them vulnerable.

---

## Key Sources

- Red Violet Q3/Q4 2024 and Q2/Q3 2025 earnings releases and calls ([investors.redviolet.com](https://investors.redviolet.com/))
- Company business model analysis ([dcf.fm](https://dcf.fm/products/rdvt-business-model-canvas))
- Welfare Capital deep dive on RDVT competitive dynamics ([welfarecapital.substack.com](https://welfarecapital.substack.com/p/red-violet-revisited-rdvt-deep-dive))
- Identity verification market research ([marketsandmarkets.com](https://www.marketsandmarkets.com/ResearchInsight/identity-verification-market.asp), [grandviewresearch.com](https://www.grandviewresearch.com/industry-analysis/identity-verification-market-report))
- GSA contract announcement August 2024 ([globenewswire.com](https://www.globenewswire.com/news-release/2024/08/13/2929118/0/en/IDI-Now-Available-on-Carahsoft-s-GSA-Schedule.html))
- Management compensation and ownership disclosures ([investors.redviolet.com proxy](https://investors.redviolet.com/static-files/2ebf7a8e-dea5-42be-8bcc-af9965039607))

---

*Analysis prepared under durability-first, valuation-agnostic mandate. No opinion expressed on whether current price is attractive.*
