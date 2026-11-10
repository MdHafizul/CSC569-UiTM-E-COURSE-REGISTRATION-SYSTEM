# Technology Notes

## Outline of the technology explanation
- C1 Concepts: what machine learning and time series are; trend, seasonality and event effects; train and test split by time; error measures (MAE, RMSE, MAPE); the pipeline from data to forecast to scaling decision
- C2 Methods and tools: SARIMA, Prophet, LSTM, scikit-learn and statsmodels, cloud predictive autoscaling
- C3 Fit to the problem: benefits; limitations (data needs, sudden opening-minute spike, forecast error, privacy and cost, model drift); comparison with reactive autoscaling and fixed capacity

## Chosen technology
Machine learning: supervised time-series forecasting of concurrent users, used to decide when to scale cloud servers.

## Why this technology
The registration peak repeats every semester and starts on dates that UiTM announces in advance, so the load can be forecast from past traffic and the registration dates.

## Sources to read
1. Hyndman, R. J., & Athanasopoulos, G. (2021). Forecasting: Principles and practice (3rd ed.). OTexts.
2. Taylor, S. J., & Letham, B. (2018). Forecasting at scale. The American Statistician, 72(1), 37-45.
3. Gridin, I. (2022). Time series forecasting using deep learning. BPB Publications.