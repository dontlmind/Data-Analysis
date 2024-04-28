<a name="readme-top"></a>
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#data-source">Data Source</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#result">Result</a>
    </li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
This project serves as a demonstration of the application of the ARIMA model in forecasting the S&P 500 index.

The S&P500 includes 500 large companies listed on stock exchanges in the United States,
which people believe is a well-diversified portfolio that indices how the stock market moves
and reflects the economic situation for investors. This project mainly focuses on analyzing this
time series, constructing appropriate models that capture trend the most, using this
model to forecast 10 future periods, and use spectral analysis to find the first three
predominant periods.


### Data Source
The dataset used in this study is from FRED:
<a href="https://fred.stlouisfed.org/series/SP500"> data source </a>

### Built With

![Language](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)  
![Language](https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)  


<!-- RESULT -->
## Result

The study modeled the trend of S&P500 from Jan 2012 to Mar 2020 using time series
analysis. Two models were proposed, and it appears that both ARIMA(7,1,2) and ARIMA(6,1,2)
model fit the data well and satisfied all the model’s assumptions, based on model selection
criteria, ARIMA(6,1,2) was selected.
As a result, this model predicts for the next 10 periods, the S&P500 will have a positive
trend that seems to lead the index upwards, but by considering the 95% confidence interval,
it is not promised to increase in value in the next 10 periods.
The study also uses periodogram analysis to identify the first three predominant periods, as
shown in the periodogram, the three predominant periods are (3.33, 10, 1.4286). However,
the 95% confidence interval are too wide to draw the conclusion of the significance of the
peak.
Yet, there are still some limitations of this study. The model only counts the stochastic
trend, but not the deterministic trend. Some outliers are not fixed, for example, the period
of the pandemic has caused the S&P500 a sudden drop around 34%. These unexpected events can
not be predicted, however they can change the trend by a lot.
percentage difference of 5.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

