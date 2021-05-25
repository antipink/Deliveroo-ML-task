# Deliveroo-Test-for-Machine-Learning-Engineering

## Appendix: Data Schema and Description

Filename : **orders.csv**

| Column Name       | Type    | Description                   |
|-------------------|---------|-------------------------------|
| order_acknowledged_at | String (timestamp) | Timestamp (local timezone) indicating when the order is acknowledged by the restaurant. |
| order_ready_at    | String (timestamp) | Timestamp (local timezone) indicating when the food is ready. |
| order_value_gbp       | Float   | Value of the order in GBP.|
| restaurant_id     | Integer | Unique restaurant identifier. |
| number_of_items   | Integer | Number of items in the order. |
| prep_time_seconds   | Integer | (order_ready_at - order_acknowledged_at) in seconds. This is the food preparation time and what you should model. |

Filename : **restaurants.csv**

| Column Name       | Type    | Description                   |
|-------------------|---------|-------------------------------|
| restaurant_id     | Integer | Unique restaurant identifier  |
| country           | String  | Country where the restaurant is |
| city              | String  | City where the restaurant is |
| type_of_food      | String  | Type of food prepared by the restaurant |


# ML Pratical
Build a model to make a decision on whether should offer compensation to an order or not.  
* What kind of ml problem is it? - Binary classification problem. If want to predict how much, it would be a regression problem. 
* What features will you chose? - 1. Checkbox to colleck what kind of complain is it. 2. How long it takes for prep food. 3. How long it takes for delivery. 4. Average rating of restaurant. 5. Number of complains from this user. 6. Number of complains received by this restaurant. 7. Average rating of the rider. 
* What is the business goal and metric?  -  There will be a trade off. If gave more compensation, it would damaged the profit but probably end up with more conversion. That is sth we want to optimize. Don't forget to mention AB testing, and how long should we run AB testing and how much trafic we should use.
* Which model will you choose? - RF or GBM
* Question arround feature enginneering.
