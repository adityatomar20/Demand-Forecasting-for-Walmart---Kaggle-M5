# Business Goal
The primary objective is to estimate the unit sales of Walmart retail goods, providing crucial support for strategic development, enabling tactical decision-making, and facilitating effective demand and supply planning. The ultimate goal is to mitigate customer service issues and minimize high inventory costs through informed and accurate sales forecasts.


### Feature engineering
To enhance the predictive power of the model, I incorporated various feature engineering techniques, including:

1. Sales-related Features: I integrated lag sales for different periods and rolling sales for distinct time frames. These features capture the trend component, providing valuable insights into sales patterns.

2. Price-related Features: I incorporated features such as maximum, minimum, and standard deviation of prices for each product. This approach allows the model to consider pricing dynamics, influencing sales predictions.

3. Calendar-related Features: I leveraged calendar-related information, including weekdays (e.g., Monday, Tuesday, Wednesday) and months (e.g., January, February). These features account for temporal variations in sales, contributing to a more nuanced and accurate forecasting model..

### Model Training
The implementation utilizes LightGBM in Python, leveraging its efficiency and effectiveness in handling large datasets. To account for store and temporal variations, I developed 40 models in total—10 models for each of the four weeks, considering different stores individually.

# Result
Through meticulous model training and feature engineering, I achieved successful sales forecasts for a 28-day period. The model's performance is assessed using the Weighted Root Mean Squared Scaled Error (WRMSSE), and I proudly achieved a performance metric of less than 0.6 WRMSSE. This result underscores the accuracy and reliability of the forecasting model in predicting Walmart's unit sales, providing a robust foundation for informed decision-making in the areas of inventory management and customer service optimization.
