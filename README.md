<p align = "center"> 
  <img src = "https://datahack-prod.s3.ap-south-1.amazonaws.com/__sized__/contest_cover/bignart1-thumbnail-1200x1200.png">
</p>


# Sales Prediction

**Author**: Nombulelo Zizi

### Business problem:
Analyzing properties of products and outlets that play crucial roles in predicting sales
## Data Source: 
Sales Prediction
[https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

For this dataset, there were 607 rows and 12 columns.

## Data Dictionary

<p align = "center"> 
  <img src = "https://raw.githubusercontent.com/coding-dojo-data-science/Project1_Exemplar/main/DS%20Salaries%20Data%20Dictionary.png">
</p>


## To prepare this data, the data was cleaned, and the following processes were performed:
  - Dropped unwated columns
  - Most frequest value was used to populate missing values on categorical columns
  - Mean value was used to populate missing values on numeric columns

### Exploratory Data Analysis
    - During the exploratory data analysis, a boxplot and histogram was visualized for each numeric datatype column.. 
    - Also, a countplot, barplot and heatmap was visualized for each categorical column. 
    - This gave a good baseline for all of the numeric and categorical columns for univariate EDA.

<p align = "center"> 
  <img src = "https://github.com/NombuleloZizi/Product-Sales-Predictions-Final/blob/main/item%20outlet%20sales.png">
</p>

This graph shows the median is around 1800 for this particular column.


 ### Expanatory Data Analysis
    - To visualize the data for explantory purposes, three bargraphs were chosen and one linegraph was chosen.
    - The bargraphs were chosen to show how the categories compare to each other. 
    - Finally, a l.inegraph was chosen to show the trend of salaries over the past three years. 

<p align = "center"> 
  <img src = "https://github.com/NombuleloZizi/Product-Sales-Predictions-Final/blob/main/EDA%20item%20weight.png">
</p>

This graph shows the median is around 12.5 for this particular column.

## Explanatory Visuals

<p align = "center"> 
  <img src = "https://github.com/NombuleloZizi/Product-Sales-Predictions-Final/blob/main/item%20type.png">
</p>

 Here we can see that the top five Type that have the most items are as follows:
  - Fruits and Vegetables
  - Snack Foods
  - Household
  - Frozen Foods
  - Dairy

We can also see that the bottom five type that have the least of the items are as follows:
  - Seafood
  - Breakfast
  - Starchy Foods
  - Others  
  - Hard Drinks


<p align = "center"> 
  <img src = "https://github.com/NombuleloZizi/Product-Sales-Predictions-Final/blob/main/location%20type.png">
</p>

- This graph shows that most outlet location type is Tier 3 and the least outlet location type is Tier 1.

<p align = "center"> 
  <img src = "https://github.com/NombuleloZizi/Product-Sales-Predictions-Final/blob/main/outlet%20type.png">
</p>

This graph shows that most outlet type is Suppermarket Type1 and the least outlet type is Supermarket Type2.




 ### Maching Learning Using the Following Models:
    - Linear Regression Model
    - Decision Tree Regressor Model
    - Tuned Decision Tree Regressor Model
    - Random Forest Regressor Model
    - Tuned Random Forest Regressor Model
    
    
## Models Evaluated & Results

- Linear Regression Model (Testing Set):
  - MAE = 803.687
  - MSE = 1,187,857.066
  - RMSE = 1,089.889
  - R^2 = 0.569
    
- Decision Tree Regressor Model (Testing Set):
  - MAE = 1,039.842
  - MSE = 2,229,380.534
  - RMSE = 1,493.111
  - R^2 = 0.192
    
- Tuned Decision Tree Regressor Model (Testing Set):
  - MAE = 738.203
  - MSE = 1,118,036.621
  - RMSE = 1,057.373
  - R^2 = 0.595

- Random Forest Regressor Model (Testing Set):
  - MAE = 772.198
  - MSE = 1,228,760.100
  - RMSE = 1,108.495
  - R^2 = 0.555

- Tuned Random Forest Regressor Model (Testing Set):
 - MAE = 728.683
  - MSE = 1,097,379.432
  - RMSE = 1,047.559
  - R^2 = 0.602


- The Final Model Chosen was a `Random Forest Regressor Model` with the n_estimators tuned to 50.
- For the testing set on the model, `56.3%` of the variance in y was explained by x. 
- The Mean Absolute Error was off by about `$31,998.94`.
- The Mean Squared Error was `$2,044,264,641.83`.
- The Root Mean Squared Error had a calculation of `$45,213.55`.

Using this model to make predictions about the best places to live and which careers to choose to earn the most money would not be a very reliable. Considering the previous regression metrics from how the model performed, there is a disparity between the R^2 score and also the Root Mean Squared Error that cannot be ignored.

## Recommendations

Data Science Insights

- For those who have an interest in Data Science:
  - Data Analytics Leads & Principal Data Engineers earn the most amount of money. However, this are usually not entry level careers and I would recommend going through a program, like Coding Dojo, where you can earn your data science certificate and then map out your career to these positions.

  - Data Engineers & Data Scientists have the most 100% remote positions. So, if you are wanting to work from home, or work from anywhere in the world, choosing one of the top five remote positions would be a good choice to build your career upon.
  
  - Lastly, the trend for the last three years show that data science and related fields are increasingly earning more money each year. So, choosing a career in one of these fields can be very lucrative.

Model Performance
- Overall, the best model is definitely the tuned Random Forest Regressor Model. There was still some bias in the model, but by far it outperformed the linear regression model. 


## Limitations & Next Steps

From here, a student could use the insights from the visuals on how to tailor their path for their career. As mentioned before, Coding Dojo has a fantastic program that prepares inspiring data scientists for the field of data science. 

## For Further Information

For any additional questions, please contact: 
- Sherlin Whaley (Data Science Instructor)
- swhaley@codingdojo.com

