# Data Tables — Zhipu AI (2513.HK) vs MiniMax (00100.HK)

All market data pulled via **Tushare `hk_daily`** on 2026-06-26 (CSV in `data/`). Fundamental data from
public filings/press (sources at bottom). Figures marked **[confirm]** need cross-check against the HKEX 18C
prospectus before final write-up.

---

## Table D1 — Company & IPO Snapshot

| Item | Zhipu AI (Knowledge Atlas) | MiniMax |
|---|---|---|
| HKEX ticker | 2513.HK | 00100.HK |
| Listing date | 2026-01-08 | 2026-01-09 |
| Listing regime | Chapter 18C (specialist tech) | Chapter 18C / standard [confirm] |
| IPO price | HK$116.20 | HK$165.00 |
| Shares newly issued | 37.42M | ~ [confirm] |
| Gross proceeds | ~HK$5.0B [confirm exact] | ~HK$4.8B (US$620M) |
| IPO valuation | HK$51.8B (~US$6.7B) | ~US$6.5B |
| Cornerstones | HK$3B cornerstone commitments | Abu Dhabi Investment Authority, Alibaba, etc. |
| HQ / founded | Beijing, 2019 (Tsinghua KEG lineage) | Shanghai, 2021 |

## Table D2 — Market Performance (IPO → 2026-06-25)

| Metric | Zhipu (2513.HK) | MiniMax (00100.HK) |
|---|---|---|
| IPO price (HK$) | 116.20 | 165.00 |
| Day-1 close (HK$) | 131.5 | 345.0 (+109%) |
| Latest close 2026-06-25 (HK$) | 2,350.0 | 456.6 |
| Return vs IPO | **+1,922%** | +177% |
| Period high (close, HK$) | 2,410.0 | 1,238.0 |
| Period low (close, HK$) | 131.5 | 345.0 |
| Trading days | 112 | 111 |
| Latest market cap | ~HK$969B (~US$124B) | ~ [confirm; mcap moved with price] |

> Cross-check: independent quote sources show 2513.HK ≈ HK$2,228 / mcap ≈ HK$969B on 2026-06-25; Tushare close
> = HK$2,350. Reconcile to official HKEX close in final paper. Today's date: 2026-06-26.

## Table D3 — Risk / Volatility

| Metric | Zhipu | MiniMax |
|---|---|---|
| Annualized volatility (daily, ×√252) | **192.5%** | 155.3% |
| Pattern | Still near highs | Boom-bust (peaked 1,238 → 456) |
| Beta | **TBD** — HK index not in feed; use bottom-up/comparable beta (global AI-software comps, unlever→relever) |

## Table D4 — Fundamentals (revenue & losses, US$)

| Period | Zhipu revenue | Zhipu net result | MiniMax revenue |
|---|---|---|---|
| FY2023 | ~US$17M | loss [confirm] | [confirm] |
| FY2024 | ~US$44M | loss [confirm] | [confirm] |
| H1 2025 | US$27.3M | **net loss ~US$329M** (R&D-driven) | — |
| 9M 2025 | — | — | revenue **+170% YoY**, overseas >70% [confirm absolute] |
| FY2026E | "on track to cross US$200M" | — | [confirm] |

> Implied valuation multiple (illustrative): US$124B cap / US$200M FY26E revenue ≈ **~600x P/S** (sanity-check figure for §8).

## Table D5 — Product / Competitive Data (for §5 leaderboard thread)

| Item | Detail | Source note |
|---|---|---|
| GLM-4.6 | ~355B params / 32B active (MoE), 200K context, open-weight, Sep 2025 | confirm specs |
| GLM-4.6 coding | ~near-parity vs Claude Sonnet 4 in human-eval coding | confirm |
| GLM-5.1 | Released 2026-03-27; **#1 SWE-Bench Pro = 58.4%**; ~2.6 pts behind Claude Opus 4.6 | confirm |
| "GLM-5.2" | User-referenced; **not yet verified** — check before citing | OPEN ITEM |
| Z.ai / Z.code | Developer coding platform topping coding leaderboards | confirm metrics |
| Strategy | open-weight + low token price = cost-disruption / developer flywheel | thesis |

## Table D6 — Capability-Event Log (event-study sample skeleton for §9)

Only events **after listing (2026-01-08)** are usable for CAR. To be populated with exact dates + a
capability-surprise score (benchmark delta vs prior SOTA / vs expectation). Pre-listing events (e.g. GLM-4.6,
Sep 2025) are context only.

| Date | Issuer | Event | Type | Capability-surprise proxy | Usable for CAR? |
|---|---|---|---|---|---|
| 2026-03-27 | Zhipu | GLM-5.1 release; #1 SWE-Bench Pro (58.4%) | model + benchmark | Δ vs prior SOTA / vs Opus 4.6 gap (2.6 pts) | ✅ in-window |
| [confirm] | Zhipu | "GLM-5.2" (user-mentioned) | model | **UNVERIFIED — confirm or drop** | ? |
| [confirm] | Zhipu | Z.code leaderboard top ranking | benchmark | rank change | ? |
| [confirm] | MiniMax | major model release(s) post-listing | model | Δ vs SOTA | ? |
| [confirm] | both | sovereign / large enterprise deals | commercial | deal size | ? |

> Action: build the full dated event list from Z.ai/MiniMax release notes + leaderboard histories
> (SWE-Bench Pro, LMArena) before running CAR. Target ≥ 8–12 in-window events across both issuers; if fewer,
> report as *diagnostic* (repo-style honesty box).

## Open data items to resolve before drafting §3 & §8
1. Zhipu full P&L, balance sheet, cash & equivalents, shares outstanding (basic/diluted) — from 18C prospectus.
2. Exact gross margin and R&D/revenue ratio.
3. MiniMax absolute revenue/loss and current market cap.
4. Comparable set for beta and EV/Sales: global AI-software / frontier-lab private rounds.
5. Confirm or drop "GLM-5.2" claim.

---

### Sources
- Caixin Global — Zhipu AI Hong Kong IPO ($640M) and debut, 2025-12-30 / 2026-01-08.
- CNBC — "First of China's AI tigers goes public" (Zhipu), 2026-01-08; MiniMax debut, 2026-01-09.
- Pandaily — Zhipu HK$3B cornerstone commitments.
- Yahoo Finance / CNBC / stockanalysis.com / Bloomberg — 2513.HK quote & market cap (2026-06-25).
- Bloomberg / HKET / The Paper / TechNode — MiniMax IPO (HK$165, US$619–620M, +109% debut).
- HowAIWorks / Hugging Face (zai-org/GLM-4.6) / Serenities AI — GLM-4.6 & GLM-5.1 specs and benchmarks.
- Market prices: Tushare `hk_daily` (token-based), retrieved 2026-06-26 → `data/*.csv`.
