# GJR_vs_GARCH_USD-PEN
Comparison between GJR-GARCH(1,1) and GARCH(1,1) models for the USD/PEN exchange rate

## Overview
This code provides a short excercise that compares the fit of GJR-GARCH(1,1) and GARCH(1,1) models for the USD/PEN daily exchange rate. As seen with the Likelihood Ratio Test (LRT), the GJR-GARCH(1,1) provides a better fit. This is due to the leverage parameter included in this model, which accounts for asymmetric shocks. In this case, the  gamma coefficient (leverage parameter) shows a negative sings, indicating that a depreciation of the Peruvian Sol—reflected by a higher USD/PEN ratio—generates a larger impact on the volatility of returns. 

## Visualizations
This notebook also includes the following visualizations:

1. **Exchange Rate (`PX_LAST`)**: A time series plot showing the USD/PEN exchange rate over time.
2. **Log-Returns (`y_t`)**: A plot of the log-returns of the USD/PEN exchange rate.
    - **Clusters and Volatility**: The log-returns plot shows clusters of volatility over time. In financial series, periods of high volatility tend to be followed by more high volatility, which leads to the observed high-volatility clusters.
4. **Conditional Variance (`h_t`)**: A time series plot showing how the conditional variance changes over time.
5. **Volatility (`σ_t`)**: A time series plot of the square root of the conditional variance to illustrate the estimated volatility.
6. **Standardized Innovations (`η_t`)**:
   - **Time Series Plot**: Displays the standardized innovations over time.
   - **Histogram**: Visualizes the distribution of standardized innovations.
   - **Density Plot**: Compares the kernel density estimate of standardized innovations with the standard normal distribution.


