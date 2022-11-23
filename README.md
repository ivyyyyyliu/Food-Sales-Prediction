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


<img src="https://github.com/ivyyyyyliu/Food-Sales-Prediction/blob/main/Explanatory%201.png" height="300" width="500" >

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


## For Further Information
### For any additional questions, please contact:
- LiPing Liu
- ivyliuzp@gmail.com
