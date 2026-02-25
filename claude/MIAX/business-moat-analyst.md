# MIAX (Miami International Holdings) -- Business Quality & Moat Analysis

**Stock Price:** ~$40-44 (Feb 2026). IPO'd Aug 2025 at $23/share. Market cap ~$3.5B.

---

## 1. Business Model Summary

MIAX operates four U.S. options exchanges (MIAX Options, MIAX Pearl, MIAX Emerald, MIAX Sapphire), one U.S. equities exchange (MIAX Pearl Equities), a futures exchange (MIAX Futures), Dorman Trading (futures commission merchant), and two international exchanges (Bermuda Stock Exchange, TISE).

**Who pays:** Broker-dealers and market makers pay transaction fees, access/connectivity fees, and market data fees. Market makers also receive rebates for providing liquidity -- so gross revenue far exceeds net revenue.

**Revenue composition (approximate):**
- Options: ~86% of net revenue (Q3 2025: $94.5M of $109.5M net revenue)
- Equities, Futures, International: remainder
- Revenue types: transaction fees (net of rebates), market data fees, access/connectivity fees
- Transaction fee CAGRs: ~19% (options), access fees ~22%, market data ~12% (2020-2024 per S-1)

**Cost structure:** High fixed cost, low marginal cost. Technology infrastructure, personnel, regulatory compliance, and data center operations are largely fixed. Incremental volume drops to the bottom line at high margins. This creates operating leverage in both directions.

**Gross vs. net:** Annual gross revenue was ~$1.14B in 2024, but this includes pass-through transaction fees and rebates. Net revenue (after rebates/liquidity payments) was ~$248M for options in 2024 (up from ~$122M in 2020). The gross number is misleading -- net revenue is the economically relevant figure.

**Fact:** Adjusted EBITDA margin expanded from 27% (Q3 2024) to 44% (Q3 2025) on 57% net revenue growth. GAAP results distorted by one-time items (debt extinguishment, IPO costs). TTM FCF of ~$135M on ~$1.32B gross revenue.

---

## 2. Source(s) of Advantage

### Technology (Real but Depreciating)

**Mechanism:** MIAX built its matching engine and exchange technology entirely in-house. This differentiates it from exchanges that license third-party technology (e.g., some Nasdaq-powered venues). MIAX claims 25 microsecond latency at the 99th percentile, wire-order determinism, and 99.9998% uptime since 2012 launch.

**Why it matters:** Market makers route flow preferentially to exchanges with the lowest latency, highest determinism, and best reliability. Speed advantages at the microsecond level affect market maker profitability and therefore their willingness to quote tightly and provide liquidity. This creates a virtuous cycle: better tech attracts market makers, more market makers attract order flow, more order flow attracts more market makers.

**Why it is depreciating:** Technology advantages in exchange infrastructure are replicable given sufficient investment. Cboe rebuilt its technology platform (migrating from legacy BATS systems). Nasdaq continuously invests in matching engine speed. MEMX was purpose-built for low latency. MIAX's technology lead, while real today, narrows as competitors invest. It is a treadmill -- you must keep spending to avoid falling behind, but spending does not guarantee pulling further ahead.

**Judgment:** Technology is a necessary condition for maintaining share, not a sufficient condition for a durable moat. It is a competitive advantage, not a competitive moat.

### Equity Rights Program / Market Maker Alignment (Structural but Expired)

**Mechanism:** Between 2013 and 2024, MIAX ran five Equity Rights Programs (ERPs) that gave major market makers (Citadel, Susquehanna, IMC, Optiver, Wolverine, Morgan Stanley, Interactive Brokers, Two Sigma, Virtu) the right to acquire equity in MIH in exchange for upfront cash, prepaid fees, and meeting volume commitments. This financially aligned the largest options market makers with MIAX's success.

**Why it mattered:** It bootstrapped liquidity. Market makers with an ownership stake had direct financial incentive to route flow to MIAX venues, creating the liquidity foundation that attracted additional order flow. This is how a new exchange overcomes the cold-start problem.

**Current status:** All ERP earning periods have expired as of June 30, 2024 (per S-1). The market makers who participated now hold equity (many of which converted to shares at IPO), but the ongoing volume commitments are gone. The question is whether routing habits persist after the financial incentives expire.

**Judgment:** The ERPs were a brilliant bootstrapping mechanism, not a durable moat. They created behavioral inertia -- market makers built connectivity, integrated MIAX into smart order routers, and developed comfort with the platform. That inertia is real but not structural. If a competitor offers better economics or technology, routers will shift.

### Scale Within a Fragmented Market (Moderate)

**Mechanism:** MIAX is the fourth-largest options exchange family with ~15-17% multi-listed market share across four venues. Scale matters because exchanges have high fixed costs and low marginal costs -- each incremental contract carries near-100% contribution margin. Larger share means better unit economics.

**Limitation:** 15-17% share in a market with 18 venues is meaningful but not dominant. Cboe has ~30-33%, Nasdaq ~22-26%, NYSE ~14%. MIAX is not subscale, but it lacks the kind of dominant share position that creates self-reinforcing advantages. It is large enough to operate profitably but not large enough to dictate industry dynamics.

### What MIAX Does NOT Have: Proprietary Products

**This is the single most important structural fact.** MIAX has zero proprietary products with exclusive trading rights. Every contract that trades on MIAX can also trade on 17 other venues. Cboe's SPX and VIX options trade exclusively on Cboe -- they are captive, high-margin, impossible-to-replicate revenue streams. MIAX's SPIKES product (a SPY-based volatility index) has gained negligible traction against the entrenched VIX ecosystem.

MIAX sold 90% of MIAXdx (its derivatives/prediction market exchange) to a Robinhood/Susquehanna JV in Jan 2026. This was arguably the one asset with proprietary product potential, and MIAX chose to monetize it rather than build it.

**Judgment:** Without proprietary products, MIAX is structurally a commodity exchange competing on speed and fees. This caps its margin potential well below Cboe's 65%+ EBITDA margins regardless of how much share it gains.

---

## 3. Competitive Landscape

**Structure:** Four exchange families control ~85% of multi-listed options volume. 18 total venues, with IEX targeting a 19th by late 2026.

| Exchange Family | Multi-Listed Share (2024-2025) | Venues | Key Edge |
|----------------|-------------------------------|--------|----------|
| Cboe | ~30-33% | 4 | SPX/VIX exclusivity |
| Nasdaq | ~22-26% | 6 | Scale, PHLX floor |
| NYSE | ~14% | 2 | Listed company relationships |
| MIAX | ~15-17% | 4 | Technology, speed |
| Others (MEMX, BOX) | ~10-15% | Various | Niche |

**Differentiation is real but thin.** Exchanges differentiate on fee structures (maker-taker vs taker-maker, pro-rata vs price-time priority), latency, and rebate tiers. These are all adjustable parameters. No exchange has a durable structural differentiation in multi-listed options beyond Cboe's proprietary products.

**Fee schedule arms race:** Exchanges continuously adjust rebate tiers and fee structures. Net revenue capture per contract (after rebates) is measured in fractions of a cent. This is a classic Red Queen dynamic -- exchanges compete away economics to maintain or gain share. Volume-based rebate tiers create a situation where market makers concentrate flow to hit higher tiers, which benefits larger exchanges but also compresses net revenue per contract.

**Venue proliferation never reverses.** New exchanges almost never shut down because marginal operating costs are low relative to sunk technology investments. The competitive landscape can only fragment further, never consolidate (absent M&A). IEX's planned options exchange adds incremental pressure.

**Entry barriers:** Moderate. Launching an exchange requires SEC approval, $20-50M+ in technology investment, and the ability to bootstrap liquidity. The ERP approach MIAX pioneered is now replicable. MEMX launched in 2020 and achieved viable share. The barriers are real but not prohibitive for well-capitalized entrants.

---

## 4. Customer Behavior & Revenue Quality

**Customer concentration:** MIAX's customer base is highly concentrated among a small number of large market makers and broker-dealers. The CEO has explicitly stated focus on "the Citadels, the Susquehannas, the IMCs, the Optivers of the world." These firms represent disproportionate share of volume. This is not disclosed precisely, but given that a handful of market makers provide the majority of options liquidity industry-wide, MIAX's volume is likely concentrated among fewer than 10-15 firms.

**Switching costs: Near zero at the routing level.** Broker-dealer smart order routers can redirect flow across venues in milliseconds. There is no contractual lock-in. The switching cost is operational (maintaining connectivity to each venue, building out co-location infrastructure) but this is a sunk cost -- every major market maker already has connectivity to all 18 venues. The incremental cost of routing more or less flow to MIAX is approximately zero.

**Behavioral stickiness vs. structural lock-in:** MIAX benefits from behavioral stickiness (routing habits, familiarity, integrated workflows) rather than structural switching costs. Market makers who have invested in MIAX connectivity and optimized their strategies for MIAX's matching engine have some inertia, but this is the weakest form of retention. It can be overcome by better economics or technology at competing venues.

**Revenue visibility:** Low relative to subscription-based businesses. Transaction revenue is inherently variable -- it depends on industry volume (driven by market volatility) and MIAX's share of that volume. There are no long-term contracts guaranteeing transaction volume. Market data and connectivity fees are more recurring and predictable but represent a minority of revenue.

**Pricing power:** Effectively zero in multi-listed options. MIAX is a price-taker. If MIAX raised transaction fees materially, smart order routers would redirect flow to cheaper venues within days. Pricing power exists only in market data and connectivity, where exchanges have some regulatory-supported pricing discretion, but these are under scrutiny.

---

## 5. Evidence of Moat in the Financials

**Margin trajectory:**
- Adjusted EBITDA margin: 27% (Q3 2024) to 44% (Q3 2025)
- This 17pp expansion was driven almost entirely by volume-driven operating leverage, not pricing power or structural margin improvement
- Cboe comparison: 65-67% adjusted EBITDA margin consistently. The ~20pp+ gap between MIAX and Cboe is structural (proprietary products), not temporary

**Market share gains:**
- MIAX family share: ~13.5% (2022) to ~15.1% (2024) to ~17.2% (Q3 2025 record)
- Share gains are real but partly reflect Sapphire launch (Aug 2024) which cannibalized some intra-family volume (Pearl's share dropped 34.7% YoY in 2024)
- Consolidated family share has grown, but at the cost of running four venues with overlapping fixed costs

**Revenue growth:**
- Options segment net revenue: $122M (2020) to $248M (2024), ~19% CAGR
- Driven by industry volume growth (~15% CAGR) plus modest share gains plus stable-to-rising revenue per contract
- The question: how much of this is MIAX-specific vs. riding the industry wave?

**Free cash flow:** TTM FCF of ~$135M is real but inflated by above-mid-cycle volumes. The company recently retired most debt (only $6.5M as of Q3 2025) and holds $401.5M cash post-IPO.

**Judgment:** The financials show a business benefiting enormously from operating leverage in a volume-surging industry. This is consistent with a decent business in a great environment, not necessarily a great business. The margin gap vs. Cboe is the financial fingerprint of the missing proprietary product moat.

---

## 6. Fragility Analysis

### Primary Fragility: Volume Dependence Without Pricing Power

MIAX's entire business model depends on industry options volume growing and MIAX maintaining/gaining share at current per-contract economics. All three legs of this stool can weaken simultaneously:

- **Volume:** If VIX normalizes to sub-15 for an extended period and 0DTE growth plateaus, industry volume growth could decelerate to single digits. MIAX's operating leverage works in reverse -- margin compression would be severe.
- **Share:** IEX options launch, continued MEMX growth, and constant fee competition from Cboe/Nasdaq/NYSE all pressure share. MIAX's ERP-driven volume commitments have expired. Market maker routing decisions are now purely economic.
- **Revenue per contract:** Fee competition compresses net capture. Each new venue adds competitive pressure. Revenue per contract has been stable-to-rising recently, but this is unusual and may not persist.

### Secondary Fragility: Customer Concentration Among Market Makers

A small number of market-making firms control a disproportionate share of MIAX's volume. If Citadel or Susquehanna shifted routing away from MIAX (due to fee changes at competitors, technology improvements elsewhere, or strategic reasons), the volume impact would be immediate and significant. These firms have zero switching costs.

### Tertiary Fragility: No Proprietary Products

Without exclusive products, MIAX cannot create captive revenue streams. Every attempt to build proprietary products (SPIKES) has failed to achieve meaningful traction. The VIX franchise is essentially unassailable due to deep liquidity, decades of index history, and integration into the financial ecosystem. MIAX sold MIAXdx rather than developing it. There is no visible path to proprietary product revenue.

### Regulatory Risk

Options Regulatory Fee (ORF) reform, maker-taker restrictions, or market data fee caps could redistribute revenue in unpredictable ways. As a smaller exchange family, MIAX has less influence over regulatory outcomes than Cboe or Nasdaq.

---

## 7. Moat & Durability Classification

**Moat Strength: Weak**

MIAX has competitive advantages (technology, market maker relationships, scale) but not a moat in the structural sense. It competes in a commoditized segment of the options exchange market with near-zero switching costs, no proprietary products, and fee-based competition that prevents sustained excess returns. Its advantages are replicable and depreciating. The 20pp+ EBITDA margin gap vs. Cboe is the clearest evidence of structural inferiority.

**Earnings Durability: Medium**

MIAX will not disappear. It has achieved sufficient scale (~15-17% share) to operate profitably through normal market conditions. The secular growth in options volumes provides a rising floor. But earnings are highly sensitive to volume cycles, and the lack of proprietary products means MIAX has no structural defense against fee compression or share erosion. Mid-cycle earnings power is materially below current run-rate. Margins will compress in a low-volume environment.

---

## The One Thing That Matters for Durability

**Whether MIAX can maintain its ~15-17% multi-listed share without the financial incentives of the Equity Rights Programs.**

The ERPs were the mechanism that built MIAX's market share. They aligned the largest market makers financially with MIAX's success. All ERP earning periods expired by June 2024. The key question is whether the behavioral inertia and technology integration that the ERPs created will persist, or whether share will gradually erode as competitors invest in technology and adjust fee incentives.

If MIAX's share holds at 15%+ through 2026-2027 without ERP incentives, it will have proven that its technology and execution quality generate genuine structural demand. If share drifts below 14% once the ERP-era market makers no longer have equity incentives, the entire growth narrative is challenged.

This factor dominates because everything else -- volume growth, margin expansion, revenue per contract -- is downstream of share retention. And share retention without financial alignment mechanisms is unproven.

---

## What Consensus May Be Missing

**Consensus view:** MIAX is a technology-differentiated options exchange riding secular volume growth, gaining share, and operating with improving margins. Recent IPO with a clean balance sheet and significant operating leverage to continued volume growth.

**The non-obvious insight (bearish):** MIAX's market share was purchased, not earned through structural advantage.

The Equity Rights Programs from 2013-2024 were a form of volume acquisition cost. MIAX gave major market makers equity stakes in exchange for volume commitments. This is functionally equivalent to a SaaS company paying customer acquisition costs -- except MIAX paid in equity dilution rather than cash. The market share MIAX enjoys today was built on these financial incentives, not purely on technology superiority.

Now that the ERPs have expired and MIAX is public (meaning the equity-for-volume mechanism is no longer available in the same form), MIAX must compete for routing decisions purely on technology and economics. It has never had to do this at scale. The 2025 volume environment -- surging 26% industry-wide -- has masked this transition because everyone is winning in a rising market. The true test comes in a flat or declining volume environment when market makers optimize routing aggressively.

Additionally: the market may be over-indexing on MIAX's margin expansion (27% to 44% EBITDA) without recognizing this is almost entirely operating leverage from a volume surge, not structural margin improvement. In a mid-cycle environment, margins likely revert to 30-35%. The current run-rate overstates sustainable earnings power.

This insight is bearish for durability. It does not mean MIAX is a bad business -- it means the competitive position is less proven and more fragile than the headline numbers suggest.

---

## Key Sources

- MIAX S-1/Prospectus (SEC, Aug 2025) -- revenue composition, ERP details, risk factors
- MIAX Q3 2025 Earnings Release (Nov 5, 2025) -- $109.5M net revenue, 44% adj. EBITDA margin, 17.2% market share
- MIAX Monthly Trading Reports (miaxglobal.com) -- market share, volume data
- MIAX Press Releases -- ERP programs (2013, 2015, 2017, 2018), Sapphire launch, MIAXdx sale
- OCC Historical Volume Statistics -- industry volume data
- Cboe Quarterly Earnings and Market Data -- competitive benchmarks, SPX/VIX volumes
- Stock Analysis (stockanalysis.com) -- revenue history, financial aggregation
- SEC Fee Schedule Filings -- MIAX Emerald, Pearl fee structures
