# Stock Portfolio Analysis — Pakistani Equities

## Project Overview
Comprehensive financial analysis of 4 major Pakistani stocks (OGDC, LUCK, HBL, ENGRO) against the KSE-100 benchmark index. Analysis period: January 2019 – December 2025.

## What This Project Does
- Calculates daily and annual returns for individual stocks
- Measures risk using standard deviation and coefficient of variation
- Estimates Beta coefficients using regression analysis (CAPM framework)
- Builds portfolio combinations and analyzes risk-return tradeoffs
- Determines stock valuation using Security Market Line (SML)
- Compares systematic vs unsystematic risk

##  Key Findings
- **Best Performer:** Lucky Cement (LUCK) — 23.04% annual return
- **Most Volatile:** ENGRO — 30.26% annual volatility
- **Lowest Volatility:** KSE-100 Index — 17.82% (market baseline)
- **Beta Analysis:** All stocks showed low correlation with KSE-100 (idiosyncratic risk dominant)
- **Risk-Free Rate:** 11.35% (12-month T-Bill rate as of 2026)

##  Methodology

### 1. Data Collection
- Daily closing prices for 4 stocks + KSE-100 index
- Period: January 1, 2019 – December 31, 2025 (7 years of data)
- Source: Pakistan Stock Exchange (PSX) historical data

### 2. Returns Calculation
```
Daily Return = (Price Today - Price Yesterday) / Price Yesterday
Annual Return = Average Daily Return × 252 trading days
```

### 3. Risk Metrics
**Standard Deviation (Volatility):**
- Measures how much returns fluctuate day-to-day
- Higher SD = more unpredictable = riskier stock
- Used to annualize: Daily SD × √252

**Coefficient of Variation (CV):**
- Risk per unit of return (CV = Std Dev / Mean Return)
- Shows risk-adjusted performance
- Lower CV = better risk-adjusted returns

### 4. Beta Estimation (Regression Analysis)
```
Stock Return = α (Alpha) + β (Beta) × Market Return + Error
```

**Beta Interpretation:**
- **β = 1.0** → Stock moves exactly with market
- **β > 1.0** → More volatile than market (aggressive)
- **β < 1.0** → Less volatile than market (defensive)
- **β ≈ 0** → Stock moves independently of market (low systematic risk)

**Alpha Interpretation:**
- Positive α = Stock outperforms market on risk-adjusted basis
- Negative α = Stock underperforms market
- Shows manager's skill or stock-specific value

### 5. CAPM (Capital Asset Pricing Model)
```
Expected Return = Risk-Free Rate + β × (Market Return - Risk-Free Rate)
```

Used to determine if a stock is overvalued or undervalued using Security Market Line (SML).

### 6. Portfolio Construction
- Created portfolios with different weight combinations
- Analyzed efficient frontier (best risk-return combinations)
- Calculated portfolio return and portfolio risk
- Portfolio Return = Sum of (Weight × Stock Return)
- Portfolio Risk = SQRT(Weighted Sum of Variance-Covariance Matrix)

## 📁 File Structure
```
FM_Assignment3_Fixed.xlsx
├── Cover
│   └── Assignment details, company list, time period, risk-free rate
├── Raw Price Data
│   └── Daily closing prices for OGDC, LUCK, HBL, ENGRO, KSE-100
├── Daily Returns
│   └── Calculated daily returns for all stocks and index
├── Summary Statistics
│   └── Mean return, std dev, CV, min/max returns for each stock
├── Beta & Regression
│   └── Beta, Alpha, Correlation, R² from regression analysis
├── Portfolio Analysis
│   └── Different portfolio combinations and their risk-return profiles
└── SML & Valuation
    └── Security Market Line and stock valuation results
```

##  Learning Outcomes

This project demonstrates mastery of:
- Portfolio diversification and Modern Portfolio Theory (MPT)
- Capital Asset Pricing Model (CAPM) and Security Market Line (SML)
- Beta coefficient calculation and interpretation
- Risk-return optimization
- Statistical analysis (correlation, regression, std dev)
- Financial modeling using Excel advanced formulas
- Real-world application to Pakistani stock market

##  Technical Skills Applied

| Skill | Application |
|-------|-------------|
| **Statistical Analysis** | Mean, standard deviation, correlation, regression |
| **Financial Modeling** | CAPM, portfolio theory, risk-return analysis |
| **Regression Analysis** | Slope/Intercept calculation for Beta/Alpha |
| **Excel Functions** | SLOPE(), INTERCEPT(), STDEV(), CORREL(), AVERAGE() |
| **Data Analysis** | 7 years × 252 trading days = 1,764 data points analyzed |
| **Critical Thinking** | Why do stocks behave independently? When to diversify? |

##  Companies Analyzed

| Stock | Sector | Beta | Annual Return | Annual Risk | R² | Interpretation |
|-------|--------|------|---------------|-------------|-----|-----------------|
| OGDC | Oil & Gas | 0.002 | -1.77% | 22.05% | 0.0000016 | Defensive, negative returns |
| LUCK | Cement | -0.092 | 23.04% | 28.19% | 0.0034 | Best performer, high risk |
| HBL | Banking | -0.009 | 4.35% | 24.68% | 0.000042 | Stable, modest returns |
| ENGRO | Chemicals | 0.005 | -1.23% | 30.26% | 0.0000085 | Highest risk, negative returns |
| KSE-100 | Index | — | 6.81% | 17.82% | — | Market baseline |

##  Future Improvements & Automation

- **Python Implementation:** Automate using pandas, numpy, scikit-learn
- **Real-time Data:** Connect to PSX API for live stock prices
- **Dashboard:** Build interactive Plotly/Dash visualization
- **Monte Carlo:** Simulate portfolio returns over 1-5 year horizon
- **Time Series Forecasting:** ARIMA/GARCH models for return prediction
- **Optimization:** Maximize Sharpe ratio for optimal portfolio weights
- **Risk Management:** Value-at-Risk (VaR), Conditional VaR calculations

##  Key Insights

1. **Low Systematic Risk:** All stocks have near-zero beta, meaning KSE-100 movements don't drive their prices. Stock-specific factors dominate.

2. **Risk ≠ Return:** ENGRO has highest risk (30.26%) but lowest return (-1.23%). LUCK has high risk (28.19%) but high return (23.04%). Risk doesn't always reward.

3. **Diversification Value:** Low/negative correlations between stocks = excellent diversification candidates. Portfolio risk can be lower than individual stock risk.

4. **Market Disconnect:** These 4 stocks behave independently from the broader KSE-100 index. May indicate sector-specific headwinds or stock-specific opportunities.

5. **Volatility Clustering:** Standard deviation ranges from 22% to 30% annually — all significantly riskier than market (17.82%).

##  Concepts Applied

- **Capital Asset Pricing Model (CAPM)** — Determining required returns
- **Modern Portfolio Theory (MPT)** — Building efficient portfolios
- **Beta & Systematic Risk** — Market-related risk measurement
- **Security Market Line (SML)** — Valuation framework
- **Diversification** — Reducing risk through correlation analysis
- **Risk-Return Tradeoff** — Investor preference curves
- **Regression Analysis** — Estimating beta coefficients

##  About This Project

Created as part of **Financial Management coursework** at COMSATS University Islamabad.

**Author:** Daniyal Nadeem  
**Course:** Financial Management (BBD-IV)  
**Institution:** COMSATS University Islamabad  
**Submission Date:** April 11, 2026  
**Data Period:** January 1, 2019 – December 31, 2025

---

## 📞 Contact & Next Steps

💡 Open to **internship opportunities** in:
- Data Analysis
- Financial Analysis
- Business Intelligence
- Quantitative Finance

📧 Email: daniyalndm.professional@gmail.com  
🔗 LinkedIn: [linkedin.com/in/daniyal-nadeem](https://www.linkedin.com/in/daniyal-nadeem-95687128b/)

---

*This analysis demonstrates practical application of financial theory to real-world asset allocation decisions.*
