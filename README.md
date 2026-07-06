# Pharmaceutical Services Financial Analysis — Charles River Laboratories (NYSE: CRL)

## About this project

This is an independent financial analysis project built around Charles River Laboratories' three public business segments — Research Models & Services (RMS), Discovery & Safety Assessment (DSA), and Manufacturing Solutions — using only their publicly disclosed SEC filings and earnings releases. The goal was to take $4.0bn in real segment revenue data and build the kind of analysis a finance analyst would actually be asked to produce: variance against prior year, margin trend analysis, revenue mix shifts, and a fully sourced audit trail behind every number.

Every hardcoded figure in the workbook traces to a specific SEC filing (8-K earnings releases, the FY2025 10-K), cited by URL on the Sources tab. Nothing is estimated, modelled, or invented, and every gap in disclosure is flagged explicitly rather than filled in to make the analysis look tidier than the underlying data actually is.

## Tools used

- **Microsoft Excel** — the entire model: six linked tabs, colour coded formula conventions (blue for sourced hardcoded facts, green for live cross-tab formulas, black for on-tab calculations, grey italic for flagged data gaps), native charts, and 650+ formula-driven data points verified against source filings with zero calculation errors.
- **SEC EDGAR** — primary source for all 8-K earnings releases and the FY2025 10-K.
- **Manual verification method** — every segment figure cross-checked to reconcile against disclosed company totals, and the organic growth bridge independently recalculated and matched against CRL's own reported organic growth percentages, rather than trusted on first entry.

---

## Raw Data

The single source of truth for every figure used elsewhere in the workbook. Six tables covering full-year segment revenue and margins, Q3 quarter/9-month detail, Q4 quarterly detail, the organic growth bridge, the total-company product/service revenue split, and FY2026 guidance. Every blue cell is a hardcoded, sourced fact — nothing here is calculated or estimated, only entered directly from filings.

![Raw Data 1](./screenshots/raw_data_1.png)
![Raw Data 2](./screenshots/raw_data_2.png)

## Variance Analysis

Answers "what changed and why" for FY2025 vs FY2024: segment revenue variance in $ and %, operating income and margin variance, each with driver commentary explaining the underlying cause. Also includes the Q3 2025 organic growth bridge, isolating true underlying growth from currency and portfolio effects, showing that a headline -0.5% company decline was actually a -1.6% organic decline.

**DSA** is the clearest case here: revenue fell 2.0% and the organic growth bridge confirms this wasn't a currency effect, with organic growth at -3.1%, driven by softer discovery services volume and safety assessment demand. This is the one segment where the numbers point to genuine underlying softness rather than an accounting artefact.

![Variance Analysis](./screenshots/variance_analysis.png)

## Margin Trend

Tracks whether each segment is genuinely getting more or less profitable, using GAAP and Non-GAAP margins side by side.

**RMS**: headline GAAP operating margin dropped from 13.8% to 5.3%, an 8.5 point fall that looks like real deterioration. But Non-GAAP margin actually improved, from 23.7% to 24.8%. The gap is a non-cash impairment distorting the GAAP number in a single period, not a genuine decline in the business.

**Manufacturing**: the sharpest contrast in the whole project. GAAP operating margin collapsed to -24.0% (from -9.3%), which alone looks alarming. Non-GAAP margin actually rose to 28.8%, the strongest of all three segments, again driven by a one-off non-cash impairment distorting GAAP. This is the clearest single example in the project of why GAAP margins alone can lead to the wrong conclusion about a business's health.

![Margin Trend](./screenshots/margin_trend.png)

## Product-Service Mix

Looks at the total-company split between product and service revenue, since CRL only discloses this split at the company level, not by segment, a limitation the tab notes explicitly rather than papering over. Shows a modest 0.6 point mix shift toward product revenue in FY2025, which lines up directly with Manufacturing's Non-GAAP margin improvement, since Manufacturing skews more product-heavy than DSA.

![Revenue Mix](./screenshots/revenue_mix.png)

## Sources

Every figure in the workbook traces back to one of six primary documents listed here — SEC 8-K earnings releases (Q1–Q4 2025), the FY2025 10-K, and the FY2024/Q4 earnings release, each with publisher, filing date, and direct URL. Also documents the verification method: segment figures independently cross-checked to reconcile with disclosed totals, and organic growth recalculated and matched against CRL's own reported percentages.

![Sources](./screenshots/sources.png)

---

## Why this matters

Together these tabs make one consistent point: **headline GAAP numbers alone would tell a misleading story about Charles River Laboratories in FY2025**, and it takes segment-level margin analysis, an organic growth bridge, and a mix-shift view to see what's actually driving performance. That's the exact type of judgement, knowing which number to trust and why, that a finance analyst is expected to bring to a business like Almac Group.

## Disclaimer

This is an independent, non-commissioned analysis for portfolio purposes only. Charles River Laboratories has no affiliation with this project. All figures are drawn from public disclosures; none are estimated or modelled.
