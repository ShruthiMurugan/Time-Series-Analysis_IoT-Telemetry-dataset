Trend analysis and forecasting on IoT telemetry data

IoT telemetry dataset description:(https://www.kaggle.com/datasets/garystafford/environmental-sensor-data-132k)
| Column   | Description          | Units      |
|----------|----------------------|------------|
| ts       | timestamp of event   | epoch      |
| device   | unique device name   | string     |
| co       | carbon monoxide      | ppm (%)    |
| humidity | humidity             | percentage |
| light    | light detected?      | boolean    |
| lpg      | liquid petroleum gas | ppm (%)    |
| motion   | motion detected?     | boolean    |
| smoke    | smoke                | ppm (%)    |
| temp     | temperature          | Fahrenheit |

Steps performed in time series analysis:

1.Data is loaded and preprocessed by removing missing values.

2.Date and time is set as the index of the dataframe.

3.Trend analysis is performed by fitting a polynomial trendline.

4.Seasonality analysis is done using seasonal decompose.

5.ARIMA model is used to forecast.

6.Metrics like mean absolute error and root mean squared error are computed.
