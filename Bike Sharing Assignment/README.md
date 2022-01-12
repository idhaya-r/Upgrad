# Bike Sharing
>    A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario.  BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19



## Table of Contents
* [Analysis approach](#analysis-approach)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Analysis Approach
- Business understanding : To evaluate the demand for the upcoming year based on the data provided.
- Data Understanding:  Understanding the data by exploring it and understanding its characterisitics.
- Data Cleaning and manipulation : Clean the data. Set the data to correct datatypes. 
- Data Quality : Checking the quality of data by checking the outliers in the continuous variables. 
    Mapping the categorical variables with numerical data to string data for better readability
- Exploratory data analysis:  To understand if there is any patterns and creating derived variables to understand the data better.
- Split the data : The data should be splitted into two dataframes for training and testing. Train part of the data is used to fit the model. Test part of the data should be used to predict the model and validate the assumptions
- Scale the data for training : If there is varying scale across the variables it would be difficult to interpret the coffecients at the end.So the model should have scaled data where the variable values lies in the same range. This can be done using minmaxscaler.
- Recursive Feature Elimination : Since we have close to 60+ columns, it wouldn't make sense to try out all the columns which might result in multicolinearity.To avoid such cases let us go through RFE to select the features which is of significance and then test it out iteratively in our linear model
- Model Selection : Run the models with varying set of parameters to understand its impact and use VIF to understand the inflation factor and remove the variables with high inflation factor and low significance.
- Evaluating features: Make sure that the features are not highly  correlated with each other.
- Residual Analysis:  Analyzing the error terms on both train and test data, to ensure the assumptions of linear regression.
- Model evaluation :  Evaluating the model by comparision of predicted vs actual.
    Calculate the mean squared error and r2score of the model selected.
- Caclculate metrics: Calculate metrics to understand whether the model is performing according to expectations.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Factors affecting the demand
     - atemp - Based on the feeling of temperature, the demand raises upto 46%
     - YEAR_2019 - Year on Year the business improvement is around 23%
     - There is a constant baseline demand of around 20% from the average.
     - These three factors contribute to around 89% percent of demand and thus help in predicting the demand.
- Recommendations to business
    - Year on Year , the business is in the upward trend, so no problem with business growth post pandemic.
    - Downtime and busytime can be predicted based on the weather. Business can use the downtime for maintence, during busy time they can look for ways to expand the supply.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy
- pandas
- seaborn
- matplotlib.plot
- sklearn.model_selection
- sklearn.pre_processing
- sklearn.feature_selection
- sklearn.linear_model
- statsmodels.api
- statsmodels.stats.outliers_influence
- sklearn.metrics
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@idhaya-r] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
