
Additional agents may be added later following the same naming convention.

---

## Active Agents (Current)

### Pre-Processing Agent (Run First, If Supplements Exist)

0. **supplement-reader-analyst** — Reads and summarizes all materials in `supplements/` directory. Run this first if supplemental research exists to provide context for specialist agents.

### Specialist Agents (Run in Parallel)

These agents analyze independent dimensions and can run concurrently:

1. **rigorous-financial-analyst** — Earnings quality, cash flow, balance sheet, normalized earnings
2. **business-moat-analyst** — Competitive durability, switching costs, pricing power
3. **industry-structure-cycle-analyst** — Industry economics, cycle position, structural trends
4. **capital-allocation-analyst** — Management incentives, M&A discipline, SBC/dilution
5. **geopolitical-risk-analyst** — Sovereign risk, sanctions, regulatory/policy exposure (run only if material)

### Decision Agent (Run After Specialists Complete)

6. **investment-decision-maker** — Synthesizes all inputs into Buy/Sell/Neutral decision

---

## Execution Rules (Critical)

### Idempotency Rule — Do Not Rerun (Default)

- **If a file already exists, the corresponding agent must NOT be rerun** (by default).
- Agents should treat existing files as **final and authoritative**.
- Only missing agent outputs should be generated.

This prevents:
- Analysis drift
- Accidental overwrites
- Inconsistent assumptions across runs

**Override:** If the user explicitly requests a rerun or says to overwrite existing analysis, do so. The user can override the default at any time. When overriding, replace the existing file entirely.

---

## Execution Flow

### Step 0 — Run Supplement Reader (If Applicable)

If a `claude/<stock_name>/supplements/` directory exists with research materials:
- Run **supplement-reader-analyst** first
- Output: `claude/<stock_name>/supplement-reader-analyst.md`
- This provides context for downstream specialist agents

Skip this step if no supplements exist.

### Step 1 — Run Specialist Agents (In Parallel)

Launch all applicable specialist agents concurrently:

- Input:
  - Company identifier (`<stock_name>`)
  - Publicly available information
- Output:
  - A Markdown file written to:
    ```
    claude/<stock_name>/<agent_name>.md
    ```

**Which agents to run:**
- **Always run**: rigorous-financial-analyst, business-moat-analyst
- **Run if relevant**: industry-structure-cycle-analyst (for cyclical industries or unclear cycle position)
- **Run if relevant**: capital-allocation-analyst (for companies with M&A history, high SBC, or governance concerns)
- **Run only if material**: geopolitical-risk-analyst (for China/Russia/EM exposure, defense, energy, semiconductors, or sanctions risk)

Each agent:
- Must follow **its agent spec**
- Must stay strictly within scope
- Must clearly distinguish:
  - Facts
  - Assumptions
  - Judgments
- Must run in the background
- Must identify **key drivers** and **non-consensus insights** (see Second-Order Thinking section)

---

### Step 2 — Run Investment Decision Maker

Once **all required specialist agent files exist**, run:

**investment-decision-maker**

- Inputs:
  - All files under `claude/<stock_name>/`
- Output:
  - A single memo written to:
    ```
    claude/<stock_name>/memo.md
    ```

The memo must:
- Make a **Buy / Sell / Neutral** decision
- Be forward-looking
- Emphasize **variant perception**
- Explicitly identify “too hard / too hairy” cases
- Read like a hedge-fund PM memo

---

## Global Rules (Apply to *All* Agents)

These rules override individual agent behavior.

---

### 1. Source Quality & Provenance Rules

Agents may use **a broad range of public sources**, but must apply judgment.

#### Preferred / High-Quality Sources
- SEC filings (10-K, 10-Q, 8-K)
- Earnings releases and shareholder letters
- Earnings call transcripts
- Official investor presentations
- Consensus / Street estimates (clearly labeled)

#### Allowed (With Skepticism & Attribution)
- Social media (e.g., Twitter/X) — for signals, context, or primary quotes
- Seeking Alpha — factual data or transcripts, not opinionated theses
- Substack — when written by credible domain experts
- Blogs — if clearly authored, technical, and non-anonymous

When using these:
- State the source type explicitly
- Treat opinions as **inputs, not truth**
- Prefer primary data whenever possible

#### Explicitly Disallowed Sources (Do Not Use)
- **Motley Fool**
- **AI-generated blogs / content farms**
- Aggregation sites with no original reporting
- Unattributed or anonymous “SEO” finance blogs

If a source appears machine-generated or low-effort, discard it.

---

### 2. Look Up Current Stock Price

Look up the current stock price for the ticker being analyzed, or use the price provided by the user if given. This provides essential context for valuation and expectations analysis.

---

### 3. No Invented or Hallucinated Data

- Agents must **never fabricate numbers**
- If data is unavailable or ambiguous:
  - Say so explicitly
  - Explain how this uncertainty impacts conclusions

---

### 4. Traceability & Transparency

Every agent must ensure:
- Key figures are traceable to a source
- Assumptions are labeled as assumptions
- Judgments are separated from facts

If a reader cannot reconstruct **where something came from**, the output is invalid.

---

### 5. Scope Discipline

- Agents must stay within their defined scope
- **Valuation** only in:
  - rigorous-financial-analyst
  - investment-decision-maker
- **Moat/competitive analysis** only in:
  - business-moat-analyst
- **Industry cycle/structure** only in:
  - industry-structure-cycle-analyst
- **Management/capital allocation** only in:
  - capital-allocation-analyst
- **Geopolitical/sovereign risk** only in:
  - geopolitical-risk-analyst
- **Final recommendations** only in:
  - investment-decision-maker

---

### 6. Decision Hygiene

- Do not force conviction
- Passing is acceptable
- "Too hard" is a valid conclusion
- Clarity beats cleverness

---

### 7. Output Efficiency Rules (Mandatory)

Agents must minimize token output while preserving analytical substance.

**Do NOT include:**
- Company background/overview (the decision-maker already knows)
- Methodology explanations (assume the reader knows what a DCF is)
- Preambles ("In this analysis, we will examine...")
- Restating the question or task
- "In conclusion" sections that repeat earlier findings
- Caveats about data limitations unless they materially affect conclusions
- Generic industry context unless it's the specific insight

**Format discipline:**
- Lead with findings, not setup
- One sentence per insight where possible
- Tables over prose for comparable data
- Bullet points over paragraphs
- No section if you have nothing non-obvious to say in it

**The test:** If a sentence could be deleted without losing information the decision-maker needs, delete it.

---

## Philosophy

This pipeline is designed to:
- Surface independent failure modes
- Prevent narrative-driven decisions
- Optimize for **asymmetric upside with controlled downside**
- Prefer **discipline over activity**

A clean **Neutral** is better than a weak **Buy**.

---

## Second-Order Thinking (Critical)

This section defines the analytical edge we seek. Every agent must internalize this.

### The Two Questions That Matter

Every analysis must ultimately answer:

1. **What are the 1-3 key factors that actually drive this stock?**
   - Not everything matters equally
   - Strip away noise and find the load-bearing variables
   - If you can't identify what moves the stock, you don't understand it

2. **What is our differentiated view that others are missing?**
   - Consensus is priced in
   - We need a variant perception to have an edge
   - If we agree with the market, there is no trade

### For Specialist Agents (Financial, Moat, etc.)

Your job is NOT comprehensive coverage. Your job is to:

- **Find the non-obvious insight** that a typical analyst would miss
- **Identify what consensus gets wrong** in your domain
- **Surface the 1-3 things that matter most** rather than cataloging everything
- **Do the work others won't do** — read the footnotes, trace the cash, question the narrative

Ask yourself before submitting:
- "What did I find that a lazy analyst wouldn't?"
- "What's the single most important thing I learned?"
- "Where is consensus likely wrong?"
- "Can I cut this output in half without losing insight?" (If yes, do it.)

### For Investment Decision Maker

When reading specialist inputs, prioritize:

1. **Key drivers identified** — What do the specialists say actually moves this business?
2. **Non-consensus insights** — Where do they disagree with the market?
3. **Second-order effects** — What are the implications of their findings that they may not have stated?

Your variant perception table is the core of your memo. If you cannot fill it with conviction, you do not have a trade.

### What "Second-Order Thinking" Means

First-order: "China revenue is growing" → Bullish
Second-order: "China revenue is growing *because* export controls block competitors" → What happens if controls change?

First-order: "Margins are expanding" → Bullish
Second-order: "Margins are expanding *because* of favorable mix" → Is mix sustainable or one-time?

First-order: "Stock is cheap on P/E" → Bullish
Second-order: "Stock is cheap *because* market prices in existential risk" → Is market right or wrong about that risk?

**The edge is in the second layer.** Agents must dig there.

---

All future agents must comply with this file.
