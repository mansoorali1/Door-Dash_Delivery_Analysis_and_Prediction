# Door-Dash_Delivery_Analysis_and_Prediction
When a consumer orders from a food delivery platform, providing an accurate estimated delivery time is crucial for ensuring a positive consumer experience. This project focuses on DoorDash delivery data, with a two-phase approach. Firstly, we analyze the data to extract valuable insights beneficial to the business. Secondly, we develop a model to predict the expected delivery duration, aiming to optimize the delivery process and enhance customer satisfaction.
## Available Features
`market_id`: A city/region in which DoorDash operates, e.g., Los Angeles, given in the data as an id

 `created_at`: Timestamp in UTC when the order was submitted by the consumer
to DoorDash. (Note this timestamp is in UTC, but in case you need
it, the actual timezone of the region was US/Pacific)

 `actual_delivery_time`: Timestamp in UTC when the order was delivered to the consumer

 `store_id`: an id representing the restaurant the order was submitted for

 `store_primary_category`: cuisine category of the restaurant, e.g., italian, asian

 `order_protocol`:  a store can receive orders from DoorDash through many modes.
This field represents an id denoting the protocol

`total_items`: total number of items in the order

 `subtotal`: total value of the order submitted (in cents)

 `num_distinct_items`:  number of distinct items included in the order

`min_item_price`:  price of the item with the least cost in the order (in cents)

`max_item_price`: price of the item with the highest cost in the order (in cents)

 `total_onshift_dashers`:  Number of available dashers who are within 10 miles of the store
at the time of order creation

`total_busy_dashers`: Subset of above total_onshift_dashers who are currently working
on an order

 `total_outstanding_orders`:  Number of orders within 10 miles of this order that are currently
being processed.

`estimated_order_place_duration`: Estimated time for the restaurant to receive the order from
DoorDash (in seconds)

`estimated_store_to_consumer_driving_duration`: Estimated travel time between store and consumer (in seconds)

`Output Variable`: actual_delivery_time - created_at
