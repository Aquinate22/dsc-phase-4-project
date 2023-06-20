
# Time Series Analysis on Real estate

Time series analysis is a statistical technique used to analyze and model data points collected over time. In this project we will use time series analysis on real estate data to forecast the top 5 cities for Talanta Ltd.


## Stakeholders

This project is to be used by:

- Talanta LTD


## Authors

- [@Ann Gitonga](https://github.com/anngitonga)

- [@Mitchelle Okubasu](https://github.com/Aquinate22)

- [@Pascal Okuda](https://github.com/okudapascal)

## Lessons Learned



Forecasting future values using historical data

Understanding trends and patterns

Modeling using ARIMA

Model evaluation
## Project Overview

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/5f7e45f6-098b-4724-be55-49ce39eb1a27)


## Understanding Real Estate

Real estate is considered real property that includes land and anything permanently attached to it or built on it, whether natural or man-made. There are five main categories of real estate which include residential, commercial, industrial, raw land, and special use. Investing in real estate includes purchasing a home, rental property, or land.
Real estate is also dramatically affected by its location and factors such as employment rates, the local economy, crime rates, transportation facilities, school quality, municipal services, and property taxes can affect the value of the real estate.
## Business Understanding   
 Some of the responsibilities of Talanta Ltd include:
 

*  To provide guidance and assistance to sellers and buyers in marketing and purchasing property for the right price under the best terms.
*  To determine clients’ needs and financial abilities to propose solutions that suit them.
*  To perform comparative market analysis to estimate properties’ value

## Objectives
*  To develop a time series model that would predict the top 5 zip codes to invest in.

*  To come up with recommendations for the top 5 zip codes for Talanta Ltd

## Data Understanding
 
 The data had rows and 272 columns in wide format
 The dates on the columns are in int64 data type

 The data was then transformed from wide to long format using **pd.melt()**.
 The date column was set as index. 

 ![datahead](https://github.com/Aquinate22/Phase-3-Project-SyriaTel-Customer-Churn/assets/121969694/dae406f2-e25e-4424-9a2d-5b39e8a4eb54)
 wide format

 ![new format](https://github.com/Aquinate22/Phase-3-Project-SyriaTel-Customer-Churn/assets/121969694/2cf3b688-afb0-4219-b259-089af3095e10)
long format with date as index
## EDA


![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/4a5f1f04-0c4b-4755-8fac-42a8254e5edb)
New York is the most popular city according to the data followed by Los Angeles.

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/6b46a0cb-df3a-44d8-8109-3aaedb921d65)
Los Angeles was the most popular county followed by Jefferson 

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/475440de-2ed3-4538-aae6-f853d1bd3e39)
There was a drop in house prices in the year 2008 

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/b8192af4-73f8-4a98-b9fa-9d3b9efb5996)
Looking at housing prices for a selected zipcodes

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/fa157561-d52f-4ea2-98f0-b0f87dbb4dc5)



## Model Selection
**ARIMA Model**  
Splitting of the data into train and test sets.

Finding the best parameters for ARIMA model (p,d,q) by calculatng AIC .

Fitting the model using the parameters

**Results and Prediction**

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/4cd3868d-97fb-4645-b827-4b9f193673c5)

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/3d2f042a-bcb6-4315-b926-ab8d0fd415af)







## Interpreting Results

### Return On Investment
 
 Calculated the ROI on the data 
 ![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/6adb24cd-aea0-4cab-aca7-f21caa9baa49)

When ROI calculations yield a positive figure, it means that net returns are in the black (because total returns exceed total costs). But when ROI calculations yield a negative figure, it means that the net return is in the red because total costs exceed total returns.

### Some Zipcodes forecasts

![image](https://github.com/Aquinate22/dsc-project-phase-4/assets/121969694/8c0f999f-8d53-4065-851f-75ce85f58169)
