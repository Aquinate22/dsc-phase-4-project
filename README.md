# dsc-phase-4-project
This is a collaborative project on time series
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

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/fa5aeea2-55ed-4053-b60c-e0b06a1151e6)




## Understanding Real Estate

Real estate is considered real property that includes land and anything permanently attached to it or built on it, whether natural or man-made. There are five main categories of real estate which include residential, commercial, industrial, raw land, and special use. Investing in real estate includes purchasing a home, rental property, or land.
Real estate is also dramatically affected by its location and factors such as employment rates, the local economy, crime rates, transportation facilities, school quality, municipal services, and property taxes can affect the value of the real estate.
## Factors to consider before investing in real estate

*   Location
*   Market growth 
*   Property demand
*   Developmnent and Regeneration
*   Future Potential

In this project our main focus will be on the Location factor as it is concerned with zipcodes
## Business Understanding   
 Some of the responsibilities of Talanta Ltd include:
 

*  To provide guidance and assistance to sellers and buyers in marketing and purchasing property for the right price under the best terms.
*  To determine clients’ needs and financial abilities to propose solutions that suit them.
*  To perform comparative market analysis to estimate properties’ value

## Objectives
*  To develop a time series model that would predict the top 5 zip codes to invest in.

*  To come up with recommendations for the top 5 zip codes for Talanta Ltd

## Data Understanding
 
 The data had 14723 rows and 272 columns in wide format
 The dates on the columns are in int64 data type

 The data was then transformed from wide to long format using **pd.melt()**.
 The date column was set as index. 

![before](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/d52cea4d-9ae0-4099-8dc3-4ea398117345)
 wide format

![after](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/e2a9406e-1d89-41b2-8285-37ab3c2ab423)

long format 
## EDA

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/4ae8e5cf-cd68-40f0-9510-8874d1a764ef)
New York is the most popular city according to the data followed by Los Angeles.

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/06ab5b4b-91bb-4f6d-8916-ddd73a1bfd6c)
Los Angeles was the most popular county followed by Jefferson 


![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/668261f3-8a2b-4824-96a2-83009e1c89cb)
Most popular state is CA


![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/6cd5052e-dff4-4f14-b664-80198d066d00)
There was a drop from 2008

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/6d62b250-145e-4118-bf00-ec35bfdc22f8)
Housing prices of selected zip codes




## Model Selection
**ARIMA Model**  
Splitting of the data into train and test sets.

Finding the best parameters for ARIMA model (p,d,q) by calculatng AIC .

Fitting the model using the parameters

**Results and Prediction**

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/b1997d66-1a74-40fb-a45d-3828d766fa49)

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/76bdae8a-03aa-44b6-9cef-c2233529992b)








## Interpreting Results

### Return On Investment
 
 Calculated the ROI on the data 
 ![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/92f612cc-e518-4557-9980-684adfa8faaa)


When ROI calculations yield a positive figure, it means that net returns are in the black (because total returns exceed total costs). But when ROI calculations yield a negative figure, it means that the net return is in the red because total costs exceed total returns.

### Some Zipcodes forecasts
![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/ecc00bfa-cbd1-4c47-b973-00c40a108be5)



## Top 5 zip codes

![image](https://github.com/Aquinate22/dsc-phase-4-project/assets/121969694/5d1faa56-5009-4367-af38-35bd3951669f)

## Recommendations

From the above analysis of the time series,  we can see that the top 5 zip codes to be recommended for the client are:

*  10305

*  44264

*  28726

*  3766 

*  28658 
This zip codes will reward high return on investment should one put the resources in them.
