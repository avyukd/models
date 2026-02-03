# Position Monitoring

## Purpose
Review existing holdings for thesis tracking based on recent developments. Collect notes on material events organized by analytical dimension.

## Input Format
"Monitor [TICKER]" or "Review [TICKER] updates"

## Process
1. Identify material events since last update (earnings, 8-Ks, news, mgmt changes, M&A, etc.)
2. For each event, categorize and note implications by analytical dimension
3. Assess whether thesis is intact
4. Make recommendation

## Output File
Save findings to: `[TICKER]/monitor-YYYY-MM-DD.md`

### Monitor File Structure
```
# [TICKER] Update - YYYY-MM-DD

## Thesis Status: [On Track / Degraded / Accelerating]

## Events Since Last Update
[Chronological list of material developments with dates]

## Notes by Dimension

### Financial (earnings quality, cash flow, balance sheet)
- [Observations relevant to rigorous-financial-analyst scope]

### Moat (competitive position, pricing power, switching costs)
- [Observations relevant to business-moat-analyst scope]

### Industry/Cycle (cycle position, structural trends)
- [Observations relevant to industry-structure-cycle-analyst scope]
- [Skip if not applicable]

### Capital Allocation (mgmt behavior, M&A, SBC, buybacks)
- [Observations relevant to capital-allocation-analyst scope]
- [Skip if not applicable]

### Geopolitical (regulatory, sanctions, sovereign risk)
- [Observations relevant to geopolitical-risk-analyst scope]
- [Skip if not applicable]

## Thesis Check
- Original thesis: [brief reminder]
- Current evidence: [supporting/contradicting]

## Recommendation: [Hold / Add / Trim / Exit]
Rationale: [1-2 sentences]
```

## Sources to Check
- Latest earnings call/filing
- Recent 8-Ks
- News (WebSearch)
- Price action context
