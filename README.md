# 能力惊喜，而非盈余惊喜：智谱AI（2513.HK）估值与定价研究 | Capability Surprise, Not Earnings Surprise: Valuing Zhipu AI (2513.HK)

<p align="center">
  <a href="#中文"><img src="https://img.shields.io/badge/语言-中文-E84D3D?style=for-the-badge&labelColor=3B3F47" alt="中文"></a>
  &nbsp;
  <a href="#english"><img src="https://img.shields.io/badge/Language-English-2F73C9?style=for-the-badge&labelColor=3B3F47" alt="English"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/标的-智谱AI · 2513.HK-F2C94C?style=for-the-badge" alt="2513.HK">
  <img src="https://img.shields.io/badge/上市-港交所主板 · 第18C章-4CAF50?style=for-the-badge" alt="HKEX 18C">
  <img src="https://img.shields.io/badge/论文-XeLaTeX-008080?style=for-the-badge&logo=latex&logoColor=white" alt="XeLaTeX">
  <img src="https://img.shields.io/badge/市销率-~620x · DCF缺口~98%25-9B51E0?style=for-the-badge" alt="P/S 620x">
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="MIT">
</p>

> **作者 / Author:** Zhesheng Xu（许哲圣） · **学号 / Student ID:** 42353012 · 公司金融期末项目 / Corporate Finance Final Project

---

## 中文

### 一句话概览

本项目对全球**首家上市的基础大模型公司**——智谱AI（Knowledge Atlas，2513.HK，2026-01-08 经港交所第18C章上市）——做公司金融估值与定价机制研究。核心不是"算出一个目标价"，而是回答一个反直觉的问题：**一家 2026 年预计收入仅约 2 亿美元、毛利率已跌至 −0.4%、净权益为负的公司，为何上市五个月暴涨约 19 倍、市值冲到约 1240 亿美元（市销率约 620 倍）？**

**主结论：** 这既不是单纯的泡沫，也不是有效定价，而是 **"对赢家通吃 AGI 结局的看涨期权 + 能力动量定价"**。基本面 DCF 仅支撑约 HK$47/股（约为市价的 2%）；现价隐含 2035 年收入 640 亿美元、9 年 90% 复合增速。市场的价格发现已从"盈余惊喜"转向**"能力惊喜"**——围绕模型发布与榜单登顶定价。

### 快速导航

| 你想看什么 | 入口 |
|---|---|
| 研究问题与原创点 | [研究问题](#研究问题) |
| 双支柱论证结构 | [核心论点](#核心论点) |
| 估值结论（DCF/反向/可比） | [估值结论](#估值结论) |
| 能力惊喜事件研究 | [事件研究](#事件研究) |
| 图表 | [关键图表](#关键图表) |
| 数据来源 | [数据来源](#数据来源) |
| 如何编译论文 | [如何编译](#如何编译) |

### 研究问题

> 当一家公司**没有盈余可被"惊喜"**时，如何用公司金融理论为它估值，又如何检验市场对它的定价是否有效？

经典市场有效性检验依赖"盈余惊喜"事件研究（Ball-Brown 1968；Bernard-Thomas 1989）。但前沿大模型公司处于深度亏损、pre-revenue 阶段，盈余无从"惊喜"。本文的处理方式：把信息事件由"盈余惊喜"替换为 **"能力惊喜"（capability surprise）**——即模型发布与基准榜单跃迁，并迁移国信证券《超预期投资全攻略》(2020) 的事件研究框架（CAR 三窗口）到这一新资产类别。

### 核心论点

论文采用**双支柱**结构：

| 支柱 | 内容 | 结论 |
|---|---|---|
| **A — 基本面锚** | CAPM/WACC、三情景 DCF、反向 DCF、可比公司、实物期权 | 内在价值远低于市价；溢价的本质是期权时间价值 |
| **B — 原创实证** | 能力惊喜事件研究（GLM-5 → GLM-5.2，对照 MiniMax） | 市场对能力即时且有辨别力地反应，但存在 PCAD 漂移 |

### 估值结论

WACC ≈ 13.5%（CAPM，自下而上 β≈1.6，Rf 4%，ERP 6%）。活公式模型见 [`model/valuation_model.xlsx`](model/valuation_model.xlsx)。

| 情景 | 收入CAGR '26–35 | 终期利润率 | 股权价值 | 每股(HK$) |
|---|---:|---:|---:|---:|
| 悲观 (p=0.35) | 21% | 18% | $1.6B | 29 |
| 中性 (p=0.45) | 31% | 28% | $2.5B | 46 |
| 乐观 (p=0.20) | 43% | 35% | $4.7B | 84 |
| **概率加权** | — | — | **$2.6B** | **47** |
| *市价 (2026-06)* | — | — | *$124B* | *2,228* |

**反向 DCF：** 要支撑现价，需相信 2035 年收入约 **$64B**（9 年 **90%** 复合增速，约 318× FY26E）——超级算力巨头级别。市场市销率约 **620×**，而 OpenAI/Anthropic 一级市场约 30–40×。

### 事件研究

把模型发布/榜单事件当作信息事件，计算累计异常收益（CAR，均值调整；以 MiniMax 为基准做同业调整稳健性）。

| 事件 | Day 0 | 反应[0,+1] | 漂移[+2,+10] | 读数 |
|---|---|---:|---:|---|
| GLM-5 | 2026-02-11 | +20.4% | +15.4% | 反应不足 |
| GLM-5-Turbo | 2026-03-16 | +10.3% | −7.7% | 小幅反转 |
| GLM-5.1 | 2026-04-08 | +11.9% | −22.8% | 过度反应 |
| GLM-5.2 | 2026-06-15 | +27.4% | +32.4% | 强反应不足 |
| *MiniMax M2.7* | 2026-03-18 | +4.5% | −3.8% | 哑火/板块分化 |

**要点：** ① 数据盲测出的最大异常日几乎一一命中 GLM 发布日；② 反应一致为正（均值 +17.5%），漂移分化（SOTA 跃迁反应不足、增量升级过度反应）；③ **同业调整后漂移全部转正**（+4.3% → +20.8%），GLM-5.1 的"过度反应"翻为延续，证明其反转主要是板块效应；④ 2/20、5/13 两个尖峰为**非能力的指数/资金流事件**（恒生科技纳入、港股通预期）。

### 关键图表

<p align="center"><img src="figures/fig1_price_paths.png" width="800" alt="价格路径"></p>
<p align="center"><img src="figures/fig3_car_eventtime.png" width="640" alt="平均CAR"></p>
<p align="center"><img src="figures/fig4_reaction_vs_drift.png" width="560" alt="反应vs漂移"></p>

### 数据来源

- **行情：** Tushare `hk_daily`（2513.HK、00100.HK），见 [`data/`](data/)。
- **财务：** 港交所第18C章招股书及 H1 2025 中报（见论文附录 A）。
- **能力事件：** GLM / MiniMax 发布日与 SWE-Bench Pro 等榜单。
- **新闻：** Caixin、CNBC、SCMP、Investing.com、Baker McKenzie 等（论文以脚注标注）。

> ⚠️ 复现行情需自备 Tushare token，通过环境变量传入，切勿写入代码或提交到仓库。

### 项目结构

```text
.
├── paper/                 # 论文 XeLaTeX 源 (main.tex, refs.bib) 与 main.pdf
├── model/                 # 活公式估值模型 valuation_model.xlsx
├── eventstudy/            # 事件研究 CAR 结果 (zhipu_car.csv, car_robustness.csv)
├── figures/               # 论文/README 图表
├── data/                  # Tushare 行情 CSV
├── OUTLINE.md             # 详细大纲
├── DATA_TABLES.md         # 数据表与来源
└── EVENT_STUDY.md         # 事件研究分析稿
```

### 如何编译

```bash
cd paper
# 需 TeX Live + XeLaTeX（论文含中文，必须用 xelatex）
xelatex -interaction=nonstopmode main.tex
bibtex   main
xelatex -interaction=nonstopmode main.tex
xelatex -interaction=nonstopmode main.tex
```

---

## English

### At A Glance

This project is a corporate-finance valuation and price-discovery study of the world's **first publicly listed
foundation-model company** — Zhipu AI (Knowledge Atlas, 2513.HK, listed on the HKEX Main Board under
Chapter 18C on 2026-01-08). The goal is not a target price but an answer to a counter-intuitive question:
**why did a firm with only ~US$200m expected 2026 revenue, a gross margin that has fallen to −0.4%, and
negative book equity rise ~19x in five months to a ~US$124B market cap (≈620× sales)?**

**Main conclusion:** this is neither a simple bubble nor efficient pricing, but **a call option on a
winner-take-all AGI outcome, priced through capability momentum**. A disciplined DCF supports only ~HK$47/share
(≈2% of the market price); the price embeds US$64B of revenue by 2035 at a 90% CAGR. Price discovery has
shifted from *earnings surprise* to **capability surprise** — pricing built around model releases and
leaderboard wins.

### Research Question

> When a company **has no earnings to be surprised by**, how can corporate-finance theory value it, and how
> can we test whether the market prices it efficiently?

We replace the earnings-surprise event study (Ball-Brown 1968; Bernard-Thomas 1989) with a
**capability-surprise** one — model releases and benchmark-leaderboard jumps — porting the CAR three-window
design of Guosen Securities (2020) to a new asset class.

### Core Argument — Two Pillars

| Pillar | Content | Finding |
|---|---|---|
| **A — Fundamental anchor** | CAPM/WACC, three-scenario DCF, reverse DCF, comparables, real options | Intrinsic value far below market; the premium is option time value |
| **B — Original empirics** | Capability-surprise event study (GLM-5 → GLM-5.2 vs MiniMax) | Immediate, discriminating reaction, but with PCAD drift |

### Valuation Summary

WACC ≈ 13.5% (CAPM, bottom-up β≈1.6). Live workbook: [`model/valuation_model.xlsx`](model/valuation_model.xlsx).

| Scenario | Rev. CAGR '26–35 | Term. margin | Equity | Per share (HK$) |
|---|---:|---:|---:|---:|
| Bear (p=0.35) | 21% | 18% | $1.6B | 29 |
| Base (p=0.45) | 31% | 28% | $2.5B | 46 |
| Bull (p=0.20) | 43% | 35% | $4.7B | 84 |
| **Prob-weighted** | — | — | **$2.6B** | **47** |
| *Market (2026-06)* | — | — | *$124B* | *2,228* |

**Reverse DCF:** justifying the price requires ~US$64B revenue by 2035 (90% CAGR, ≈318× FY26E). Market P/S
≈ 620× vs ~30–40× for OpenAI/Anthropic private rounds.

### Event Study

| Event | Day 0 | Reaction [0,+1] | Drift [+2,+10] | Reading |
|---|---|---:|---:|---|
| GLM-5 | 2026-02-11 | +20.4% | +15.4% | under-reaction |
| GLM-5-Turbo | 2026-03-16 | +10.3% | −7.7% | mild reversal |
| GLM-5.1 | 2026-04-08 | +11.9% | −22.8% | over-reaction |
| GLM-5.2 | 2026-06-15 | +27.4% | +32.4% | strong under-reaction |
| *MiniMax M2.7* | 2026-03-18 | +4.5% | −3.8% | muted / de-rate |

Blind-detected abnormal days map onto GLM releases; reaction is robust (mean-adj +17.5% vs peer-adj +18.5%),
and drift **strengthens to +20.8%** once the falling sector is removed (PCAD survives). Two spikes (Feb-20,
May-13) are non-capability index/flow events (Hang Seng Tech inclusion, Stock Connect).

### Repository Structure

```text
.
├── paper/      # Thesis XeLaTeX source (main.tex, refs.bib) and main.pdf
├── model/      # Live-formula valuation model
├── eventstudy/ # CAR results
├── figures/    # Figures
└── data/       # Tushare market-data CSVs
```

### How to Build

```bash
cd paper
xelatex -interaction=nonstopmode main.tex   # XeLaTeX required (CJK content)
bibtex   main
xelatex -interaction=nonstopmode main.tex
xelatex -interaction=nonstopmode main.tex
```

> ⚠️ Reproducing the market data needs your own Tushare token, passed via an environment variable — never
> commit it.

---

## License

MIT License — see [LICENSE](LICENSE). Copyright (c) 2026 Zhesheng Xu (许哲圣).
