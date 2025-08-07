
# 📈 ENHANCING PAIRS TRADING: CLASSICAL VS LSTM-BASED STRATEGIES

## 🧠 Overview
This project investigates the effectiveness of classical statistical arbitrage (cointegration-based pairs trading) and compares it with an advanced machine learning approach using LSTM (Long Short-Term Memory) models. By applying both strategies to Indian banking sector stocks, we assess their profitability, risk-adjusted performance, and adaptability in various market conditions.

---

## 🎯 Objectives

- Identify cointegrated stock pairs from the Indian stock market
- Apply classical pairs trading strategy based on spread reversion
- Enhance the strategy using an LSTM-based prediction model
- Compare performance across multiple timeframes and volatility regimes

---

## 🧪 Methodology

### 1. Classical Pairs Trading (Baseline)
- Use **Engle-Granger Two-Step Test** for cointegration
- Compute spread and set dynamic trading boundaries
- Enter trades when spread exceeds thresholds, assuming mean reversion

### 2. LSTM-Enhanced Strategy
- Train an LSTM model on historical spreads to predict trend directions
- Filter trades with LSTM predictions to avoid trending markets
- Adjust trading thresholds dynamically based on volatility

### Dataset
- Source: Yahoo Finance
- Sector: Indian Banking
- Frequency: Daily (2020–2025), including high-frequency 1-minute data (for short intervals)

---

## 📊 Results & Visualizations

- Classical strategy gives higher number of trades and raw returns
- LSTM-based model improves **risk-adjusted returns**, reduces **drawdowns**, and filters **risky trades**
- Multiple evaluation metrics: win rate, cumulative returns, drawdown, trade count

---

## 🧩 Limitations

- Market frictions (e.g., slippage, transaction costs) not included
- LSTM model architecture and parameters are basic; can be optimized
- Results depend on specific stock pairs and timeframes

---

## 🔭 Future Work

- Apply alternative deep learning models (GRU, Transformers)
- Automate real-time trading with live market data
- Incorporate brokerage, slippage, stop-loss mechanisms
- Explore sector-wise and cross-sector pair formations

---

## 🛠️ Technologies Used

- **Languages:** Python
- **Libraries:** `pandas`, `numpy`, `statsmodels`, `yfinance`, `tensorflow`, `matplotlib`, `seaborn`
- **Models:** Engle-Granger Test, LSTM

---


## 📄 References

- Designing Efficient Pair-Trading Strategies Using Cointegration for the Indian Stock Market – Sen (2022)
- LSTM-Based Deep Learning Model for Predicting Pairs Trading Signals – PeerJ CS (2024)
