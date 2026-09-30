## Darson Chen

M.S. Chemical Engineering at Northwestern (exp. Mar 2027). I do independent quantitative research on
market microstructure, LLM-driven equity screening and prediction markets, and I build agentic AI
development pipelines at work.

Most of my projects end with me proving my own first result was wrong: a leak, a cost, a bias or a
bug. I publish that part too.

### Research

| Project | What it is | Headline |
|---|---|---|
| [**hidden-liquidity-microstructure**](https://github.com/Darson2004/hidden-liquidity-microstructure) | Order-by-order book replay of 1,098 Databento MBO files; a from-scratch Hausman–Lo–MacKinlay ordered-choice model for hidden (iceberg) executions; streaming Hawkes / OFI / micro-price features feeding an XGBoost 5-second predictor | OOS R² 0.016 (t = 225), 31× a Stoikov baseline, and **untradable**: 0.86¢ edge vs a 2¢ round trip |
| [**catalyst-runway**](https://github.com/Darson2004/catalyst-runway) | Two-stage US equity screener: SEC EDGAR XBRL funnel, then an LLM deep-read of filings | Backtest IC of +0.20 was **leakage**: an LLM re-identifies 65–80% of "anonymized" companies. Replaced with a SHA-256-sealed prospective test (48 names, graded 2027–29) |
| [**prediction-market-microstructure**](https://github.com/Darson2004/prediction-market-microstructure) | Kalshi ↔ Polymarket venue clients, fee models, tick recorders on a cloud VM, queue-aware MM backtest, shadow-mode quoter | Taker arb is net-negative after fees (−1.39¢ mean); passive maker mark-outs +0.44¢ at 5 s over 98k fills; P&L leaks through inventory |
| [**kelly-event-vol**](https://github.com/Darson2004/kelly-event-vol) | Kelly sizing engine and a pre-earnings straddle backtest on real OPRA quotes, with measured fill costs | One rule survives costs: +6.39%/trade net (n = 193, t = 2.65), 5 of 6 years. The same trade in small caps is −17.3% net |
| [**preregistered-exploration**](https://github.com/Darson2004/preregistered-exploration) | A research protocol designed to say no: hashed evaluator, append-only trial log, adversarial audit, sealed one-shot validation | 74 logged trials across 3 questions; 0 cross-sectional tests survive BH-FDR; the audit's corrections are recorded, not quietly fixed |

### Other projects

- [**fantasy-draft-optimizer**](https://github.com/Darson2004/fantasy-draft-optimizer): lookahead
  drafting against a computable opponent model, season and injury Monte Carlo, and a projection
  calibration study. Wins 16.2% of held-out leagues vs a 10% luck baseline (+8.0 SE).
- [**MFT**](https://github.com/Darson2004/MFT): an early (2025) Mamba state-space model for
  post-earnings intraday trading. It failed, and why it failed is what sent me to order-book data.

### How I validate

Temporal hold-outs with hard cutoffs · fee and fill-cost models measured from real prints ·
look-ahead and de-anonymization audits for LLM components · multiple-testing correction (BH-FDR,
effective test counts) · pre-registration with content hashes · shadow mode before anything trades.

### Stack

Python (NumPy, SciPy, pandas, XGBoost, PyTorch) · SQL (Oracle PL/SQL, MSSQL) · TypeScript/React ·
C#/.NET · Databento, SEC EDGAR, Kalshi/Polymarket APIs · LLM agents (Anthropic API)

### Contact

[LinkedIn](https://www.linkedin.com/in/darson-chen) · darsonchen2026@u.northwestern.edu
