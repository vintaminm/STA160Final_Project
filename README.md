# STA160Final_Project
**Note:** The LSTM analysis section is implemented in Python and is provided as a separate Python file (`LuxuryLSTM.py`). The ARIMAX portion and other analyses are conducted in R.

# The Impact of Economic Indicators on Luxury Market Growth

This project investigates how various economic indicators influence the growth of the luxury market over time. By using an ARIMAX (Autoregressive Integrated Moving Average with Exogenous Variables) model, we aim to forecast luxury market growth and understand which factors have the strongest predictive power.

## Overview

- **Objective:** Identify key economic indicators that drive luxury market growth and produce a forecast for a future year.
- **Approach:** Use time series analysis combined with external indicators to fit and evaluate ARIMAX models.
- **Output:** A final PDF report that details the analysis steps, visualizations, and model performance metrics.

## Data

- **File:** `merged_luxury_indicators.csv`
- **Description:** This file contains annual luxury market growth data along with various economic indicators, such as GDP growth, income growth, Gini changes, and others.  
- **Variables:**  
  - **Year:** The calendar year of the observation.  
  - **Growth_Rate:** The luxury market growth rate (%) for that year.  
  - **GDP.Growth.Rate:** GDP growth rate (%) for the same year.  
  - **Gini.Change.Rate:** The change in the Gini coefficient, representing income inequality shifts.  
  - **Consumer.Sentiment.Growth.Rate:** Measures changes in consumer sentiment.  
  - **Income.Growth.Rate, Top.1..Growth.Rate, Top.10..Growth.Rate, Bottom.50..Growth.Rate:** Growth rates for various income segments.  
- **Source:** Luxury Earnings Data for Ten Brands, University of Michigan Consumer Confidence Index, FRED, WORLD INEQUALITY DATABASE.

## Requirements

- **R version:** Tested with R 4.0.0+  
- **Packages:**  
  - `tidyverse` (for data manipulation and plotting)  
  - `corrplot` (for correlation matrix visualization)  
  - `forecast` (for ARIMA/ARIMAX modeling)  
  - `lmtest` (for residual diagnostic tests)  
  - `changepoint`, `zoo`, `tseries`, `xts` (for additional time series handling and tests)

You can install missing packages in R using:
```r
install.packages(c("tidyverse", "corrplot", "forecast", "lmtest", "changepoint", "zoo", "tseries", "xts"))
```

