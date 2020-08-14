# COVID-19 Project Overview 
* Created a model to predict number of COVID-19 cases world-wide
* Optimized Support Vector Regression and Linear Regression models to reach best model.  

# Background 
Coronavirus (COVID-19) is a respiratory disease that originated in Wuhan, China in late 2019 and has since rapidly spread around the world, leading to a pandemic. Symptoms associated with COVID-19 can be mild to severe and may even result in death. Working hard to control the situation, worldwide governments are partnering with public health officials to mitigate and control the situation. 

Please visit cdc.gov for the most up to date information and to learn how to best protect yourself and your community. 

The dataset includes the number of confirmed, recovered, and death cases across the globe. 

# EDA 

I explored the death rate vs recovery rate globally. Please check out the code directly for more visualizations. 


# Model Building
Objective: predict the number of world-wide cases on any given day

First, I transformed the time series data by indicating that January 22, 2020 as "Day 0" and adding 1 for each additional day. Then, I split the data into training and test data (20%).  

I tried two different models and used the Mean Absolute Error to evaluate their performance. 

I tried:
* *Support Vector Regression*: baseline model
* *Polynomial Regression*: There is a strong relationship between days passed and number of total cases, thus, I thought a PLR would be effective. 


# Model Performance
* *Support Vector Regression*: MAE = 269349.07
* *Polynomial Regression*: MAE = 48479.86

![pr](https://i.postimg.cc/3wh0kGwX/PR.png)

![svm](https://i.postimg.cc/k5y6K5Vk/svm.png)

The polynomial regression model performed the best. 
