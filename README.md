# Deliveroo-Test-for-Machine-Learning-Engineering

Appendix: Data Schema and Description

Filename : orders.csv

Column Name	Type	Description
order_acknowledged_at	String (timestamp)	Timestamp (local timezone) indicating when the order is acknowledged by the restaurant.
order_ready_at	String (timestamp)	Timestamp (local timezone) indicating when the food is ready.
order_value_gbp	Float	Value of the order in GBP.
restaurant_id	Integer	Unique restaurant identifier.
number_of_items	Integer	Number of items in the order.
prep_time_seconds	Integer	(order_ready_at - order_acknowledged_at) in seconds. This is the food preparation time and what you should model.
Filename : restaurants.csv

Column Name	Type	Description
restaurant_id	Integer	Unique restaurant identifier
country	String	Country where the restaurant is
city	String	City where the restaurant is
type_of_food	String	Type of food prepared by the restaurant
