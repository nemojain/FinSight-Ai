# 📈 FinSight AI — Tick-Level Market Analytics

> **AI-powered quantitative finance dashboard** analyzing **491,400+ synthetic tick records** across 5 major tickers over 2 years of simulated minute-level trading data — built with Python, Pandas, Plotly, and the Anthropic Claude API.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-5.18+-3F4F75?style=flat&logo=plotly&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.24+-013243?style=flat&logo=numpy&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude-Sonnet_4-D97706?style=flat&logo=anthropic&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)

---

## 🧠 What This Project Does

This project simulates a full **institutional-grade quantitative analytics pipeline** — the kind used by hedge funds, asset managers, and Big 4 financial consulting firms:

- 🔬 **Generates 491,400+ tick records** using Geometric Brownian Motion (GBM) — the same model used in Black-Scholes options pricing
- 📊 **Computes institutional risk metrics**: Sharpe ratio, VaR (95%/99%), Max Drawdown, Rolling Volatility
- 🕯️ **Interactive candlestick charts** with MA20/MA50 overlays and volume bars via Plotly
- 📉 **Return distribution analysis** with VaR markers for all 5 tickers
- 🔗 **Correlation matrix** computed from daily returns across AAPL, MSFT, GOOGL, NVDA, META
- 💼 **Equal-weight portfolio** with full risk attribution
- 🤖 **Anthropic Claude API** integration for natural-language quantitative insights

---

## 🗂️ Project Structure

```
finsight-ai/
├── 📓 finsight_ai.ipynb     # Main analysis notebook
├── 🌐 finsight_ai.html      # Interactive web dashboard (live demo)
├── 📄 README.md
└── 📦 requirements.txt
```

---

## 📊 Key Metrics (from simulation)

| Metric | Value |
|--------|-------|
| 🗃️ Total tick records | 491,400+ |
| 🏷️ Tickers | AAPL · MSFT · GOOGL · NVDA · META |
| 📅 Period | 2 years · minute-level |
| ⚡ Sharpe Ratio | ~3.1 |
| 📉 Max Drawdown | ~-4.2% |
| 🔢 Data model | Geometric Brownian Motion (GBM) |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🐍 Python 3.10+ | Core language |
| 🔢 NumPy | GBM simulation, statistical computation |
| 🐼 Pandas | Time-series resampling & aggregation |
| 📈 Plotly | Interactive candlestick, histogram, heatmap charts |
| 🤖 Anthropic Claude API | AI-generated market commentary & insights |
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

**4️⃣ Open `finsight_ai.ipynb` → Kernel → Restart & Run All**

> 💡 To enable AI insights, paste your Anthropic API key in the last cell.  
> Get a free key at: [console.anthropic.com](https://console.anthropic.com)

---

## 🎯 Skills Demonstrated

- ✅ Quantitative finance modeling (GBM, VaR, Sharpe, Drawdown)
- ✅ Large-scale synthetic data generation with NumPy
- ✅ Time-series resampling and aggregation with Pandas
- ✅ Interactive data visualization with Plotly
- ✅ REST API integration (Anthropic Claude)
- ✅ Portfolio risk analytics and attribution
- ✅ Statistical analysis (skewness, kurtosis, correlation)

---

## 🌐 Live Demo

> Open `finsight_ai.html` in any browser for the full interactive dashboard — no installation needed.

**Hosted at:** `https://nemojain.github.io/finsight-ai/finsight_ai.html`

---

## 👤 Author

**Nimanshu Jain**  
🎓 MS Information Technology & Management — UT Dallas  
📜 Graduate Certificate in Business Analytics & Data Mining  
🔗 [LinkedIn](https://linkedin.com/in/nimanshu-jain) · [GitHub](https://github.com/nemojain)

---

⭐ *If you found this project useful, consider giving it a star!*
