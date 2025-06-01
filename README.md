# Applied_Forecasting_Methods

**Abstract**—This report presents a simple and clear analysis of
temperature data for Delhi using time series methods. The study
focuses on finding unusual temperature values (outliers), checking
the shape of data (kurtosis and skewness), observing warming
trends, removing seasonal effects using different methods, and
using the SARIMA model for forecasting. The data was analyzed
using Jupyter Notebooks and showed that Delhi is getting warmer
over time. Several techniques such as moving average, seasonal
decomposition, and differencing were used to better understand
the data. The SARIMA model was then used to predict future
temperatures. Deep Learning models were implemented to improve the prediction.

**Index Terms**—Time Series Analysis, Outliers, Skewness,
Warming Trend, Deseasonalization, SARIMA Model, Deep
Learning, LSTM, RNN, GRU

**INTRODUCTION**
Understanding temperature changes is important to monitor
the climate and plan for the future. This report explains how
we studied monthly temperature data of Delhi using time
series analysis. We used simple tools and methods to look at
how temperatures have changed and to predict how they might
change in the future.

**DATA INTERPRETATION**
We have specifically used data for Delhi, India, only to
analyze the surface temperature of a specific region. The range
of average monthly temperature data is dated from January
1950 to September 2013. The data set used in this project is
taken from kaggle

**Data format**
The dataset used in this study, titled GlobalLandTemperaturesByMajorCity.csv, contains long-term monthly average
land surface temperatures for major global cities, including
Delhi. Provided in CSVformat, the dataset comprises over
23,000 records and 7 columns. The key columns include
the observation date (dt), average temperature (AverageTemperature), uncertainty (AverageTemperatureUncertainty), city,
country, and geographical coordinates (Latitude and Longitude). The average temperature is recorded in degrees Celsius.

**Data Resolution and Granularity**
Temperature values are recorded at a monthly resolution,
allowing decadal and seasonal aggregation for trend analysis.

**Data cleaning and processing**
Rows with missing values or NaN values in Average MonthlyTemperature column were estimated using interpolation technique.

**Temporal coverage**
Although the dataset spans from 1743 to 2013, this study
focuses on the period from 1950 to 2013 due to improved
data quality and consistency. Data prior to 1950 contains
more missing values and higher uncertainty, reflecting limited
observational coverage. Starting from 1950 ensures a reliable
baseline and strengthens the validity of long-term trend analysis.

**CONCLUSION**
The study concluded a clear long-term warming trend from the
1980s onward, along with increased temperature variability.
Seasonal patterns remained consistent, with peak temperatures
in May–June and lows in December–January. Statistical measures like skewness and kurtosis provided deeper insights into
temperature distribution, highlighting the prevalence of warm
anomalies and changes in extreme events. Deseasonalization
techniques, such as seasonal decomposition and differencing, effectively removed cyclic patterns to expose underlying
trends. ARIMA and SARIMA models effectively captured
both seasonal and non-seasonal patterns in the data. Residual
diagnostics showed minimal autocorrelation and approximate
normality, confirming model adequacy. Among the two, the
SARIMA model demonstrated better performance with lower
forecasting error. Overall, the study demonstrated the value
of time series analysis in climate research and forecasting,
offering meaningful insights into Delhi’s changing climate and
showcasing robust methods to analyze long-term environmental trends.
However, despite their strengths, traditional statistical models like SARIMA face notable limitations in handling large
datasets and complex seasonal patterns particularly when
multiple seasonalities are present. This necessitates the exploration of deep learning models, which offer greater flexibility
and efficiency. Models like RNN, LSTM, and GRU leverage
sequential learning and internal memory to capture intricate
temporal dependencies and nonlinear relationships in the
data. Their implementation showed promising improvements
in predictive accuracy, especially when non-linear functions
and hidden layers were introduced. While baseline and linear models offered valuable benchmarks, the deep learning
models, even on modest datasets, outperformed them in terms
of error metrics like MAE. These findings reinforce the
growing importance of integrating deep learning approaches
in climate forecasting, particularly as the scale and complexity
of environmental data continue to increase.

**Dataset link** : https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data?select=GlobalLandTemperaturesByMajorCity.csv
