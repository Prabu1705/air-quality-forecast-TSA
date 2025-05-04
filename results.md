### Theoretical Comparison: ARIMA vs Prophet

| Aspect                        | ARIMA                                              | Prophet                                            |
|------------------------------|----------------------------------------------------|----------------------------------------------------|
| **Model Type**               | Linear, statistical                                | Additive time series model                         |
| **Trend Modeling**           | Differencing (I in ARIMA) removes trend            | Automatically detects and models trend             |
| **Seasonality**              | Needs manual specification (SARIMA for seasonality)| Built-in, flexible seasonal components             |
| **Missing Data Handling**    | Struggles without imputation                       | Tolerates missing data                             |
| **Outliers**                 | Sensitive                                          | More robust                                        |
| **Interpretability**         | Requires domain expertise                          | Easy to interpret, intuitive parameters            |
| **Automation**               | Needs tuning (p,d,q manually or auto_arima)        | Mostly automatic                                   |
| **Forecast Horizon**         | Performs well in short-term                        | Good for medium to long-term with trends/seasonality |
| **Multivariate Support**     | Pure ARIMA is univariate                           | Prophet is also univariate                         |

---

### RMSE-Based Evaluation

From the comparison:

- **ARIMA outperforms Prophet** in:
  - `C6H6(GT)`
  - `NOx(GT)`
  - `PT08.S3(NOx)`
  - `PT08.S5(O3)`
  - `RH`

- **Prophet outperforms ARIMA** in:
  - `NMHC(GT)`
  - `PT08.S4(NO2)`

- **Both are within acceptable limits** for most variables.

---

### Result:

- **Accuracy-wise** (based on RMSE comparison), **ARIMA slightly edges out Prophet** for your dataset, especially for variables like `CO(GT)`, `T`, `AH`, and pollutants like `NOx(GT)`.

- **However**, if your data has:
  - strong seasonal trends,
  - irregular time intervals,
  - or lots of missing values,

  then **Prophet** might be the better **long-term** choice.

---
