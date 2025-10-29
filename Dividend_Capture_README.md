# Dividend Capture Strategy: Empirical Analysis Using CRSP Data

### Project Overview
This notebook investigates the profitability and risk-adjusted performance of a dividend capture strategy using U.S. equity data from the CRSP database.  
The strategy examines whether buying stocks before the ex-dividend date and selling afterward generates abnormal returns after accounting for transaction costs and market risk.

### Methodology
1. Identify all dividend-paying stocks with valid ex-dividend and payment dates from the CRSP dataset.  
2. Construct a buy-at-close and sell-at-open trading strategy around the ex-dividend date.  
3. Compute returns net of bid-ask spreads and round-trip transaction costs.  
4. Compare performance with market benchmarks and risk-adjusted metrics such as Sharpe ratio and t-statistics.  
5. Evaluate the persistence of returns across market regimes and firm characteristics.

### Key Findings
- The dividend capture strategy yields positive raw returns but loses significance after adjusting for transaction costs.  
- There is no evidence of persistent abnormal returns after accounting for risk factors.  
- The observed returns are largely explained by short-term price adjustments and tax-related timing effects.  
- Overall, the results suggest that dividend capture opportunities are limited in efficient markets.

### Tools and Techniques
- Python: pandas, numpy, statsmodels  
- Finance concepts: ex-dividend pricing, risk-neutral valuation, abnormal return estimation  
- Data source: CRSP monthly and daily stock data (via WRDS)

### References
Michaely, R., & Vila, J.-L. (1996). *Trading volume with private valuation: Evidence from the ex-dividend day.* Review of Financial Studies, 9(2), 471–509.  
Graham, J. R., Michaely, R., & Roberts, M. R. (2003). *Do price discreteness and transactions costs affect stock returns? Comparing ex-dividend pricing before and after decimalization.* Journal of Finance, 58(6), 2611–2635.
