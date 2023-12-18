# Business Goal
Estimate the Unit Sales of Walmart retail goods to support their strategic development, make tactical decisions, and manage their demand and supply planning processes to avoid customer service issues and high inventory costs.


### Feature engineering
1. Sales-related features, like lag sales for different periods, and rolling sales for different periods. This type of feature reflects the trend component. 
2. Price-related features, like max, min standard deviation of prices for that product. 
3. Calendar related features. Different weekdays like Monday, Tuesday, and Wednesday; different months like January, February, and so on.

### Model Training
We will implement LightGBM via Python, and use different models for different weeks and 10 different models for different stores, so we will have 4 weeks* 10 stores = 40 models in total.

# Result
We successfully forecast sales of 28 days with less than 0.6 WRMSSE (Weighted Root Mean Squared Scaled Error).
