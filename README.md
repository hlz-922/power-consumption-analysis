# power-consumption-analysis

### Project description

Use Vector AutoRegression (VAR) model to forecast the power consumption

### Key steps

1. **Stationarity Check and Differencing**: The project involves a step where the stationarity of the dataset is confirmed, possibly using the Dickey-Fuller test. If the data were not stationary, a differencing approach would be applied to achieve stationarity, which is crucial for time series forecasting.
2. **Forecasting Problems**: The notebook outlines three forecasting scenarios:
    - Short-term forecasting (predicting 1 week ahead based on historical data).
    - Long-term forecasting (predicting 2 months ahead based on historical data).
    - Multi-step forecasting for 1 month, where each prediction is used as input for subsequent predictions.
3. **Prediction and Model Fitting**: It includes steps for creating predictions using the VAR model. For instance, one step involves creating an array **`prediction1`** that contains predictions for 7 values based on a test dataset.
4. **Multi-step Forecast Implementation**: The project describes implementing a multi-step forecast function, **`ms_forecast`**, which predicts multiple future observations in a sequence, using each prediction as input for the next.
