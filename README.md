# Food-Sales-Prediction

## Author:LiPing Liu


Business problem: Retailer planning requires sale prediction to allow them to budget their upcoming fiscal year with a reasonable margin of error. One of the key input for the prediction is sales volume. Sales rediction help corporation predict future revenue.

## Data Source

https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/#About


For this dataset, there were 8523 rows and 12 columns.





## To prepare this data, the data was cleaned and the following procsses were performed: 
### Exploratory Data Analysis



<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Exploratory%20.png" height="500" width="500" >

This histogram shows that Fruits and Vegetables and Snack Foods are the most popular item type for customers.

### Explanatory Data Analysis
- To visualize the date for explantory purpose, one scatterplot and two bargraphs are presented. 


<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Explanatory%201.png" height="500" width="600" >

This graph shows that When Retail price increaseing, item sales will increaseing also in supermarket type 3.

<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Explanatory%203.png" height="300" width="500" >


This graph shows that Tier 2 Location has the most sales compared to other Locations.

<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Explanatory%202.png" height="400" width="1000" >

This graph shows that regular fat items have higher item visibility, MRP and Sales.


### Maching Learning Using the Following Models:

- Linear Regression Model
- Decision Tree Regressor Model

## Models Evaluated & Results
- Linear Regression Model (Testing Set):
  - R^2 = -1.6575880497968222e+19
  - MAE = 558742259972.594
  - MSE = 4.5732477819291586e+25
  - RMSE = 6762579228318.999
- Decision Tree Regressor Model (Testing Set):
  - R^2: 0.23769742878875222
  - RMSE: 1450.2329055736004




## Recommendation

For the retailer:
To understand more about the sales, we obtained the information from data that item and outlet are both important rule to predict sales.
- Items
  - Fruits and Vegetables and Snack Foods are the most popular items. I would recommend retailer can either focus on generating more sales on these two types or planning to get more sale from other types by promoting.
  - Regular fat content items has higher items visibility, MRP and sale compare to low fat content, retailer can import more regular fat content item.
- Outlet
  - Outlet also play crucial roles in predicting sales.
  - Supermarket type 3 and location tier 2 performance the best sale among others, ratailers can consider to expand more on hot location and reduce to oepn or maintain the unpopular location in order to reduce the cost.

## Model Performance

Overall, the best model is definitely the tuned Decision Tree Regressor Model. There was still some bias in the model, but by far it outperformed than linear regression model.

## Project 1 Revisited - Part 1: Remaking, Saving, and Explaining Your Models
For this part of the project, we  will be producing a new version of your final project notebook using the updated tools in sklearn v1.1

## LinearRegression
- Fit and evaluate LinearRegresion model using dataframe X_train and X_test data.
- Extract and visualize the coefficients that the model determined.
- Select the top 3 most impactful features.
<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/coeffs.png" height="500" width="600" >

### Top 3 Most impactful features
From above coefficients graph, we know that these are the Top 3 Most impactful Features:
- Outlet Type Supermarket Type 3
    - Have the highest coefficients among features which that Type 3 Supermarket have more sales than others.
- Outlet Size High
    - Sales tend to be better in bigger size outlet.
- Outlet Type Supermarket Type 1
    - Type 1 Supermarket have better sales than Type 2 but not Type 3 which is has the highest coefficients.

## Tree-Based Model
- Fit and evaluate LinearRegresion model using dataframe X_train and X_test data.
- Extract and visualize the feature importances that the model determined.
- Identify the top 5 most important features.

<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/importances.png" height="400" width="600" >

### Top 5 most important features:
- Item MRP
    - Item Market Retail Price are the most important factor for Sales.
- Outlet Type Grocery Store
    - Grocery Store has better sales than other outlet types.
- Item Visibility
    - its important to have good visibility for selling items, better visibility more likely to engage with consumers and maximise sales.
- Outlet Type Supermarket Type3
    - People are likely to go to type 3, it could be the interior design/ style of the supermarket or size tend to have more people like to go there.
- Item Weight
    - Item Weights are matter so people could probably tend to do online delivery for heavier items.

## a summary plot - bar version
<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/summary_plot_rf.png" height="800" width="600" >

Feature found by shap are not exactly the same as previous one, the first and the second are the same. In shap, the supermarket type 3 go up in to third place. The item visibility went down to the last. However, we have new feature - Establishment Year.

## a summary plot - dot version
<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/summary_plot_dot.png" height="800" width="600" >
 
 ### interpretation of the top 3 most important features
- Item MRP
    - The Sales will be higher if the items prices are higher
- Outlet type Grocery Store
    - it will affect sales.
- Outlet Type Supermarket Type 1
    - more supermarket type 3, it will increasing more sales.
    
### Local Explanations
- Below are the Force Plots and Lime Explanations for high MRP and Low MRP

<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/forceplot1.png" height="400" width="1000" >
<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/forceplot2.png" height="400" width="1000" >


<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/lime1.png" height="600" width="800" >
<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Data/lime2.png" height="600" width="800" >




## For Further Information
### For any additional questions, please contact:
- LiPing Liu
- ivyliuzp@gmail.com
