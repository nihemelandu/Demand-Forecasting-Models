<h1>Comparing Demand Forecasting Models</h1>

<h2>Overview</h2>
<p>In this project, we compare traditional demand forecasting techniques with machine learning models across a variety of datasets that exhibit different time series components: <strong>level</strong>, <strong>trend</strong>, <strong>seasonality</strong>, and <strong>cyclicality</strong>. The goal is to demonstrate which forecasting models perform best under different complexities of time series data. We focus on evaluating both classical methods (such as Exponential Smoothing) and modern machine learning models (such as XGBoost), assessing their ability to capture various data patterns and generate accurate forecasts for supply chain demand.</p>

<h2>Datasets</h2>
<p>The project uses three different datasets that represent time series data with different components:</p>

<ol>
  <li>
    <strong>Level Component:</strong><br>
    <strong>Source:</strong> Australian Bureau of Statistics, Consumer Price Index, Australia (September 2020)<br>
    <a href="https://www.abs.gov.au/statistics/economy/price-indexes-and-inflation/consumer-price-index-australia/sep-2020#data-download" target="_blank">Consumer Price Index, Australia September 2020</a><br>
    This dataset represents time series with a level component, i.e., a series where the data points fluctuate around a constant value over time.
  </li>
  <li>
    <strong>Trend Component:</strong><br>
    <strong>Source:</strong> Australian Bureau of Statistics, National Accounts, Australia (September 2020)<br>
    <a href="https://www.abs.gov.au/statistics/economy/national-accounts/australian-national-accounts-national-income-expenditure-and-product/latest-release#data-download" target="_blank">National Accounts, Australia September 2020</a><br>
    This dataset exhibits a trend component, i.e., a dataset where values increase or decrease over time in a consistent manner.
  </li>
  <li>
    <strong>Seasonality Component:</strong><br>
    <strong>Source:</strong> Coursera Time Series for Business Forecasting<br>
    This dataset shows a clear seasonal pattern, with data points showing regular up-and-down movements at consistent intervals (e.g., yearly, monthly).
  </li>
  <li>
    <strong>Cyclicality Component:</strong><br>
    While no specific external dataset is used, the analysis considers time series with cyclic fluctuations (irregular cycles not necessarily linked to seasons).
  </li>
</ol>

<h2>Models Compared</h2>
<p>We compare two groups of forecasting models: <strong>Traditional Demand Forecasting Models</strong> and <strong>Machine Learning Models</strong>.</p>

<h3>Traditional Demand Forecasting Models (Supply Chain Context):</h3>
<ul>
  <li><strong>Exponential Smoothing (Holt-Winters):</strong> A widely-used method in the supply chain industry for forecasting demand. It’s well-suited for data with trend and seasonality, applying weighted averages of past observations to make forecasts.</li>
  <li><strong>Simple Moving Average (SMA):</strong> A basic method of forecasting that calculates the average of a fixed number of past periods. While simple, it’s still widely used in many supply chain contexts.</li>
  <li><strong>Naive Forecasting:</strong> A simple baseline method where future demand is assumed to be the same as the most recent observation. Often used for benchmarking more complex models.</li>
</ul>

<h3>Machine Learning Models:</h3>
<ul>
  <li><strong>XGBoost (Extreme Gradient Boosting):</strong> A machine learning model that is well-suited to time series forecasting due to its ability to capture non-linear relationships and complex patterns.</li>
  <li><strong>Random Forest:</strong> Another ensemble learning model that uses multiple decision trees, combining them for improved forecasting accuracy.</li>
  <li><strong>LSTM (Long Short-Term Memory):</strong> A type of recurrent neural network (RNN) designed to capture long-term dependencies in sequential data, making it a powerful tool for time series forecasting.</li>
</ul>

<h2>Objective</h2>
<p>The goal of this project is to explore which forecasting models perform best depending on the characteristics of the time series data. The models are evaluated based on accuracy metrics such as:</p>
<ul>
  <li><strong>Mean Absolute Error (MAE)</strong></li>
  <li><strong>Root Mean Squared Error (RMSE)</strong></li>
  <li><strong>Mean Absolute Percentage Error (MAPE)</strong></li>
</ul>
<p>The findings aim to provide insights into which models are most suitable for different problem complexities, helping supply chain professionals select the best tool for forecasting demand based on the type of time series data they are working with.</p>
