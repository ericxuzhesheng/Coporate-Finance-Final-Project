# Valuing a Frontier-Model AI Lab — and Testing How Its Price Discovers "Capability"
## Zhipu AI (Knowledge Atlas, 2513.HK) — Corporate Finance Final Project, Detailed Outline

**Subject company:** Zhipu AI / Knowledge Atlas Technology Joint Stock Co., Ltd. — HKEX Main Board, **2513.HK**, listed **2026-01-08** via **Chapter 18C** (specialist technology).
**Comparable / benchmark:** MiniMax (稀宇科技), HKEX **00100.HK**, listed **2026-01-09**.
**Language:** English. **Typesetting:** LaTeX (+BibTeX). **Model:** Excel. **Abstract:** ≤ 300 words.

### The original idea (the paper's spine)
A pre-revenue foundation-model lab has **no earnings to be surprised by**, yet its price moved ~**19x** to **~US$124B** (**P/S ≈ 600x**). So the paper does two things:
1. **(Main line) Valuation** — establish a *fundamental anchor* with scenario DCF + comparables + a real-options lens that explains why a pre-revenue lab can rationally carry option-like value.
2. **(Original highlight) "Capability-Surprise" event study** — port the classic earnings-surprise / PEAD machinery onto a new event type: **model releases and benchmark-leaderboard rankings** (GLM-5.x, Z.code). Test whether *capability information* is efficiently priced, or whether there is **Post-Capability-Announcement Drift (PCAD)** — the AI analogue of PEAD.

> Thesis: price discovery for frontier AI labs has shifted from *earnings surprise* to *capability surprise*; the market is semi-efficient with respect to capability signals, which both anchors and bounds the bubble debate.
> (Methodological lineage: extends the author's prior work — *Earnings-Surprise-Market-Efficiency*, China A-shares — to a new asset class, reusing CAR windows, SUE-style normalization, and an honest diagnostic posture.)

---

## 0. Abstract (≤300 words) + Keywords
Subject; dual method (valuation anchor + capability-surprise event study); headline finding; practical takeaway.
Keywords: foundation models, Chapter 18C, pre-revenue valuation, real options, market efficiency, event study, PEAD/PCAD.

## 1. Introduction
- 1.1 The 2026 "AI Tigers" HK listing wave (Zhipu 1/8, MiniMax 1/9).
- 1.2 Research questions: (i) fundamental value range? (ii) does the ~19x run reflect efficient pricing of *capability*, exuberance, or option value? (iii) is open-source + cost-disruption financially sustainable?
- 1.3 Contribution: the *capability-surprise* reframing of market efficiency. Roadmap.

## 2. Company & Business Model
History (Tsinghua KEG → Knowledge Atlas, 2019); GLM family; revenue model (API usage + subscription + on-prem + fine-tuning); **open-weight funnel**; Z.ai / Z.code platform; ownership & governance.

## 3. Financial Performance (2023–H1 2025; pre-revenue adaptation)
Revenue trajectory (Table D1/D4); losses, R&D intensity, cash burn, runway; post-IPO balance sheet (proceeds ~70% to model R&D 2026–28); pivot from ratios to **unit economics / usage metrics**.

## 4. Market Reaction & Capital-Market Strategy  ← *["Why HK-Zhipu is so impressive" thread]*
IPO mechanics (HK$116.20, cornerstones, 18C eligibility); post-listing price action vs MiniMax & HK tech (Tables D2/D3); **why the listing matters** (first foundation-model IPO globally; 18C regulatory access for a pre-revenue lab; signaling/certification; permanent capital). Sets up the efficiency question pursued empirically in §9.

## 5. Industry & Competitive Landscape  ← *[GLM-5.x / Z.code leaderboard thread]*
Porter's Five Forces for foundation models; China "AI Tigers" + global frontier labs as the valuation anchor set; **leaderboard strategy decoded** (MoE: GLM-4.6 ≈355B/32B active, 200K ctx; GLM-5.1 #1 SWE-Bench Pro 58.4%; open-weight + low token price = cost-disruption flywheel). This section **defines the event taxonomy** consumed by §9.

## 6. Macroeconomic & Policy Environment
China AI policy / state procurement; US compute-export controls (efficiency-by-necessity); HK capital market (18C, Stock Connect eligibility, liquidity); rates / risk appetite / HKD peg and long-duration growth valuation.

## 7. Corporate Strategy & SWOT
Open-source flywheel vs closed frontier; enterprise + sovereign + overseas expansion; SWOT; scenario drivers feeding §8.

## 8. Valuation — MAIN LINE  ← *[recommended mix]*
- 8.1 Cost of capital: CAPM Ke with **bottom-up/comparable beta** (HK index unavailable in feed → global AI-software comps, unlever→relever); WACC.
- 8.2 **Scenario DCF (FCFF, explicit 2026–2035 + terminal)**: Bear/Base/Bull on revenue CAGR, steady-state margin, reinvestment; probability-weighted EV → per-share equity value.
- 8.3 **Comparables**: EV/Sales vs MiniMax and global labs (private-round implied multiples); reconcile to market price.
- 8.4 **Real-options lens**: lab as a portfolio of options on AGI-scale outcomes; decision-tree / Black–Scholes sizing to *explain* (not justify) the premium and the ~600x P/S.
- 8.5 Football-field chart; 8.6 Sensitivity & tornado (WACC, terminal margin, CAGR).

## 9. Original Highlight — The "Capability-Surprise" Event Study (Zhipu vs MiniMax)
- 9.1 Motivation: no earnings ⇒ test efficiency w.r.t. *capability* signals; PEAD → **PCAD** hypothesis.
- 9.2 **Event taxonomy** (from §5): model launches (GLM-5/5.1, MiniMax releases), benchmark rank changes (SWE-Bench Pro, LMArena/coding leaderboards), major open-weight drops, big customer/sovereign deals.
- 9.3 **"Surprise" metric**: define a capability-surprise proxy (e.g., benchmark-delta vs prior SOTA / vs consensus expectation; ranked tiers), analogous to SUE/standardized surprise.
- 9.4 **Method**: CAR across three windows — leakage (pre-event), reaction [0,+1]/[1,10], drift [11,N]; market model with comparable/peer benchmark (since HK index feed unavailable, use peer-adjusted or equal-weight AI-basket return); Zhipu vs MiniMax cross-section.
- 9.5 **Results & interpretation**: immediate reaction vs drift → semi-strong efficiency verdict; link drift sign/size back to the §8 fundamental anchor (does the market over/under-react to capability?).
- 9.6 **Honesty box** (repo-style): small sample (only ~5 months since listing, limited events) ⇒ *diagnostic evidence, not definitive*; robustness across surprise definitions and windows.

## 10. Conclusion & Practical Implications
Fundamental range vs market price → over/under/optionality verdict; capability-surprise efficiency finding; implications for investors, 18C founders, policymakers; limitations & future work (expand event panel, NLP-scored capability surprise, multi-lab panel).

## Appendices
A. Data tables (`DATA_TABLES.md`). B. Excel assumptions log. C. Event log & CAR tables. D. Bibliography (BibTeX).

---

### Assignment requirement → section map
| Requirement | Section(s) |
|---|---|
| Historical financials & operations | §2, §3 |
| Market reaction | §4, **§9** |
| Future strategy | §5, §7 |
| Industry & business environment | §5 |
| Macroeconomic impact | §6 |
| Corporate finance theory (valuation, cost of capital, real options, market efficiency, event study) | §4, **§8 (main)**, **§9 (original)** |

### Repo / build structure
```
Coporate-Finance-Final-Project/
├── OUTLINE.md                 ← this file
├── DATA_TABLES.md             ← compiled data + sources (+ event log D6)
├── data/                      ← Tushare CSVs (prices), event-study inputs
├── paper/                     ← LaTeX (main.tex, sections/, refs.bib)     [next]
├── model/                     ← valuation_model.xlsx                       [next]
├── eventstudy/                ← CAR computation scripts + outputs          [next]
└── figures/                   ← football field, CAR plots, price charts    [next]
```
