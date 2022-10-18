Case Study 4(ii) – Sales Reports

This case study should require adding a “check-out” button to the modified “Menu” page of case study 3(ii). On check out, the customer’s order should be inserted into the database.

As shown below is a sample administrative page for generating the daily sales reports based on daily customer’s orders.

Daily sales reports showing the total dollar and quantity sales for each of the products and categories (single and double shots) should be generated and presented in html format.

It should also be possible to include the most popular option category of the best selling product in the report.

Table:
product | category | itemPrice | orderQty | sales
jj | null | 2 | 0 | 0
cal | single | 2 | 0 | 0
cal | double | 3 | 0 | 0
ic | single | 4.75 | 0 | 0
ic | double | 5.75 | 0 | 0

Daily Sales Report:
Product | Total Dollar Sales | Quantity Sales
jj | jj.itemPrice x jj.orderQty | jj.orderQty
cal | cal.single.itemPrice x cal.single.orderQty + cal.double.itemPrice x cal.double.orderQty | cal.single.orderQty + cal.double.orderQty
ic | ic.single.itemPrice x ic.single.orderQty + ic.double.itemPrice x ic.double.orderQty | ic.single.orderQty + ic.double.orderQty

or

Daily Sales Report:
Product | Total Dollar Sales | Quantity Sales
jj | jj.sales | jj.orderQty
cal | cal.single.sales + cal.double.sales | cal.single.orderQty + cal.double.orderQty
ic | ic.single.sales + ic.double.sales | ic.single.orderQty + ic.double.orderQty

Category Sales Report:
Category | Total Dollar Sales | Quantity Sales
null | jj.itemPrice x jj.orderQty | jj.orderQty
single | cal.single.itemPrice x cal.single.orderQty + ic.single.itemPrice x ic.single.orderQty | cal.single.orderQty + ic.single.orderQty
double | cal.double.itemPrice x cal.double.orderQty + ic.double.itemPrice x ic.double.orderQty | cal.double.orderQty + ic.double.orderQty
