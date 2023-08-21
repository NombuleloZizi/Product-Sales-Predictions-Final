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


- The Final Model Chosen was a `Random Forest Regressor Model` with the n_estimators tuned to 60.
- For the testing set on the model, `60.02%` of the variance in y was explained by x. 
- The Mean Absolute Error was off by about `$728.683`.
- The Mean Squared Error was `$1,097,379.432`.
- The Root Mean Squared Error had a calculation of `$1,074.559`.

Using this model to help the retailer understand the properties of products and outlets that play crucial roles in predicting sales. Considering the previous regression metrics from how the model performed, there is a disparity between the R^2 score and also the Root Mean Squared Error that cannot be ignored.

## Recommendations

Sales Predictions

- For those who are interest based on Item type:
  - Fruits and vegatables appears more than  other item types.
    
- For those who are interest based on outlet type:
  - Suppermarket Type1 is the most outlet type.
  
- For those who are interest based on location type:
  - Tier 3 is the most location type.
  

Model Performance
- Overall, the best model is definitely the tuned Random Forest Regressor Model. 


## Limitations & Next Steps

We only used a few visuals, we could add more to have more insight about the prediction of the sales.. 

## For further information
- For any additional questions, please contact **Nombulelo Zizi**: zizinombu@gmail.com

