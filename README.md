<h1 align="center">Ansh Dani</h1>

<p align="center">
  Market microstructure · market making · C++ trading systems · volatility
</p>

<p align="center">
  M.S. Financial Mathematics, University of Chicago (Dec 2027)<br>
  B.S. Computer Science + B.S. Mathematics, Arizona State University (GPA 4.00, Summa Cum Laude)
</p>

<p align="center">
  <a href="https://anshdani.com">anshdani.com</a> ·
  <a href="https://www.linkedin.com/in/ansh-dani">LinkedIn</a> ·
  <a href="mailto:adani2@uchicago.edu">adani2@uchicago.edu</a>
</p>

---

I work on how orders, queues and liquidity behave in futures markets, and on what that means for
someone quoting in them. Most of my work starts from order-by-order (CME MBO) data and pre-registered
tests, and I report null results alongside the positive ones.

Currently: quantitative research in the **WH Trading × UChicago Project Lab** (delta hedging and
volatility forecasting on futures options), and a pre-registered study of order-book liquidity
around the weekly EIA energy releases.

### Projects

**[mbo-queue](https://github.com/AnshDani2004/mbo-queue)** · C++20, pybind11, Python · `pip install mbo-queue`
Rebuilds exact FIFO queues from CME market-by-order data and scores the queue-position models that
open-source market-making backtesters use (hftbacktest's risk-averse, power and log models;
Rigtorp) against the true queue: queue error, fill-rate bias, fill time and P&L bias. The C++ engine
and an independent Python reference agree bitwise; validated on a synthetic exchange with known
answers.

**[C++ Limit Order Book & Market-Making Simulator](https://github.com/AnshDani2004/cpp-limit-order-book-market-maker)** · C++20
Deterministic price-time matching engine (partial fills, cancel/replace, self-trade prevention,
flat-array book) at ~3.7M events/s, 125 ns p50 / 1.2 µs p99 over 1M events. Over 1,080 paired-seed
runs, Avellaneda-Stoikov quoting cut inventory variance in high volatility; under ITCH-calibrated
QQQ flow, fill rates fell below 2% because executions were sparse, and the risk-adjusted gain
disappeared.

**[BTC/USD Cross-Venue Price Discovery](https://github.com/AnshDani2004/cross-venue-price-discovery)** · Python
Which venue moves first, Coinbase or Kraken, on synchronized data: Granger causality, HAC
regressions and VAR/VECM over 10 paired sessions (9 usable), with stronger Coinbase-to-Kraken
predictability at short horizons.

**[SPY Volatility Surface Lab](https://github.com/AnshDani2004/vol-surface-research-lab)** · Python
Option-chain cleaning, IV inversion, Greeks, static-arbitrage checks and SABR/Heston calibration.
On one saved chain, SABR fit 206 liquid OTM quotes to 0.77 vol points RMSE and beat Heston on all
three expiries.

**[Honors Thesis: Bayesian Sequential Decision-Making](https://github.com/AnshDani2004/BSD_Thesis)** · Python, LaTeX
HMM regime detection with a CUSUM trigger feeding Kelly sizing under a drawdown floor, evaluated by
Monte Carlo on detection delay, ruin and wealth.

### Competitions

- **IMC Prosperity 4:** 256th of 18,800+ teams worldwide (top 1.4%, 194th algo)
- **Optiver × UChicago Explaining Markets:** 2nd globally 

### Tools

Python (NumPy, pandas, Polars, SciPy, statsmodels, PyTorch) · C++20, pybind11, CMake · SQL · R · Git, Linux, Docker
