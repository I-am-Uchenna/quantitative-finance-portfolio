# Quantitative Finance & Algorithmic Trading Portfolio

**A collection of quantitative research projects focusing on Algorithmic Trading, Risk Management, and Financial Engineering.**

## 🚀 Projects Overview

### 1. [Trend Following Optimization](01_Trend_Following_Strategy)
* **Objective:** Test the robustness of Moving Average strategies across different market regimes.
* **Method:** Implemented Walk-Forward Optimization to eliminate look-ahead bias.
* **Key Finding:** Identified "Parameter Lag" during V-shaped recoveries (2023), proving the need for dynamic volatility adjustment.

### 2. [Institutional Risk Dashboard (VaR)](02_Risk_Management_VaR)
* **Objective:** Model tail risk for a hypothetical equity portfolio.
* **Method:** Calculated Historical, Parametric, and Monte Carlo Value at Risk (95% Confidence).
* **Key Finding:** Backtesting revealed "Volatility Clustering" during the COVID-19 crash, with a breach rate of 5.86% (exceeding the 5% theoretical limit).

### 3. [Options Pricing Engine](03_Options_Pricing)
* **Objective:** Price European Call Options using numerical methods.
* **Method:** Built a Monte Carlo simulation (N=50,000) using Geometric Brownian Motion.
* **Key Finding:** Demonstrated convergence to the Black-Scholes analytical price with <$0.01 error, validating the Law of Large Numbers.

### 4. [Statistical Arbitrage (Kalman Filter)](04_Kalman_Filter_Arbitrage)
* **Objective:** Execute a market-neutral Pairs Trading strategy (EWC/EWA).
* **Method:** Utilized a **Kalman Filter** to estimate dynamic, time-varying hedge ratios (Beta) rather than static OLS regression.
* **Key Finding:** Achieved a market-neutral equity curve with a max drawdown of only **6.25%** during a period where the S&P 500 drew down ~25%.

---

## 🛠 Tech Stack
* **Python:** Core logic and vectorization.
* **Libraries:** `pandas`, `numpy`, `scipy`, `pykalman`, `yfinance`.
* **Visualization:** `matplotlib`, `seaborn`.

## 📦 How to Run
1. Clone the repo:
   ```bash
   git clone [https://github.com/I-am-Uchenna/quantitative-finance-portfolio.git](https://github.com/I-am-Uchenna/quantitative-finance-portfolio.git)
