# Stock Portfolio Analysis — Pakistani Equities

## Project Overview

A comprehensive financial analysis of four major Pakistani stocks (OGDC, LUCK, HBL, ENGRO) against the KSE-100 benchmark index using capital asset pricing model (CAPM) and modern portfolio theory (MPT). Analysis covers seven years of historical data (January 2019 – December 2025) with 1,764 daily observations.

## Objective

To analyze and compare the risk-return characteristics of selected Pakistani equities, estimate systematic risk through beta coefficients, assess diversification potential via correlation analysis, and provide evidence-based insights for portfolio construction and asset allocation decisions.

## Dataset

Source: Pakistan Stock Exchange (PSX) historical data
Period: January 1, 2019 – December 31, 2025
Data Points: 1,764 daily observations
Companies: OGDC (Oil & Gas), LUCK (Cement), HBL (Banking), ENGRO (Chemicals)
Benchmark: KSE-100 Index
Risk-Free Rate: 11.35% (12-month T-Bill rate, 2026)

## Methodology

### 1. Data Collection and Cleaning

Daily closing prices were collected for all four stocks and the KSE-100 index. The dataset was validated for completeness and accuracy across the seven-year period.

### 2. Returns Calculation

Daily returns were calculated using the percentage change formula:

Daily Return = (Price(t) - Price(t-1)) / Price(t-1)

Annual returns were derived by multiplying average daily returns by 252 (the number of trading days in a year):

Annual Return = Average Daily Return × 252

### 3. Risk Metrics

Standard deviation was calculated to measure volatility, both on a daily and annualized basis:

Annual Volatility = Daily Standard Deviation × √252

Coefficient of Variation (CV) was computed to assess risk-adjusted performance:

CV = Standard Deviation / Expected Return

### 4. Beta Estimation via Regression Analysis

Linear regression was performed to estimate beta coefficients:

Stock Return = α (Alpha) + β (Beta) × Market Return + ε (Error)

Where:
- Beta measures systematic risk relative to the market
- Alpha represents risk-adjusted excess return
- The regression was performed using daily returns over the entire period

### 5. Correlation Analysis

Pearson correlation coefficients were calculated to measure the relationship between each stock and the KSE-100 index, providing insight into diversification benefits.

### 6. Portfolio Analysis

Different portfolio weight combinations were analyzed to evaluate risk-return tradeoffs and efficient frontier opportunities. Portfolio metrics were calculated as:

Portfolio Return = Σ (Weight × Stock Return)
Portfolio Risk = √(Weighted Variance-Covariance Matrix)

## Key Findings

### Return Analysis

LUCK Cement emerged as the best performer with an annual return of 23.04%, substantially outperforming the market average of 6.81%. HBL delivered modest but positive returns of 4.35%, while OGDC and ENGRO both recorded negative returns at -1.77% and -1.23% respectively.

### Risk Analysis

Annual volatility ranged from 17.82% (KSE-100) to 30.26% (ENGRO). All four stocks demonstrated higher individual volatility compared to the market index, a characteristic typical of single equities.

### Systematic Risk Assessment

All stocks exhibited near-zero beta coefficients (ranging from -0.0918 to 0.0049), indicating minimal systematic risk exposure. This suggests these stocks move independently of broader market movements, driven primarily by company-specific and sector-specific factors.

### Correlation with Market

Correlation coefficients remained close to zero for all stocks, with LUCK showing slight negative correlation (-0.0581) with the KSE-100 index. This low correlation indicates strong diversification potential when combining these stocks with market index positions.

### Risk-Adjusted Performance

The coefficient of variation analysis revealed LUCK (1.22) and KSE-100 (2.62) as the best risk-adjusted performers, followed by HBL (5.68). ENGRO (24.53) and OGDC (12.47) exhibited poor risk-adjusted returns.

## Analysis and Interpretation

### Daily Returns Over Time

The time series analysis of daily returns demonstrates significant volatility differences across the five assets. ENGRO and LUCK exhibit pronounced price fluctuations with daily swings exceeding 5%, while KSE-100 displays relatively stable movement patterns. This visual representation confirms the statistical volatility metrics.

### Annual Return Comparison

The return differential across stocks underscores the importance of stock selection. A 25-percentage-point spread separates the best performer (LUCK: 23.04%) from the worst performer (ENGRO: -1.23%), emphasizing that higher risk does not automatically guarantee proportional returns.

### Risk vs Return Tradeoff

The scatter plot analysis reveals three distinct regions: LUCK occupies the upper-right quadrant (high risk, high return), ENGRO occupies the lower-right quadrant (high risk, low return), and HBL remains in the middle ground (moderate risk, moderate return). This distribution illustrates the core principle of portfolio theory: investors must be compensated for accepting risk through proportionate returns.

### Risk-Adjusted Returns

When controlling for risk through coefficient of variation analysis, HBL and LUCK emerge as superior choices. HBL's 5.68 CV indicates reasonable returns for its risk level, while LUCK's 1.22 CV demonstrates exceptional return efficiency despite high volatility. ENGRO's 24.53 CV indicates excessive risk relative to negative returns, making it an unfavorable risk-return combination.

### Systematic Risk and Market Independence

The near-zero beta coefficients indicate that these stocks are driven by idiosyncratic rather than systematic risk factors. This finding is significant for portfolio construction: these assets do not amplify or dampen market movements, instead moving according to company-specific developments, sector dynamics, and regional economic factors.

### Diversification Potential

Low or negative correlation coefficients suggest strong diversification benefits. When combined with market index holdings or other Pakistani stocks, these assets can reduce overall portfolio volatility without proportionally reducing expected returns. LUCK's negative correlation is particularly valuable as a portfolio hedge.

## Technical Skills Demonstrated

- Statistical analysis (mean, standard deviation, correlation, regression)
- Financial modeling (CAPM framework, portfolio theory, risk metrics)
- Quantitative analysis (beta estimation, efficient frontier optimization)
- Time series analysis (daily return patterns, volatility clustering)
- Data visualization (multiple chart types, professional presentation)
- Business intelligence (translating quantitative results into actionable insights)

## Tools and Libraries

- Microsoft Excel (data organization, calculations, formulas)
- Advanced Excel functions (SLOPE, INTERCEPT, STDEV, CORREL)
- Python (data analysis, visualization, statistical modeling)
- Pandas (data manipulation and analysis)
- Matplotlib/Seaborn (professional chart creation)

## Data Structure

The analysis is organized across multiple worksheets:

- **Raw Price Data**: Daily closing prices for all five assets (1,825 rows)
- **Daily Returns**: Calculated daily returns for all five assets (1,825 rows)
- **Summary Statistics**: Descriptive statistics including mean, standard deviation, and coefficient of variation
- **Beta & Regression**: Beta coefficients, alpha values, correlation, and R-squared from regression analysis
- **Portfolio Analysis**: Various portfolio combinations and their risk-return profiles
- **SML & Valuation**: Security Market Line calculations and stock valuation results

## Visualizations

The analysis includes eight primary visualizations:

1. Daily Returns Over Time: Time series chart showing return patterns across all assets
2. Annual Return Comparison: Bar chart comparing total return performance
3. Annual Volatility Comparison: Bar chart comparing risk levels
4. Risk vs Return Scatter Plot: Efficient frontier representation
5. Coefficient of Variation: Risk-adjusted return comparison
6. Beta Comparison: Systematic risk by asset
7. Correlation with Market: Market sensitivity analysis
8. Regression Analysis: Individual scatter plots for each stock showing market relationship

## Key Insights and Conclusions

1. Risk and return are not perfectly correlated. Higher volatility does not guarantee higher returns (ENGRO example).

2. Market independence creates diversification value. Low systematic risk means these stocks behave differently from the broader market.

3. Risk-adjusted metrics are essential for decision-making. CV analysis reveals that LUCK delivers superior returns per unit of risk despite high absolute volatility.

4. Diversification reduces portfolio risk. The low correlation between stocks and the market suggests significant benefits to combining these assets in a diversified portfolio.

5. Stock selection matters significantly. The 25-percentage-point spread between best and worst performers demonstrates the impact of individual equity choices on portfolio outcomes.

## Applications and Use Cases

This analysis framework is applicable to:

- Portfolio construction and rebalancing
- Investment manager performance evaluation
- Risk assessment for institutional portfolios
- Educational demonstration of CAPM and MPT principles
- Market analysis for Pakistani equity markets
- Comparative asset allocation studies

## Limitations

The analysis assumes historical data is representative of future performance. Market conditions, regulatory changes, and company-specific developments may alter the relationships observed in this seven-year period. Beta coefficients and correlation values should be updated regularly as new data becomes available.

## Future Enhancements

Potential extensions to this analysis include:

- Implementation of dynamic beta estimation using rolling windows
- Factor analysis to identify specific drivers of stock performance
- Monte Carlo simulation for portfolio return forecasting
- Machine learning models for return prediction
- Integration of additional variables (earnings, macroeconomic indicators)
- Real-time data integration and automated reporting

## Contact and Information

Author: Daniyal Nadeem
Institution: COMSATS University Islamabad
Program: Business Data Analytics
Course: Financial Management (BBD-IV)
Analysis Date: April 2026
Data Period: January 1, 2019 – December 31, 2025

## Repository

All analysis files, including raw data, calculations, and visualizations, are available in this repository. The Excel file contains complete formulas and can be modified for alternative stock selections or time periods.

## Professional Application

This project demonstrates competency in:
- Applied financial theory
- Quantitative data analysis
- Professional visualization
- Business intelligence and reporting
- Statistical interpretation
- Risk management frameworks

This work is suitable for portfolio presentation to financial institutions, investment firms, and data analysis roles requiring demonstrated understanding of portfolio theory and quantitative methods.

---

*This analysis represents a comprehensive application of capital asset pricing model and modern portfolio theory to real-world market data, with particular relevance to Pakistani equity markets.*
