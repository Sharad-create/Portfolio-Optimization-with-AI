# Portfolio-Optimization-with-AI
# 📊 Portfolio Optimization & Risk Analysis using Python

This project applies **Modern Portfolio Theory (MPT)** to optimize a real-world equity portfolio.  
It uses live stock holdings, historical market data, and quantitative methods to identify the **Global Minimum Variance (GMV)** and **Maximum Sharpe Ratio** portfolios.

---

## 🧩 Project Overview

**Objective:**  
To construct, analyze, and optimize a multi-asset stock portfolio based on actual holdings, balancing **risk** and **return** using Python.

**Key Outcomes:**
- Identified *Global Minimum Variance* and *Maximum Sharpe Ratio* portfolios.
- Simulated 1,000,000 random portfolios to trace the **Efficient Frontier**.
- Recommended optimal weights for a **₹5,00,000 conservative-growth investor**.
- Compared Actual vs Optimized portfolios in tabular and graphical formats.

---

## ⚙️ Workflow Summary

| Step | Process | Key Tools |
|------|----------|-----------|
| **1** | Data Import: Broker portfolio + Yahoo Finance | `pandas`, `yfinance` |
| **2** | Data Cleaning & Preprocessing | `pandas`, `numpy` |
| **3** | Compute Daily & Annual Returns, Covariance Matrix | `pandas` |
| **4** | Risk/Return Visualization (Heatmap, Correlations) | `matplotlib`, `seaborn` |
| **5** | Monte Carlo Simulation (1,000,000 Portfolios) | `numpy` |
| **6** | Portfolio Optimization (GMV & Max Sharpe) | `scipy.optimize.minimize` |
| **7** | Capital Allocation Line & Recommendation | `matplotlib`, `numpy` |

---

## 📈 Results Summary

| Portfolio | Expected Annual Return | Annual Risk (Std) | Sharpe Ratio |
|------------|-----------------------|-------------------|---------------|
| **Actual Portfolio** | 11.4% | 14.2% | 0.62 |
| **Global Min Variance** | 9.8% | 10.6% | 0.72 |
| **Max Sharpe Portfolio** | 15.7% | 18.3% | 0.85 |

*(Values indicative — computed dynamically in code)*

---

## 📊 Portfolio Weights Comparison (Top 10)

| Symbol | Actual Weight | GMV Weight | Max Sharpe Weight |
|---------|----------------|-------------|-------------------|
| HDFCBANK | 0.164 | 0.220 | 0.236 |
| HINDUNILVR | 0.015 | 0.199 | 0.000 |
| TCS | 0.036 | 0.160 | 0.000 |
| ITC | 0.008 | 0.131 | 0.000 |
| BERGEPAINT | 0.015 | 0.098 | 0.000 |
| BHARTIARTL | 0.012 | 0.053 | 0.483 |
| HAVELLS | 0.018 | 0.042 | ~0.000 |
| BANKINDIA | 0.018 | 0.037 | 0.000 |
| UNITDSPR | 0.021 | 0.031 | 0.000 |
| DABUR | 0.005 | 0.010 | 0.000 |

---

## 💡 Investment Recommendation

For a **conservative investor seeking growth** with ₹5,00,000:  
- Allocate **70%** to the **Global Minimum Variance Portfolio** (stability focus).  
- Allocate **30%** to the **Max Sharpe Portfolio** (growth focus).  

> This hybrid approach balances risk and return efficiently, offering steady growth with controlled volatility.

---

## 🧮 Formulas Used

\[
R_p = \sum_{i=1}^{n} w_i R_i
\]

\[
\sigma_p = \sqrt{w^T \Sigma w}
\]

\[
\text{Sharpe Ratio} = \frac{R_p - R_f}{\sigma_p}
\]

Where:
- \( R_p \): Portfolio Return  
- \( \sigma_p \): Portfolio Standard Deviation  
- \( R_f \): Risk-Free Rate  
- \( w_i \): Weight of asset \(i\)  
- \( \Sigma \): Covariance Matrix  

---

## 🧠 Technologies Used
- **Python**: Data analysis and optimization  
- **Libraries**: `numpy`, `pandas`, `yfinance`, `matplotlib`, `seaborn`, `scipy`
- **Optimization Method**: Sequential Least Squares Programming (SLSQP)

---

## 📁 Repository Structure

