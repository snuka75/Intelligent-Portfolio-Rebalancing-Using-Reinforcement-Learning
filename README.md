## 📌 Project Title

**RL-Driven Stock Portfolio Optimization with News Sentiment**

---

## 📈 Overview

This project implements a **Reinforcement Learning (RL)** agent to optimize a stock portfolio allocation strategy using:
- Historical price data of 10 major S&P 500 companies
- Financial news sentiment from real-time RSS headlines
- Proximal Policy Optimization (PPO) from Stable Baselines3

The agent is benchmarked against the **SPY ETF**, allowing a direct comparison between learned allocation strategies and passive market investing.

---

## 🧠 Key Features

- 📉 Stock allocation using PPO-based reinforcement learning
- 📰 News sentiment reward shaping using Hugging Face Transformers
- 💰 Transaction cost penalties for realistic simulation
- 📊 Visualizations: heatmaps, area plots, and performance metrics
- 📈 Performance comparison with SPY benchmark

---

## 🔧 Tech Stack

| Component         | Tool / Library                          |
|------------------|------------------------------------------|
| RL Algorithm      | PPO (Stable-Baselines3)                  |
| Data Source       | yFinance, Finviz RSS Feed                |
| Sentiment Model   | distilBERT (Hugging Face Transformers)   |
| Environment       | OpenAI Gym (Custom)                      |
| Visualization     | Matplotlib, Seaborn                      |

---

## 📂 File Structure

```
portfolio-optimization-rl/
├── portfolio_optimization_with_rl.py    # Main notebook
├── README.md                            # Project documentation
└── images/                              # Screenshots/outputs
```

---

## 🚀 Getting Started

### 1. Install Dependencies
```bash
pip install yfinance stable-baselines3 gym shimmy matplotlib ta transformers feedparser
```

### 2. Run the Notebook
```bash
Open portfolio_optimization_with_rl.py in Jupyter or Google Colab
```

---

## 🖼️ Visual Results

### 🔹 Portfolio Allocation Heatmap
![Heatmap](images/heatmap.png)

### 🔹 Portfolio Value vs. SPY Benchmark
![Portfolio vs SPY](images/portfolio_vs_spy.png)

### 🔹 Reward Breakdown Over Time
![Reward Breakdown](images/reward_breakdown.png)

---

## 📊 Performance Summary

| Metric           | RL Portfolio     | SPY Benchmark    |
|------------------|------------------|------------------|
| Final Value      | 2.57             | 1.84             |
| Return (%)       | 29.24%           | 23.49%           |
| Volatility (%)   | 38.96%           | 25.10%           |
| Sharpe Ratio     | 0.75             | 0.94             |

---

## 🏦 Real-World Use

- Simulate with live prices via `yfinance` or broker APIs
- Test with **Alpaca** or **Interactive Brokers** (paper trading)
- Add rebalancing frequency control and execution constraints

---

## 📌 Future Work

- Add Drawdown, Sortino ratio for better evaluation
- Deploy as Streamlit dashboard
- Add support for crypto or forex assets

---

## 👩‍💻 Author
**Samhitha Nuka**  
_M.S. Data Science, Indiana University Bloomington_

---
