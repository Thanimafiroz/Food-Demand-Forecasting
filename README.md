# Food-Demand-Forecasting

## Data Acquisition
The data was provided by the meal delivery company. The dataset, present in csv
format, contains
1. Product(Meal) features such as category, sub-category, current price and discount.
2. Information for fulfillment center like center area, city information etc.
3. Historical data of demand for a product-center combination (Weeks: 1 to 145)
4. Future data of product-center combination for prediction (Weeks: 146 to 155)

## Data Analysis
Below steps were taken to analyse the dataset
![image](https://user-images.githubusercontent.com/101709975/220565109-b17f218c-1e0e-4c26-95d9-a0a8df9d2d76.png)
![image](https://user-images.githubusercontent.com/101709975/220565322-666b65b6-359f-4348-8b83-203a5ac0e1ce.png)

## Outliers
Action on outliers will be taken during the modeling based on the performance of
model with and without outliers.

## Missing Records
Missing records can be because to below two reasons:
1. There is actually no sales for that meal, center and weeks combination
2. Records were not captured due to technical error
Reason will become more clear after exploring data and then action can be taken.

## Data Merging
All three data are present in different dataframes. Hence, its required to merge them
into one dataframe. Below steps were taken to merge the dataset
1. Left join on training data and meal information on meal_id.
2. Left join on training data and fulfilment center information on center_id.
Same steps were taken for test data.

