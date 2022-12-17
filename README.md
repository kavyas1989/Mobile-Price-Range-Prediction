# Mobile-Price-Range-Prediction

## Problem Description

In this Digital world where everything from our mode of communication to way if transporatation and food has been happening with the help of our tehcnologies which has caused the rising demand for mobile phones and it led to many companies engaging in market of mobile phone and in this age of capitalism the competition has become very fiernce and profit margin has become very low in the market.Therefore, there is a need to understand mindset and buying pattern of customers which led to making and recommending most appropriate choice for every users . 
Therefor,it is very important to understand the relation between the characteristics of the mobile phone and it’s selling price and classifying into different group (like very high ,High , Low categories) as price will be biggest factor affecting demand of mobule phone.This will help the companies to decide the appropriate price for their product.So ,this project aims to identify the important features which influence the price of the phone and find the best Classification model which predicts the price range of the phone based on it’s characteristics

## Data Description 

- Total number of rows in data : 8760
- Total number of columns : 14
The features given in the dataset are:
- Battery_power : Total energy a battery that can be stored in one time measured in MAh.
- Bluetooth : Has bluetooth or not.
- Clock_speed : speed at which microprocessor executes instructions.
- Dual_sim : Has dual sim support or not.
- Fc - Front : Camera megapixels.
- four_g : Has 4G or not.
- int_memory : Internal Memory in Gigabytes
- m_dep : Mobile Depth in cm
- mobile_wt : Weight of mobile phone
- n_cores : Number of cores of processor
- pc : Primary Camera mega pixels
- px_height : Pixel Resolution Height
- px_width : Pixel Resolution Width
- RAM : Random Access Memory in Mega Bytes
- sc_h : Screen Height of mobile in cm
- sc_w : Screen Width of mobile in cm
- talk_time : longest time that a single battery charge will last when you are
- three_g : Has 3G or not
- touch_screen : Has touch screen or not
- wifi : Has wifi or not
- price_range : This is the target variable with values of 0(low cost), 1(medium cost), 2(high cost) and 3(very high cost).

## Data Cleaning and Feature Engineering

### (1) Removing Null Duplicate Rows
- No duplicate and Null row sample were present in dataset.

### (2) Outliers Treatment
- There is no outlier in our dataset and our target class us also very balanced.

### (3) Feature Selection and Extraction
- There is very high multicolinearity in our independent features of dataset ,so we used Tree based Feature Selection Technique also known as Extra Tree Classifier and selected most important top 15 Features.

## EDA

To gain insights from the data. We are going to plot various charts like bar graph, histogram, heat map, line graph etc. efor univariate and bivariate analysis. This process helped us figuring out various aspects and relationships among the dependent and the independent variables.
Observation of our EDA as follows:

- Our dependent variable of Price Range of mobile balance is very balanced .
- Most of the phones currently available in the market have 3G support and 4G supported devices are also slightly have more existence in market than without 4G devices .
- Relatively expensive phones have more RAM and higher capacity batteries.
- Expensive mobile phone’s pixel width and picel height is also more.
- Most of the phones do not contain front camera or have low quality front cameras.
- Most expensive phones are light-weight and have wider screens as compared to phones belonging to lower price ranges.

##  Model Building

In this clssification problem statement of predicting mobile phone price based on its features, we need to classify our input data into 4 price based categories (like Low, Medium, High, and Very High) and we are going to use following classification algorithm for it :-

- Naive Bayes.
- Decision Tree.
- Random Forest.
- KNN
- Logistic Regression.
- XG Boost

## Evaluation Metrics 

To evaluate the models we should use metrics like F1 score
and we need to use the fact that higher the value of F1 score then better our model is. 

F1 score for all the Classification Algorithms on thier test data 

- Naive Bayes : F1 score = 0.82 
- Decision Tree : F1 score = 0.84
- Random Forest : F1 score = 0.84
- KNN : F1 score = 0.63
- logistic Regression : F1 score = 0.96
- XG boost : F1 score = 0.93 

## Conclusion 

From our evaluation metric F1 score values for different algorithms we have observed that we are getting our highest value of F1 score for Logistic Regression and XGBoosting. So we can use either of these 2 algorithms for model building  .
