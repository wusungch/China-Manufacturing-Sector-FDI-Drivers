# Understanding the Decline of Taiwan’s FDI in China: Economic and Geopolitical Drivers Across Manufacturing Sectors

## Overview

This research project investigates the significant decline in Taiwan’s Foreign Direct Investment (FDI) in China from 2008 to 2023. The study focuses on identifying the economic and geopolitical factors driving this trend, with a sector-specific analysis of traditional and advanced manufacturing.

### Objective
- Primary Goal: Understand the relationship between Taiwan’s FDI in China and various economic/geopolitical factors.
- Sectoral Focus: Analyze differences in drivers for traditional and advanced manufacturing sectors.

### Key Findings
Significant Factors:
- Rising Southeast Asian GDP growth diverts investment from China in both sectors.
- China’s Housing Price Index (HPI) negatively impacts FDI due to increased labor and operational costs.
- Economic Policy Uncertainty (EPU) reduces Taiwanese investor confidence but has a modest effect size.
- Sectoral Insights:
- Traditional Manufacturing: Stronger ties to Taiwan’s domestic growth; sensitive to operational cost changes.
- Advanced Manufacturing: More vulnerable to regional competition; higher sensitivity to economic shifts in Southeast Asia.

### Dataset
- Time Frame: Monthly data from January 2008 to December 2023.

Sources:
- Taiwan’s Ministry of Economic Affairs (FDI Data)
- Caldara & Iacoviello (2018) – Geopolitical Risk Index (GPR)
- Baker, Bloom & Davis (2016) – Economic Policy Uncertainty Index (EPU)
- CEIC and National Bureau of Statistics of China – GDP and HPI data
- Investing.com – CNY:TWD Exchange Rates

## Methodology

### Preprocessing
- Aggregated monthly Approved Outward Investment (AOI) for traditional and advanced sectors.
- Incorporated lagged predictors to capture delayed effects:
- GPR Index: Lagged by 1 month.
- EPU Index: Lagged by 6 months.
- GDP and HPI: Lagged by 1 year.
- Addressed potential multicollinearity and heteroscedasticity using Variance Inflation Factors (VIF) and robust standard errors.

### Analysis
Models Used
- Time-series regression models for combined and sector-specific data.

Key Predictors:
- Economic indicators: Southeast Asia GDP growth, Taiwan GDP growth.
- Geopolitical factors: GPR and EPU Index.
- Cost factors: China’s HPI, exchange rate volatility.

### Evaluation
- Robustness checks conducted with alternative lag structures (6 and 12 months).
- Assessed model assumptions (stationarity, autocorrelation, and residual normality).

## Results
- Combined Model R²: 27.9% of FDI variation explained.
- Sectoral Model R²: 29.0% (Traditional) and 21.0% (Advanced).
- Significant Predictors:
- Southeast Asia GDP growth: Strong negative effect on FDI.
- China’s HPI: Negative effect across sectors.
- EPU Index: Modest negative effect in the combined model.

## Limitations
- Sample Size: 192 observations per sector.
- Omitted Variables: No direct measure for labor costs, a key FDI driver.
- External Validity: Results specific to Taiwan-China dynamics and manufacturing sectors.
