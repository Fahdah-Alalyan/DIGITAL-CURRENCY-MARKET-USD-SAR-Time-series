# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: DIGITAL CURRENCY MARKET (USD & SAR) - Time series

##### Applying Unsupervised Learning Algorithms

----

### Problem Statement

Forecasting digital currency stock prices is a challenging task due to multiple inflluencing factors. Therefore, it is helpful to build base models for predicting future digital currency trends. Moreover, extracting hidden knowledge and gathering new information can enhance the base models.


### Goal
To predict the close price of digital currency stock market using three different TimeSeries models.

### Dataset
The used dataset describes daily historical time series for Bitcoin traded on the Saudi stock market. Prices and volumes are quoted in both the market-specific currency (SAR) and USD. Historical date range: 2018-05-11 to 30.01.2021.

### Data source
Kaggle dataset [DIGITAL CURRENCY MARKET](https://www.kaggle.com/ahmedadam415/digital-currency-time-series)

---
### Key findings
- Overall, some challenges are raised while discovering the dataset—one of which, the sudden increase of Close_SAR after July 2020. As a result, we have considered the dates before July 2020 for modelling to get a better prediction. The second challenge was that the RMSE errors were high because of the nature of the stock dataset.

- After applying the models below, The lowest RMSE error was achieved by predicting using the XGBoost model. On the other hand, The highest RMSE error was achieved by forecasting using the XGBoost model.

- Our findings highlight the difficulty of predicting or forecasting the stock market prices. A better prediction or forecasting might be achieved by having more features and complex models.




---
### Model Summary

|MODEL|MEAN|RMSE|
|:-|:-|:-|
|XGBoost-Prediction|35756.13|1452.98|
|FB Prophet|36019.09|2642.15|
|SARIMAX|27715.78|2970.51|
|XGBoost-Forecasting|35756.13|3245.03|

**key**
- Mean: the mean close pirce (SAR)
- RMSE: Root Mean Square Error

---
### Data dictionary

|Feature|Type|Dataset|Description|
|:-|:-|:-|:------------:|
|open_SAR|*float*|dc_|Opening price Saudi Riyal(SAR)|
|open_USD|*float*|dc_|Opening price (USD)|
|high_SAR|*float*|dc_|Highest stock price (SAR)|
|high_USD|*float*|dc_|Highest stock price (USD)|
|low_SAR|*float*|dc_|lowest stock price (SAR)|
|low_USD|*float*|dc_|lowest stock price (USD)|
|**close_SAR**|*float*|dc_|Market closing stock price (SAR)|
|close_USD|*float*|dc_|Market closing stock price (USD)|
|volume|*int*|dc_|Trading volume|

---
#### FOLDERS

 - **code**:
  - Contains the jupyter notebook detailing the models used to predict the stock price.
 - **data**:
  - contains all data files used in .csv format



---


**CONTRIBUTORS**

Fahdah Alalyan | Email: fahdah.a15@gmail.com

Amjaad Alsubaie | Email: amjaad_636@hotmail.com

Ahmed Adam | Email: am4ma@hotmail.com
