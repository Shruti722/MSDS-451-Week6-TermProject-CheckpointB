# MSDS-451-Week6-TermProject-CheckpointB
---
##  Overview

The project explores the design of an **actively managed ETF** focused on **large-cap technology companies**—AAPL, MSFT, and NVDA. The ETF is built around a **rule-based framework** that integrates:

- Traditional financial metrics (returns, volatility, Sharpe ratio)
- Market structure analysis (rolling volatility, correlations)
- Future integration of macroeconomic indicators and behavioral signals (Google Trends, sentiment)

This update includes enhanced exploratory data analysis (EDA), clean visuals, and improved risk-adjusted performance evaluation.

---

## Repository Structure

├── README.md

├── requirements.txt

│
├── reports/

│ └── 451-Week6-Term-Project-CheckpointB.pdf

│
├── notebooks/

│ └── Improved_quick_eda.ipynb

│
├── week4_improved_outputs/

│ ├── prices_levels.png

│ ├── prices_normalized.png

│ ├── daily_returns.png

│ ├── rolling_vol_21d.png

│ ├── correlation_matrix.png

│ ├── close_prices.csv

│ ├── log_returns.csv

│ ├── metrics.csv

│ └── correlations.csv

---

## How to Run the Notebook

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/MSDS451-Term-Project.git
cd MSDS451-Term-Project
```
### 2. Set up your Python environment

```
pip install -r requirements.txt
```
### 3. Launch the Jupyter Notebook

```
jupyter notebook notebooks/Improved_quick_eda.ipynb
```

This notebook will:

Download adjusted stock prices from Yahoo Finance

Compute log/daily returns, Sharpe ratio, volatility

Generate key visualizations and save outputs to /week4_improved_outputs/

## EDA Highlights (2025 Update)

| Metric | AAPL | MSFT | NVDA |
|:--------|:----:|:----:|:----:|
| **Annualized Return** | 0.23 | 0.26 | 0.49 |
| **Annualized Volatility** | 0.21 | 0.22 | 0.36 |
| **Sharpe Ratio (r<sub>f</sub>=2%)** | 1.00 | 1.09 | 1.31 |

- **NVDA** leads both in return and risk-adjusted return.  
- High pairwise correlations (~0.75–0.85) support macro-linked movement.  
- Rolling volatility indicates regime shifts (COVID-19, AI boom).

---
**Key Outputs** (saved in `week4_improved_outputs/`):

- `prices_levels.png`: Raw adjusted price comparison  
- `prices_normalized.png`: Price indexed to 100 from 2019 start  
- `daily_returns.png`: Daily return distribution  
- `rolling_vol_21d.png`: 21-day volatility trend  
- `correlation_matrix.png`: Heatmap of pairwise correlations  

---

## Research Report

A formal PDF write-up of **Week 6 Checkpoint B** is provided under: 451-Week6-Term-Project-CheckpointB.pdf


It includes:

- Project motivation and potential ETF use cases  
- Literature review from Grinold, Sharpe, Covel, and others  
- Updated methods, improved data processing  
- Detailed EDA results with embedded graphs  
- Next steps toward a full algorithmic ETF framework  

---

## Future Roadmap

- Integrate FRED macroeconomic indicators (interest rate, inflation)  
- Add Google Trends, Reddit/News sentiment (Alt-data)  
- Use ML models (e.g., XGBoost) for signal blending  
- Implement Monte Carlo portfolio optimization 



