# Time_series_forecast
🧭 Notebook Structure

This notebook follows a clear end-to-end workflow for time series forecasting and model comparison, using ARIMA, SARIMA, and Prophet models to predict inventory levels.

**1. Install Required Libraries**

Installs all the necessary dependencies, including pandas, matplotlib, statsmodels, and prophet.

**2. Load and Prepare the Data**

Imports the dataset, formats date columns, handles missing values, and sets the time index for proper chronological ordering.

**3. Exploratory Data Analysis (EDA)**

Analyzes data distribution, trends, and seasonality. Includes visualizations of the historical inventory levels.

**4. Plot the Autocorrelation Function (ACF/PACF)**

Identifies lag relationships and helps determine the ARIMA/SARIMA parameter selection.

**5. Data Preprocessing**

Performs stationarity testing using the Augmented Dickey-Fuller (ADF) test and differencing if required to stabilize the series.

**6. ARIMA Model**

Builds and evaluates ARIMA models with different parameter combinations.
Includes metrics such as MAE, RMSE, MAPE, and R² for model performance comparison.

**7. SARIMA Model**

Extends ARIMA by incorporating seasonality components.
Performs hyperparameter tuning using AIC and compares results to ARIMA.

**8. Prophet Model**

Implements the Facebook Prophet model for more flexible trend and seasonality forecasting.
Evaluates performance with error metrics and includes visualizations:

Actual vs Predicted inventory

Scatter plot (Actual vs Forecasted)

Full 6-month forecast

Trend and seasonal decomposition plots

**9. Building the Most Optimum Model**

Trains the best-performing Prophet model on the full dataset for final deployment.

**10. Download the Model**

Saves the trained Prophet model as a .pkl file for integration with the Streamlit forecasting app.

**12. Conclusion and Insights**

Summarizes model performance, visual findings, and forecasting insights.
Highlights Prophet as the most accurate and interpretable model for long-term inventory forecasting.
