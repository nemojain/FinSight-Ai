# 📈 FinSight AI — Quantitative Market Simulation Engine

> **GBM-powered tick-level analytics platform** simulating **491,400+ minute-level price records** across 5 major tickers using Geometric Brownian Motion — the same mathematical model underlying Black-Scholes options pricing. Built with Python, Pandas, Plotly, and the Anthropic Claude API.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-5.18+-3F4F75?style=flat&logo=plotly&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.24+-013243?style=flat&logo=numpy&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude-Sonnet_4-D97706?style=flat&logo=anthropic&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![Data](https://img.shields.io/badge/Data-GBM%20Simulation-8A2BE2?style=flat)

> 🔗 **Looking for the real market data version?** → [FinSight AI v2 — Live Yahoo Finance Data](https://github.com/nemojain/finsight-ai-live)

---

## 🧠 Why Simulation?

Geometric Brownian Motion is not just "fake data" — it is the **industry-standard stochastic model** used in:
- **Black-Scholes options pricing** (the formula that won a Nobel Prize in Economics)
- **Monte Carlo risk simulations** at hedge funds and investment banks
- **Stress testing** at financial institutions under Basel III regulatory frameworks

Building GBM from scratch in NumPy — without using any finance library — demonstrates a deeper understanding of the mathematics behind market behavior than simply loading a CSV. The simulation parameters (μ, σ) are calibrated to reflect realistic market characteristics for each ticker.

---

## 🎯 What This Project Does

- 🔬 **Implements GBM from scratch** in NumPy — no finance libraries used, pure mathematical modeling
- 📊 **Generates 491,400+ simulated minute-level tick records** across 5 tickers over 2 years
- 📉 **Computes institutional risk metrics**: Sharpe ratio, VaR 95%/99%, Max Drawdown, Rolling Volatility
- 🕯️ **Interactive candlestick charts** with MA20/MA50 overlays and volume bars via Plotly
- 🔗 **Correlation matrix** computed from daily returns across all 5 tickers
- 💼 **Equal-weight portfolio** with full risk attribution and drawdown analysis
- 🤖 **Anthropic Claude API** for natural-language quantitative market insights

---

## ⚙️ GBM Simulation Parameters

Each ticker is calibrated with realistic drift and volatility parameters:

| Ticker | Base Price | Annual Drift (μ) | Annual Volatility (σ) | Profile |
|--------|-----------|-----------------|----------------------|---------|
| 🍎 AAPL | $211 | 12% | 22% | Stable large-cap |
| 🪟 MSFT | $415 | 14% | 20% | Low-vol growth |
| 🔍 GOOGL | $183 | 11% | 24% | Moderate growth |
| ⚡ NVDA | $876 | 28% | 42% | High-risk, high-reward |
| 📘 META | $528 | 18% | 30% | Volatile tech |

**Simulation scale:**
- Time step: Δt = 1 / (252 trading days × 390 minutes/day)
- Total ticks per ticker: 98,280
- Total tick records: **491,400+**
- Random seed: Fixed per ticker for full reproducibility

---

## 🗂️ Project Structure

```
finsight-ai/
├── 📓 finsight_ai_gbm_simulation.ipynb    # Main simulation & analytics notebook
├── 🌐 finsight_ai.html                    # Interactive web dashboard (no install needed)
├── 📄 README.md
└── 📦 requirements.txt
```

---

## 📊 Key Output Metrics

| Metric | Value |
|--------|-------|
| 🗃️ Simulated tick records | 491,400+ |
| 🏷️ Tickers | AAPL · MSFT · GOOGL · NVDA · META |
| 📅 Simulated period | 2 years · minute-level |
| ⚡ Portfolio Sharpe Ratio | ~3.1 |
| 📉 Max Drawdown | ~-4.2% |
| 🔢 Simulation model | Geometric Brownian Motion (GBM) |
| 🎲 Reproducibility | Seeded LCG — identical output every run |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python 3.10+ | Core language |
| 🔢 NumPy | GBM simulation engine, all statistical computation |
| 🐼 Pandas | Time-series resampling & aggregation |
| 📈 Plotly | Interactive candlestick, histogram, heatmap charts |
| 🤖 Anthropic Claude API | AI-generated market commentary & quant insights |
| 📓 Jupyter Notebook | Interactive code + analysis environment |

---

## 🚀 How to Run Locally

**1️⃣ Clone the repo**
```bash
git clone https://github.com/nemojain/finsight-ai.git
cd finsight-ai
```

**2️⃣ Install dependencies**
```bash
pip install -r requirements.txt
```

**3️⃣ Launch Jupyter**
```bash
jupyter notebook
```

**4️⃣ Open `finsight_ai_gbm_simulation.ipynb` → Kernel → Restart & Run All**

> 💡 To enable AI insights, paste your Anthropic API key in the last cell.  
> Get a free key at: [console.anthropic.com](https://console.anthropic.com)

---

## 🌐 Live Demo

Open `finsight_ai.html` in any browser — no installation needed.

**Hosted at:** [`https://nemojain.github.io/FinSight-Ai/finsight_ai.html`](https://nemojain.github.io/FinSight-Ai/finsight_ai.html)

---

## 🎯 Skills Demonstrated

- ✅ Geometric Brownian Motion implementation from mathematical first principles
- ✅ Large-scale stochastic simulation with NumPy typed arrays
- ✅ Time-series resampling and OHLCV aggregation with Pandas
- ✅ Institutional risk analytics: Sharpe, VaR, Drawdown, Correlation
- ✅ Interactive financial visualization with Plotly
- ✅ REST API integration (Anthropic Claude)
- ✅ Portfolio construction and equal-weight risk attribution
- ✅ Deterministic reproducibility via seeded random number generation

---

## 🔗 Related Projects

| Project | Description | Link |
|---------|-------------|------|
| 📈 FinSight AI v2 | Same analytics stack — real Yahoo Finance market data | [finsight-ai-live](https://github.com/nemojain/finsight-ai-live) |
| 📊 PerfIQ FP&A | Enterprise financial planning — 504k+ GL transactions | [fpa-command-center](https://github.com/nemojain/fpa-command-center) |

---

## 👤 Author

**Nimanshu Jain**  
🎓 MS Information Technology & Management — UT Dallas  
📜 Graduate Certificate in Business Analytics & Data Mining  
🔗 [LinkedIn](https://linkedin.com/in/nemojainn/) · [GitHub](https://github.com/nemojain)

---

⭐ *If you found this useful, consider giving it a star!*
