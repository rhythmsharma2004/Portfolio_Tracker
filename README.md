# 📈 Quantitative Portfolio Analytics Dashboard

A Python-based portfolio analytics system that tracks, analyzes, and optimizes stock portfolios using real market data and Modern Portfolio Theory.

Built by: Rhythm Sharma | IIT Jodhpur | B.Tech  
Date: July 2025

---

## 📌 Project Objective

Build a quantitative portfolio analytics dashboard to evaluate stock performance, risk metrics, and optimized allocations using Python — demonstrating the analytical and quantitative skills required for market-making and trading roles.

## 📌 Problem Statement

Retail and institutional investors need data-driven tools to:
1. Track portfolio performance against market benchmarks
2. Quantify risk using industry-standard metrics
3. Optimize asset allocation using Modern Portfolio Theory
4. Identify correlation patterns for better diversification

This project builds an **end-to-end portfolio analytics system** addressing all four requirements using real NSE market data.

---

## 🚀 Features

| Feature | Description |
|---|---|
| **Real-Time Data** | Live NSE stock data via Yahoo Finance API |
| **Portfolio Tracking** | Holdings, P&L, sector allocation |
| **Performance Analytics** | 13+ metrics including Sharpe, Sortino, VaR, Alpha, Beta |
| **Benchmark Comparison** | Portfolio vs Nifty 50 Index |
| **Correlation Analysis** | Inter-stock correlation for diversification insights |
| **Markowitz Optimization** | Mean-Variance optimization with Efficient Frontier |
| **Auto-Generated Insights** | Data-driven findings, not hardcoded |
| **Executive Summary** | Professional report with key takeaways |

---

## 📊 Portfolio Construction

The portfolio consists of **5 large-cap Indian equities** selected for **sector diversification**:

| Stock | Sector | Selection Rationale |
|---|---|---|
| **RELIANCE** | Energy/Conglomerate | Largest Indian company, diversified revenue |
| **TCS** | IT Services | Global IT leader, stable USD revenue |
| **INFOSYS** | IT Services | Growth-oriented, strong digital revenue |
| **HDFC BANK** | Banking & Finance | Largest private bank, India growth proxy |
| **ITC** | FMCG | Defensive stock, high dividend yield |

**Diversification Logic:**
- Mix of cyclical (Banking, Energy) and defensive (FMCG, IT) sectors
- Exposure to both domestic consumption and global revenue
- All stocks are Nifty 50 constituents → high liquidity

**Benchmark:** Nifty 50 Index (^NSEI)  
**Risk-Free Rate:** 7.0% (India 10Y Government Bond Yield)

---

## 📐 Metrics Calculated

### Performance Metrics
- Total Return & Annualized Return
- Annualized Volatility
- Win Rate, Best Day, Worst Day

### Risk Metrics
- **Sharpe Ratio** — Risk-adjusted return: `(Rp - Rf) / σp`
- **Sortino Ratio** — Downside risk only: `(Rp - Rf) / σd`
- **Maximum Drawdown** — Worst peak-to-trough loss
- **Value at Risk (95%)** — Daily loss threshold at 95% confidence
- **Conditional VaR (95%)** — Expected loss beyond VaR

### CAPM Metrics
- **Beta** — Market sensitivity: `Cov(Rp,Rm) / Var(Rm)`
- **Jensen's Alpha** — Excess return over CAPM: `Rp - [Rf + β(Rm - Rf)]`

### Optimization
- **Markowitz Mean-Variance Optimization**
- Max Sharpe Ratio Portfolio
- Min Volatility Portfolio
- Efficient Frontier (5000 simulated portfolios)

---

## 📈 Visualizations

1. **Portfolio vs Benchmark** — Cumulative returns comparison
2. **Sector Allocation** — Pie chart by sector
3. **Stock Allocation** — Pie chart by individual stock
4. **Portfolio Drawdown** — Peak-to-trough loss over time
5. **Correlation Heatmap** — Inter-stock return correlations
6. **Normalized Prices** — Individual stock performance (base 100)
7. **Efficient Frontier** — 5000 random portfolios with optimal points
8. **Monthly Returns Heatmap** — Calendar view of monthly performance

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| **Language** | Python 3.10+ |
| **Data Source** | Yahoo Finance API (`yfinance`) |
| **Data Analysis** | `pandas`, `numpy` |
| **Optimization** | `scipy.optimize` (SLSQP) |
| **Visualization** | `plotly` (interactive), `seaborn`, `matplotlib` |
| **Environment** | Google Colab / Jupyter Notebook |

## 🔮 Future Enhancements

- [ ] Streamlit interactive web dashboard
- [ ] Black-Litterman model for views-based optimization
- [ ] Sector rotation strategy based on macro indicators
- [ ] Options overlay analysis for hedging
- [ ] Real-time WebSocket data streaming
- [ ] Backtesting engine for strategy validation

---

## 👤 Author

Rhythm Sharma
B.Tech 
Indian Institute of Technology, Jodhpur  

📧 [rhythmsharmaiitj@gmail.com]  



