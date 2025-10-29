# Fundamental Factor Analysis: Replicating "Fundamental Indexation"

### Project Overview
This notebook reproduces the empirical results of *Fundamental Indexation* (Arnott et al., 2005),  
which proposed constructing portfolios based on fundamental measures instead of market capitalization.  
The analysis is extended with out-of-sample performance tests covering 2005–2024 to examine the persistence of the strategy.

### Methodology
1. Replicate Table 1 and Table 2 from the original paper using CRSP and Fama-French datasets.  
2. Construct both market-cap-weighted and fundamental-weighted portfolios.  
3. Compute monthly and annualized returns, volatility, Sharpe ratios, and CAPM/Fama-French 3-Factor alphas.  
4. Conduct both in-sample (1962–2004) and out-of-sample (2005–2024) analyses.

### Key Findings
- Fundamental-weighted portfolios outperform market-cap portfolios during the in-sample period.  
- The performance advantage decreases in the out-of-sample period, indicating potential factor crowding and diminishing returns.  
- Once SMB and HML factors are included in the Fama-French 3-Factor model, most of the CAPM alpha becomes statistically insignificant.  
- The results suggest that the observed excess returns are primarily explained by exposure to size and value factors rather than true alpha.

### Tools and Techniques
- Python: pandas, numpy, statsmodels  
- Finance concepts: CAPM, Fama-French 3-Factor model, portfolio return decomposition, alpha and beta estimation  
- Data sources: CRSP monthly stock returns, Fama-French Factors (via WRDS)

### References
Arnott, R. D., Hsu, J., & Moore, P. (2005). *Fundamental Indexation.* Financial Analysts Journal, 61(2), 83–99.
