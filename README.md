# 📈 Financial Time Series Analysis

A comprehensive Python-based analysis of major financial assets using 5 years of historical market data (2021–2026). This project explores price trends, returns, risk metrics, correlations, and anomalies to derive actionable investment insights.

---

## 📌 Assets Analyzed

| Ticker | Asset |
|--------|-------|
| `AAPL` | Apple Inc. |
| `NVDA` | NVIDIA Corporation |
| `SPY` | S&P 500 ETF (Benchmark) |
| `GLD` | Gold ETF |
| `BTC-USD` | Bitcoin |

**Period:** January 2021 – January 2026  
**Data Source:** Yahoo Finance via `yfinance`

---

## 🔍 Project Overview

This project answers a core question in quantitative finance:

> *Which asset delivers the best return per unit of risk — and how do they behave together?*

The analysis is structured across 14 sections covering the full lifecycle from raw data to investment insights.

---

## 📂 Repository Structure

```
financial-time-series-analysis/
│
├── Financial_Time_Series.ipynb   # Main analysis notebook
├── README.md                     # Project documentation
└── requirements.txt              # Python dependencies
```

---

## 📊 Analysis Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | Library Imports | NumPy, Pandas, Matplotlib, Seaborn, yfinance |
| 2 | Data Loading | 5-year OHLCV data download via yfinance API |
| 3 | Exploratory Data Analysis | Shape, dtypes, missing value inspection |
| 4 | Closing Price Extraction | Isolating the primary price signal |
| 5 | Data Cleaning | Handling calendar misalignments (equity vs. crypto) |
| 6 | Price Visualization | Raw prices + normalized performance (Base = 100) |
| 7 | Daily Returns | Percentage change calculation and validation |
| 8 | Risk vs. Return Analysis | Mean return, volatility, scatter plot comparison |
| 9 | Correlation Analysis | Return correlations + heatmap visualization |
| 10 | Moving Average Analysis | 50-Day & 200-Day MA for NVDA (Golden/Death Cross) |
| 11 | Anomaly Detection | 3-Sigma rule to flag extreme return events on NVDA |
| 12 | Sharpe Ratio | Risk-adjusted return ranking across all assets |
| 13 | Maximum Drawdown | Peak-to-trough decline (worst historical loss) |
| 14 | Summary & Key Takeaways | Consolidated performance table + insights |

---

## 🏆 Key Findings

| Metric | Best Performer | Worst Performer |
|--------|---------------|-----------------|
| Total Return | NVDA | GLD |
| Volatility (Risk) | GLD (lowest) | BTC-USD (highest) |
| Sharpe Ratio | NVDA | BTC-USD |
| Maximum Drawdown | SPY / GLD | BTC-USD |

**Insights:**
- **NVDA** dominated on both raw and risk-adjusted returns, driven by the AI boom
- **BTC-USD** offered extreme upside but with the highest volatility and deepest drawdown
- **GLD** acted as a stable low-volatility hedge with modest but consistent returns
- **SPY** delivered steady market returns with controlled risk — a reliable benchmark
- Combining these assets in a portfolio can reduce overall risk through diversification

---

## ⚙️ Tech Stack

- **Python 3.x**
- **pandas** — data manipulation and time series handling
- **numpy** — numerical computations
- **matplotlib** — custom charting and visualization
- **seaborn** — correlation heatmaps
- **yfinance** — financial data retrieval from Yahoo Finance

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Esha-Rahim/financial-time-series-analysis.git
cd financial-time-series-analysis
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the Notebook
```bash
jupyter notebook Financial_Time_Series.ipynb
```

> **Note:** The notebook downloads live data from Yahoo Finance on execution. An internet connection is required.

---

## 📦 requirements.txt

```
numpy
pandas
matplotlib
seaborn
yfinance
jupyter
```

---

## 📈 Visualizations Included

- Asset prices over time (raw closing prices)
- Normalized performance comparison chart (Base = 100)
- Risk vs. Return scatter plot
- Correlation heatmap (coolwarm)
- NVDA price with 50-Day & 200-Day moving averages
- NVDA daily return anomaly chart (3-sigma flagging)
- Sharpe Ratio bar chart
- Maximum Drawdown bar chart

---

## 👩‍💻 Author

**Esha Rahim**  
BS Software Engineering — University of Agriculture Faisalabad (UAF)  
📧 esharahim30@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/esha-rahim-7673163ab) · [GitHub](https://github.com/Esha-Rahim)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

*Built with Python · pandas · matplotlib · seaborn · yfinance*
